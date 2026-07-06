<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ERP - Gestão Avançada de Pedidos</title>
    <style>
        :root {
            --bg-primary: #f8fafc;
            --card-bg: #ffffff;
            --text-main: #1e293b;
            --text-muted: #64748b;
            --primary: #4f46e5;
            --primary-hover: #4338ca;
            --success: #10b981;
            --danger: #ef4444;
            --warning: #f59e0b;
            --border: #e2e8f0;
            --radius: 12px;
            --shadow: 0 4px 6px -1px rgb(0 0 0 / 0.1), 0 2px 4px -2px rgb(0 0 0 / 0.1);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', system-ui, sans-serif;
        }

        body {
            background-color: var(--bg-primary);
            color: var(--text-main);
            padding: 2rem;
            line-height: 1.5;
        }

        .container {
            max-width: 1400px;
            margin: auto;
        }

        header {
            margin-bottom: 2rem;
        }

        h1 {
            font-size: 1.8rem;
            font-weight: 700;
        }

        /* Dashboard KPIs */
        .dashboard-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
            gap: 1.5rem;
            margin-bottom: 2rem;
        }

        .kpi-card {
            background: var(--card-bg);
            padding: 1.5rem;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
        }

        .kpi-title {
            font-size: 0.875rem;
            color: var(--text-muted);
            font-weight: 600;
            text-transform: uppercase;
        }

        .kpi-value {
            font-size: 1.5rem;
            font-weight: 700;
            margin-top: 0.5rem;
        }

        /* Layout Principal */
        .main-layout {
            display: grid;
            grid-template-columns: 350px 1fr;
            gap: 2rem;
        }

        @media (max-width: 1024px) {
            .main-layout {
                grid-template-columns: 1fr;
            }
        }

        .card {
            background: var(--card-bg);
            padding: 1.5rem;
            border-radius: var(--radius);
            box-shadow: var(--shadow);
            border: 1px solid var(--border);
            height: fit-content;
        }

        .card-title {
            font-size: 1.1rem;
            font-weight: 600;
            margin-bottom: 1.25rem;
            color: var(--text-main);
        }

        /* Formulários */
        .form-group {
            margin-bottom: 1rem;
        }

        label {
            display: block;
            font-size: 0.875rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: var(--text-main);
        }

        input, select {
            width: 100%;
            padding: 0.625rem;
            border: 1px solid var(--border);
            border-radius: 6px;
            font-size: 0.95rem;
            color: var(--text-main);
            outline: none;
            transition: border-color 0.2s;
        }

        input:focus, select:focus {
            border-color: var(--primary);
        }

        /* Botões */
        .btn {
            display: inline-flex;
            align-items: center;
            justify-content: center;
            width: 100%;
            padding: 0.75rem;
            border: none;
            border-radius: 6px;
            font-weight: 600;
            cursor: pointer;
            transition: background 0.2s;
        }

        .btn-primary { background: var(--primary); color: white; }
        .btn-primary:hover { background: var(--primary-hover); }
        .btn-danger { background: var(--danger); color: white; padding: 0.4rem 0.8rem; font-size: 0.85rem;}
        
        /* Filtros e Busca */
        .toolbar {
            display: flex;
            justify-content: space-between;
            align-items: center;
            gap: 1rem;
            margin-bottom: 1rem;
            flex-wrap: wrap;
        }

        .search-box {
            max-width: 300px;
        }

        /* Tabela Responsiva */
        .table-container {
            overflow-x: auto;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            text-align: left;
            font-size: 0.95rem;
        }

        th, td {
            padding: 1rem;
            border-bottom: 1px solid var(--border);
        }

        th {
            background: #f8fafc;
            color: var(--text-muted);
            font-weight: 600;
        }

        /* Badges de Status */
        .badge {
            display: inline-block;
            padding: 0.25rem 0.5rem;
            border-radius: 50px;
            font-size: 0.8rem;
            font-weight: 600;
        }

        .badge-pendente { background: #fef3c7; color: var(--warning); }
        .badge-faturamento { background: #e0f2fe; color: var(--primary); }
        .badge-entregue { background: #d1fae5; color: var(--success); }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>📦 Módulo ERP | Gestão de Pedidos</h1>
        </header>

        <!-- Indicadores de Desempenho (KPIs) -->
        <div class="dashboard-grid">
            <div class="kpi-card">
                <div class="kpi-title">Total de Pedidos</div>
                <div class="kpi-value" id="kpi-total-pedidos">0</div>
            </div>
            <div class="kpi-card">
                <div class="kpi-title">Faturamento Total</div>
                <div class="kpi-value" id="kpi-faturamento">R$ 0,00</div>
            </div>
            <div class="kpi-card">
                <div class="kpi-title">Pedidos Pendentes</div>
                <div class="kpi-value" id="kpi-pendentes" style="color: var(--warning)">0</div>
            </div>
        </div>

        <div class="main-layout">
            <!-- Formulário Lateral -->
            <div class="card">
                <div class="card-title">Emitir Novo Pedido</div>
                <form id="formPedido">
                    <div class="form-group">
                        <label>Cliente</label>
                        <input type="text" id="cliente" required placeholder="Nome ou Razão Social">
                    </div>
                    <div class="form-group">
                        <label>Produto</label>
                        <select id="produto" required>
                            <option value="" disabled selected>Selecione um produto</option>
                            <option value="Notebook Dell|4500">Notebook Dell - R$ 4.500,00</option>
                            <option value="Monitor LG 29'|1200">Monitor LG 29' - R$ 1.200,00</option>
                            <option value="Teclado Mecânico|350">Teclado Mecânico - R$ 350,00</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label>Quantidade</label>
                        <input type="number" id="quantidade" min="1" value="1" required>
                    </div>
                    <div class="form-group">
                        <label>Forma de Pagamento</label>
                        <select id="pagamento">
                            <option>Pix</option>
                            <option>Cartão de Crédito</option>
                            <option>Boleto Bancário</option>
                        </select>
                    </div>
                    <div class="form-group">
                        <label>Status Inicial</label>
                        <select id="status">
                            <option value="Pendente">Pendente</option>
                            <option value="Faturamento">Em Faturamento</option>
                            <option value="Entregue">Entregue</option>
                        </select>
                    </div>
                    <button type="submit" class="btn btn-primary">Gravar Pedido (Salvar)</button>
                </form>
            </div>

            <!-- Tabela Principal e Filtros -->
            <div class="card">
                <div class="toolbar">
                    <div class="card-title" style="margin:0;">Listagem de Vendas</div>
                    <input type="text" id="busca" class="search-box" placeholder="🔎 Buscar por cliente..." oninput="filtrarTabela()">
                </div>
                
                <div class="table-container">
                    <table>
                        <thead>
                            <tr>
                                <th>ID</th>
                                <th>Data</th>
                                <th>Cliente</th>
                                <th>Produto</th>
                                <th>Qtd</th>
                                <th>Total</th>
                                <th>Pagamento</th>
                                <th>Status</th>
                                <th>Ações</th>
                            </tr>
                        </thead>
                        <tbody id="tabelaPedidos">
                            <!-- Inserção via JS -->
                        </tbody>
                    </table>
                </div>
            </div>
        </div>
    </div>

    <script>
        let pedidos = [];
        let contadorId = 1001; // IDs no padrão ERP

        const form = document.getElementById("formPedido");

        form.addEventListener("submit", function(e) {
            e.preventDefault();
            adicionarPedido();
        });

        function adicionarPedido() {
            const cliente = document.getElementById("cliente").value;
