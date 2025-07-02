<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dashboard Administrativo - Jana Terra Photo</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;600&family=Playfair+Display:wght@400;600&display=swap');
        
        :root {
            --earth-beige: #F5E9D9;
            --earth-brown: #A38F72;
            --earth-olive: #7A9B76;
            --earth-terracotta: #D77A61;
            --earth-dark: #5D534A;
        }
        
        body {
            font-family: 'Montserrat', sans-serif;
            background-color: #f9f9f9;
        }
        
        .admin-container {
            display: flex;
            min-height: 100vh;
        }
        
        .sidebar {
            width: 260px;
            background: linear-gradient(to bottom, #5D534A, #3a332d);
            color: white;
            transition: all 0.3s ease;
            position: fixed;
            height: 100vh;
            overflow-y: auto;
            z-index: 1000;
        }
        
        .main-content {
            flex: 1;
            margin-left: 260px;
            transition: margin-left 0.3s ease;
        }
        
        .sidebar-header {
            padding: 20px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .sidebar-menu {
            padding: 15px 0;
        }
        
        .sidebar-menu a {
            display: flex;
            align-items: center;
            padding: 12px 20px;
            color: rgba(255, 255, 255, 0.8);
            text-decoration: none;
            transition: all 0.3s;
            border-left: 4px solid transparent;
        }
        
        .sidebar-menu a:hover,
        .sidebar-menu a.active {
            background: rgba(255, 255, 255, 0.1);
            color: white;
            border-left: 4px solid var(--earth-terracotta);
        }
        
        .sidebar-menu a i {
            margin-right: 12px;
            width: 20px;
            text-align: center;
        }
        
        .topbar {
            background: white;
            padding: 15px 30px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.05);
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 100;
        }
        
        .stat-card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            padding: 20px;
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        
        .stat-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 10px 15px rgba(0, 0, 0, 0.08);
        }
        
        .stat-card.income {
            border-top: 4px solid var(--earth-olive);
        }
        
        .stat-card.expenses {
            border-top: 4px solid var(--earth-terracotta);
        }
        
        .stat-card.profit {
            border-top: 4px solid #7A9B76;
        }
        
        .stat-card.clients {
            border-top: 4px solid #A38F72;
        }
        
        .card {
            background: white;
            border-radius: 10px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.05);
            padding: 25px;
        }
        
        .table-container {
            overflow-x: auto;
        }
        
        table {
            width: 100%;
            border-collapse: collapse;
        }
        
        th {
            background-color: #f5f7fa;
            text-align: left;
            padding: 12px 15px;
            font-weight: 600;
            color: var(--earth-dark);
            border-bottom: 2px solid #eaeaea;
        }
        
        td {
            padding: 12px 15px;
            border-bottom: 1px solid #eaeaea;
            color: #555;
        }
        
        tr:hover {
            background-color: #f9fafb;
        }
        
        .status-badge {
            padding: 4px 10px;
            border-radius: 20px;
            font-size: 0.8rem;
            font-weight: 500;
        }
        
        .status-pending {
            background-color: #fffbeb;
            color: #d97706;
        }
        
        .status-completed {
            background-color: #ecfdf5;
            color: #059669;
        }
        
        .status-canceled {
            background-color: #fef2f2;
            color: #dc2626;
        }
        
        .btn {
            padding: 8px 16px;
            border-radius: 6px;
            font-weight: 500;
            cursor: pointer;
            transition: all 0.2s;
        }
        
        .btn-primary {
            background-color: var(--earth-olive);
            color: white;
            border: none;
        }
        
        .btn-primary:hover {
            background-color: #6a8a66;
        }
        
        .btn-outline {
            background-color: transparent;
            border: 1px solid var(--earth-olive);
            color: var(--earth-olive);
        }
        
        .btn-outline:hover {
            background-color: rgba(122, 155, 118, 0.1);
        }
        
        .notification-badge {
            position: absolute;
            top: -5px;
            right: -5px;
            background-color: var(--earth-terracotta);
            color: white;
            border-radius: 50%;
            width: 20px;
            height: 20px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 0.7rem;
            font-weight: bold;
        }
        
        .mobile-menu-btn {
            display: none;
        }
        
        @media (max-width: 992px) {
            .sidebar {
                margin-left: -260px;
            }
            .sidebar.active {
                margin-left: 0;
            }
            .main-content {
                margin-left: 0;
            }
            .mobile-menu-btn {
                display: block;
            }
        }
    </style>
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        earth: {
                            beige: '#F5E9D9',
                            brown: '#A38F72',
                            olive: '#7A9B76',
                            terracotta: '#D77A61',
                            dark: '#5D534A'
                        }
                    },
                    fontFamily: {
                        sans: ['Montserrat', 'sans-serif'],
                        serif: ['Playfair Display', 'serif'],
                    }
                }
            }
        }
    </script>
