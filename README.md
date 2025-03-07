<html lang="pt">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quadro de Tarefas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f4f4f4;
            margin: 0;
            padding: 0;
        }
        .tabs {
            display: flex;
            cursor: pointer;
            margin-top: 20px;
            justify-content: center;
            background-color: #333;
        }
        .tab {
            padding: 10px 20px;
            color: white;
            background-color: #555;
            border: 1px solid #333;
            margin-right: 2px;
        }
        .tab.active {
            background-color: #f1c40f;
            color: black;
        }
        .tab-content {
            display: none;
            padding: 20px;
            background-color: white;
            border: 1px solid #ddd;
            border-top: none;
        }
        .tab-content.active {
            display: block;
        }
        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 20px;
        }
        table, th, td {
            border: 1px solid #ddd;
        }
        th, td {
            padding: 10px;
            text-align: left;
        }
    </style>
    <script>
        function openTab(event, tabName) {
            var i, tabcontent, tablinks;
            tabcontent = document.getElementsByClassName("tab-content");
            for (i = 0; i < tabcontent.length; i++) {
                tabcontent[i].style.display = "none";
            }
            tablinks = document.getElementsByClassName("tab");
            for (i = 0; i < tablinks.length; i++) {
                tablinks[i].className = tablinks[i].className.replace(" active", "");
            }
            document.getElementById(tabName).style.display = "block";
            event.currentTarget.className += " active";
        }
    </script>
</head>
<body>

    <div class="tabs">
        <div class="tab active" onclick="openTab(event, 'tpc-t1')">TPC T.1</div>
        <div class="tab" onclick="openTab(event, 'tpc-t2')">TPC T.2</div>
        <div class="tab" onclick="openTab(event, 'tpc-t3')">TPC T.3</div>
        <div class="tab" onclick="openTab(event, 'tpc-t4')">TPC T.4</div>
    </div>

    <div id="tpc-t1" class="tab-content active">
        <h2>TPC T.1</h2>
        <table>
            <tr>
                <th>Tarefa</th>
                <th>Link</th>
            </tr>
            <tr>
                <td>Tarefa 1</td>
                <td><a href="https://simone-zua17.github.io/TCP.T.1//">Link para Tarefa 1</a></td>
            </tr>
        </table>
    </div>

    <div id="tpc-t2" class="tab-content">
        <h2>TPC T.2</h2>
        <table>
            <tr>
                <th>Tarefa</th>
                <th>Link</th>
            </tr>
            <tr>
                <td>Tarefa 1</td>
                <td><a href="https://simone-zua17.github.io/TPC-T.2/">Link para Tarefa 1</a></td>
            </tr>
        </table>
    </div>

    <div id="tpc-t3" class="tab-content">
        <h2>TPC T.3</h2>
        <table>
            <tr>
                <th>Tarefa</th>
                <th>Link</th>
            </tr>
            <tr>
                <td>Tarefa 1</td>
                <td><a href="https://simone-zua17.github.io/TPC-T3/">Link para Tarefa 1</a></td>
            </tr>
        </table>
    </div>

    <div id="tpc-t4" class="tab-content">
        <h2>TPC T.4</h2>
        <table>
            <tr>
                <th>Tarefa</th>
                <th>Link</th>
            </tr>
            <tr>
                <td>Tarefa 1</td>
                <td><a href="URL_DO_TPC_T4">Link para Tarefa 1</a></td> <!-- Substitua pelo link real do TPC T.4 -->
            </tr>
        </table>
    </div>

</body>
</html>