</head>
<body>
    <div class="admin-container">
        <!-- Sidebar -->
        <div class="sidebar" id="sidebar">
            <div class="sidebar-header">
                <h1 class="text-xl font-serif font-bold text-white">Jana Terra Photo</h1>
                <p class="text-sm text-gray-300 mt-1">Dashboard Administrativo</p>
            </div>
            
            <div class="sidebar-menu">
                <a href="#dashboard" class="active">
                    <i class="fas fa-tachometer-alt"></i>
                    Dashboard
                </a>
                <a href="#financeiro">
                    <i class="fas fa-chart-line"></i>
                    Financeiro
                </a>
                <a href="#sessoes">
                    <i class="fas fa-calendar-alt"></i>
                    Sessões
                </a>
                <a href="#clientes">
                    <i class="fas fa-users"></i>
                    Clientes
                </a>
                <a href="#galeria">
                    <i class="fas fa-images"></i>
                    Galeria
                </a>
                <a href="#website">
                    <i class="fas fa-globe"></i>
                    Gestão do Site
                </a>
                <a href="#relatorios">
                    <i class="fas fa-file-alt"></i>
                    Relatórios
                </a>
                <a href="#configuracoes">
                    <i class="fas fa-cog"></i>
                    Configurações
                </a>
            </div>
            
            <div class="p-5 mt-8">
                <div class="bg-earth-olive bg-opacity-20 p-4 rounded-lg border border-earth-olive border-opacity-30">
                    <p class="text-sm text-white text-opacity-80">
                        <i class="fas fa-info-circle mr-2"></i>
                        Último login: 02/07/2025 às 10:15
                    </p>
                </div>
            </div>
        </div>
        
        <!-- Main Content -->
        <div class="main-content">
            <!-- Topbar -->
            <div class="topbar">
                <div class="flex items-center">
                    <button id="menu-toggle" class="mobile-menu-btn mr-4 text-earth-dark">
                        <i class="fas fa-bars text-xl"></i>
                    </button>
                    <h2 class="text-xl font-bold text-earth-dark">Dashboard</h2>
                </div>
                
                <div class="flex items-center space-x-6">
                    <div class="relative">
                        <button class="text-earth-dark hover:text-earth-terracotta relative">
                            <i class="fas fa-bell text-xl"></i>
                            <span class="notification-badge">3</span>
                        </button>
                    </div>
                    
                    <div class="relative">
                        <button class="flex items-center space-x-2">
                            <div class="w-10 h-10 rounded-full bg-earth-olive flex items-center justify-center text-white">
                                <i class="fas fa-user"></i>
                            </div>
                            <div class="hidden md:block text-left">
                                <p class="font-medium text-earth-dark">Admin</p>
                                <p class="text-sm text-earth-brown">Administrador</p>
                            </div>
                        </button>
                    </div>
                </div>
            </div>
            
            <!-- Dashboard Content -->
            <div class="p-6">
                <!-- Stats Section -->
                <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 mb-8">
                    <div class="stat-card income">
                        <div class="flex items-center justify-between">
                            <div>
                                <p class="text-sm text-earth-brown mb-1">Receitas (Mês)</p>
                                <h3 class="text-2xl font-bold text-earth-dark">R$ 8.240,00</h3>
                            </div>
                            <div class="bg-earth-olive bg-opacity-20 p-3 rounded-full text-earth-olive">
                                <i class="fas fa-money-bill-wave text-xl"></i>
                            </div>
                        </div>
                        <div class="mt-3">
                            <p class="text-sm text-green-600 flex items-center">
                                <i class="fas fa-arrow-up mr-1"></i> 12% vs mês anterior
                            </p>
                        </div>
                    </div>
                    
                    <div class="stat-card expenses">
                        <div class="flex items-center justify-between">
                            <div>
                                <p class="text-sm text-earth-brown mb-1">Despesas (Mês)</p>
                                <h3 class="text-2xl font-bold text-earth-dark">R$ 2.150,00</h3>
                            </div>
                            <div class="bg-earth-terracotta bg-opacity-20 p-3 rounded-full text-earth-terracotta">
                                <i class="fas fa-file-invoice-dollar text-xl"></i>
                            </div>
                        </div>
                        <div class="mt-3">
                            <p class="text-sm text-red-600 flex items-center">
                                <i class="fas fa-arrow-up mr-1"></i> 5% vs mês anterior
                            </p>
                        </div>
                    </div>
                    
                    <div class="stat-card profit">
                        <div class="flex items-center justify-between">
                            <div>
                                <p class="text-sm text-earth-brown mb-1">Lucro (Mês)</p>
                                <h3 class="text-2xl font-bold text-earth-dark">R$ 6.090,00</h3>
                            </div>
                            <div class="bg-earth-olive bg-opacity-20 p-3 rounded-full text-earth-olive">
                                <i class="fas fa-piggy-bank text-xl"></i>
                            </div>
                        </div>
                        <div class="mt-3">
                            <p class="text-sm text-green-600 flex items-center">
                                <i class="fas fa-arrow-up mr-1"></i> 15% vs mês anterior
                            </p>
                        </div>
                    </div>
                    
                    <div class="stat-card clients">
                        <div class="flex items-center justify-between">
                            <div>
                                <p class="text-sm text-earth-brown mb-1">Novos Clientes</p>
                                <h3 class="text-2xl font-bold text-earth-dark">14</h3>
                            </div>
                            <div class="bg-earth-brown bg-opacity-20 p-3 rounded-full text-earth-brown">
                                <i class="fas fa-user-plus text-xl"></i>
                            </div>
                        </div>
                        <div class="mt-3">
                            <p class="text-sm text-green-600 flex items-center">
                                <i class="fas fa-arrow-up mr-1"></i> 8% vs mês anterior
                            </p>
                        </div>
                    </div>
                </div>
                
                <!-- Charts and Tables Section -->
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-6 mb-8">
                    <!-- Revenue Chart -->
                    <div class="card">
                        <div class="flex justify-between items-center mb-6">
                            <h3 class="text-lg font-bold text-earth-dark">Desempenho Financeiro</h3>
                            <select class="border border-gray-300 rounded px-3 py-1 text-sm">
                                <option>Últimos 6 meses</option>
                                <option>2025</option>
                                <option>2024</option>
                            </select>
                        </div>
                        <div class="h-72">
                            <canvas id="revenueChart"></canvas>
                        </div>
                    </div>
                    
                    <!-- Sessions Chart -->
                    <div class="card">
                        <div class="flex justify-between items-center mb-6">
                            <h3 class="text-lg font-bold text-earth-dark">Sessões por Tipo</h3>
                            <select class="border border-gray-300 rounded px-3 py-1 text-sm">
                                <option>Últimos 3 meses</option>
                                <option>2025</option>
                                <option>2024</option>
                            </select>
                        </div>
                        <div class="h-72">
                            <canvas id="sessionsChart"></canvas>
                        </div>
                    </div>
                </div>
                
                <!-- Recent Sessions and Financial Activity -->
                <div class="grid grid-cols-1 lg:grid-cols-2 gap-6 mb-8">
                    <!-- Recent Sessions -->
                    <div class="card">
                        <div class="flex justify-between items-center mb-6">
                            <h3 class="text-lg font-bold text-earth-dark">Sessões Recentes</h3>
                            <button class="btn btn-outline">
                                <i class="fas fa-plus mr-1"></i> Nova Sessão
                            </button>
                        </div>
                        <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Cliente</th>
                                        <th>Data</th>
                                        <th>Tipo</th>
                                        <th>Status</th>
                                        <th>Ações</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td class="font-medium">Carolina Mendes</td>
                                        <td>15/07/2025</td>
                                        <td>Casais</td>
                                        <td>
                                            <span class="status-badge status-completed">Realizada</span>
                                        </td>
                                        <td>
                                            <button class="text-earth-olive hover:text-earth-brown">
                                                <i class="fas fa-eye"></i>
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Mariana Oliveira</td>
                                        <td>18/07/2025</td>
                                        <td>Infantil</td>
                                        <td>
                                            <span class="status-badge status-pending">Agendada</span>
                                        </td>
                                        <td>
                                            <button class="text-earth-olive hover:text-earth-brown">
                                                <i class="fas fa-eye"></i>
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Ricardo Silva</td>
                                        <td>20/07/2025</td>
                                        <td>Evento</td>
                                        <td>
                                            <span class="status-badge status-pending">Agendada</span>
                                        </td>
                                        <td>
                                            <button class="text-earth-olive hover:text-earth-brown">
                                                <i class="fas fa-eye"></i>
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Fernanda Costa</td>
                                        <td>05/07/2025</td>
                                        <td>Família</td>
                                        <td>
                                            <span class="status-badge status-completed">Realizada</span>
                                        </td>
                                        <td>
                                            <button class="text-earth-olive hover:text-earth-brown">
                                                <i class="fas fa-eye"></i>
                                            </button>
                                        </td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Juliana Ramos</td>
                                        <td>25/06/2025</td>
                                        <td>Gestante</td>
                                        <td>
                                            <span class="status-badge status-canceled">Cancelada</span>
                                        </td>
                                        <td>
                                            <button class="text-earth-olive hover:text-earth-brown">
                                                <i class="fas fa-eye"></i>
                                            </button>
                                        </td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>
                    
                    <!-- Financial Activity -->
                    <div class="card">
                        <div class="flex justify-between items-center mb-6">
                            <h3 class="text-lg font-bold text-earth-dark">Atividade Financeira</h3>
                            <button class="btn btn-outline">
                                <i class="fas fa-plus mr-1"></i> Novo Pagamento
                            </button>
                        </div>
                        <div class="table-container">
                            <table>
                                <thead>
                                    <tr>
                                        <th>Descrição</th>
                                        <th>Data</th>
                                        <th>Valor</th>
                                        <th>Tipo</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                        <td class="font-medium">Sessão Casal - Carolina</td>
                                        <td>16/07/2025</td>
                                        <td class="text-green-600 font-medium">R$ 1.200,00</td>
                                        <td>Receita</td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Aluguel Estúdio</td>
                                        <td>15/07/2025</td>
                                        <td class="text-red-600 font-medium">- R$ 800,00</td>
                                        <td>Despesa</td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Sessão Família - Fernanda</td>
                                        <td>06/07/2025</td>
                                        <td class="text-green-600 font-medium">R$ 950,00</td>
                                        <td>Receita</td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Manutenção Equipamento</td>
                                        <td>05/07/2025</td>
                                        <td class="text-red-600 font-medium">- R$ 350,00</td>
                                        <td>Despesa</td>
                                    </tr>
                                    <tr>
                                        <td class="font-medium">Sessão Infantil - Pedro</td>
                                        <td>30/06/2025</td>
                                        <td class="text-green-600 font-medium">R$ 850,00</td>
                                        <td>Receita</td>
                                    </tr>
                                </tbody>
                            </table>
                        </div>
                    </div>
                </div>
                
                <!-- Website Management -->
                <div class="card mb-8">
                    <div class="flex justify-between items-center mb-6">
                        <h3 class="text-lg font-bold text-earth-dark">Gestão do Site</h3>
                        <div class="flex space-x-2">
                            <button class="btn btn-outline">
                                <i class="fas fa-sync-alt mr-1"></i> Atualizar
                            </button>
                            <button class="btn btn-primary">
                                <i class="fas fa-plus mr-1"></i> Novo Conteúdo
                            </button>
                        </div>
                    </div>
                    
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                        <div class="border border-gray-200 rounded-lg p-4">
                            <div class="flex items-center mb-3">
                                <div class="bg-earth-beige p-3 rounded-full mr-3">
                                    <i class="fas fa-file-alt text-earth-terracotta"></i>
                                </div>
                                <h4 class="font-bold">Conteúdo da Página</h4>
                            </div>
                            <p class="text-sm text-gray-600 mb-3">Atualize textos, imagens e seções do site</p>
                            <button class="btn btn-outline w-full">
                                Editar Conteúdo
                            </button>
                        </div>
                        
                        <div class="border border-gray-200 rounded-lg p-4">
                            <div class="flex items-center mb-3">
                                <div class="bg-earth-beige p-3 rounded-full mr-3">
                                    <i class="fas fa-images text-earth-terracotta"></i>
                                </div>
                                <h4 class="font-bold">Portfólio</h4>
                            </div>
                            <p class="text-sm text-gray-600 mb-3">Gerencie as fotos exibidas no portfólio</p>
                            <button class="btn btn-outline w-full">
                                Gerenciar Portfólio
                            </button>
                        </div>
                        
                        <div class="border border-gray-200 rounded-lg p-4">
                            <div class="flex items-center mb-3">
                                <div class="bg-earth-beige p-3 rounded-full mr-3">
                                    <i class="fas fa-chart-bar text-earth-terracotta"></i>
                                </div>
                                <h4 class="font-bold">Análise de Tráfego</h4>
                            </div>
                            <p class="text-sm text-gray-600 mb-3">Acompanhe visitas e engajamento do site</p>
                            <button class="btn btn-outline w-full">
                                Ver Relatórios
                            </button>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        // Initialize Charts
        document.addEventListener('DOMContentLoaded', function() {
            // Revenue Chart
            const revenueCtx = document.getElementById('revenueChart').getContext('2d');
            const revenueChart = new Chart(revenueCtx, {
                type: 'line',
                data: {
                    labels: ['Jan', 'Fev', 'Mar', 'Abr', 'Mai', 'Jun', 'Jul'],
                    datasets: [
                        {
                            label: 'Receitas',
                            data: [6500, 7200, 7800, 8200, 8900, 9200, 8240],
                            borderColor: '#7A9B76',
                            backgroundColor: 'rgba(122, 155, 118, 0.1)',
                            tension: 0.3,
                            fill: true
                        },
                        {
                            label: 'Despesas',
                            data: [1800, 1950, 2100, 2000, 2300, 2050, 2150],
                            borderColor: '#D77A61',
                            backgroundColor: 'rgba(215, 122, 97, 0.1)',
                            tension: 0.3,
                            fill: true
                        }
                    ]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: {
                            position: 'top',
                        }
                    },
                    scales: {
                        y: {
                            beginAtZero: true,
                            grid: {
                                drawBorder: false
                            }
                        },
                        x: {
                            grid: {
                                display: false
                            }
                        }
                    }
                }
            });
            
            // Sessions Chart
            const sessionsCtx = document.getElementById('sessionsChart').getContext('2d');
            const sessionsChart = new Chart(sessionsCtx, {
                type: 'bar',
                data: {
                    labels: ['Casais', 'Infantil', 'Eventos', 'Família', 'Gestante'],
                    datasets: [{
                        label: 'Sessões',
                        data: [14, 18, 9, 12, 7],
                        backgroundColor: [
                            '#7A9B76',
                            '#D77A61',
                            '#A38F72',
                            '#F5E9D9',
                            '#5D534A'
                        ],
                        borderRadius: 5,
                        borderSkipped: false
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: {
                        legend: {
                            display: false
                        }
                    },
                    scales: {
                        y: {
                            beginAtZero: true,
                            grid: {
                                drawBorder: false
                            }
                        },
                        x: {
                            grid: {
                                display: false
                            }
                        }
                    }
                }
            });
        });
        
        // Toggle sidebar on mobile
        document.getElementById('menu-toggle').addEventListener('click', function() {
            document.getElementById('sidebar').classList.toggle('active');
        });
        
        // Close sidebar when clicking outside
        document.addEventListener('click', function(event) {
            const sidebar = document.getElementById('sidebar');
            const menuToggle = document.getElementById('menu-toggle');
            
            if (window.innerWidth < 992 && 
                !sidebar.contains(event.target) && 
                !menuToggle.contains(event.target) &&
                sidebar.classList.contains('active')) {
                sidebar.classList.remove('active');
            }
        });
        
        // Highlight active menu item
        document.querySelectorAll('.sidebar-menu a').forEach(item => {
            item.addEventListener('click', function() {
                document.querySelectorAll('.sidebar-menu a').forEach(link => {
                    link.classList.remove('active');
                });
                this.classList.add('active');
                
                // Close sidebar on mobile after selection
                if (window.innerWidth < 992) {
                    document.getElementById('sidebar').classList.remove('active');
                }
            });
        });
    </script>
</body>
</html>
