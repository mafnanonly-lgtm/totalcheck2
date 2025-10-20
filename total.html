<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TotalCheck AI | Ultimate Personal Finance Dashboard</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
    <style>
        :root {
            --primary: #00c6ff; --primary-dark: #0072ff; --secondary: #7a00ff; --accent: #ff0080;
            --success: #00ff9d; --warning: #ffbd00; --danger: #ff2e63; --dark: #0f172a;
            --darker: #020617; --light: #f8fafc; --gray: #64748b; --card-bg: rgba(30, 41, 59, 0.9);
            --card-border: rgba(255, 255, 255, 0.1); --card-shadow: 0 20px 40px rgba(0, 0, 0, 0.6); --glow: 0 0 20px;
        }
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; }
        body { background: linear-gradient(135deg, var(--darker) 0%, var(--dark) 100%); color: var(--light); min-height: 100vh; overflow-x: hidden; }
        .particles-container { position: fixed; top: 0; left: 0; width: 100%; height: 100%; z-index: -1; background: linear-gradient(135deg, var(--darker) 0%, var(--dark) 100%); }
        .particle { position: absolute; border-radius: 50%; background: rgba(0, 198, 255, 0.5); animation: float 15s infinite linear; }
        @keyframes float { 0% { transform: translateY(0) translateX(0); opacity: 0; } 10% { opacity: 1; } 90% { opacity: 1; } 100% { transform: translateY(-100vh) translateX(100px); opacity: 0; } }
        .container { width: 100%; max-width: 1600px; margin: 0 auto; padding: 0 20px; }
        
        .auth-container { display: flex; justify-content: center; align-items: center; min-height: 100vh; padding: 20px; }
        .auth-box { background-color: var(--card-bg); border-radius: 20px; padding: 50px; width: 100%; max-width: 500px; box-shadow: var(--card-shadow); backdrop-filter: blur(15px); border: 1px solid var(--card-border); animation: slideUp 0.5s ease-out; position: relative; overflow: hidden; }
        .auth-box::before { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 5px; background: linear-gradient(90deg, var(--primary), var(--accent)); }
        @keyframes slideUp { from { transform: translateY(30px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .auth-header { text-align: center; margin-bottom: 40px; }
        .auth-header h1 { font-size: 36px; margin-bottom: 10px; background: linear-gradient(90deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; font-weight: 800; text-shadow: var(--glow) rgba(0, 198, 255, 0.5); }
        .auth-header p { opacity: 0.8; font-size: 16px; }
        .auth-tabs { display: flex; margin-bottom: 30px; border-bottom: 1px solid rgba(255, 255, 255, 0.1); }
        .auth-tab { padding: 15px 30px; cursor: pointer; font-weight: 600; color: var(--light); opacity: 0.7; transition: all 0.3s ease; position: relative; }
        .auth-tab.active { opacity: 1; color: var(--primary); }
        .auth-tab.active::after { content: ''; position: absolute; bottom: -1px; left: 0; width: 100%; height: 3px; background: linear-gradient(90deg, var(--primary), var(--accent)); border-radius: 3px 3px 0 0; }
        .auth-form { display: none; }
        .auth-form.active { display: block; animation: fadeIn 0.5s ease-out; }
        @keyframes fadeIn { from { opacity: 0; } to { opacity: 1; } }
        .form-group { margin-bottom: 25px; }
        .form-group label { display: block; margin-bottom: 10px; font-weight: 500; font-size: 14px; text-transform: uppercase; letter-spacing: 1px; opacity: 0.8; }
        .form-control { width: 100%; padding: 16px 20px; background-color: rgba(255, 255, 255, 0.08); border: 1px solid rgba(255, 255, 255, 0.1); border-radius: 12px; color: var(--light); font-size: 16px; transition: all 0.3s ease; }
        .form-control:focus { outline: none; border-color: var(--primary); box-shadow: 0 0 0 3px rgba(0, 198, 255, 0.3); background-color: rgba(255, 255, 255, 0.12); }
        .btn { display: inline-block; padding: 16px 30px; background: linear-gradient(90deg, var(--primary), var(--secondary)); color: white; border: none; border-radius: 12px; font-weight: 600; cursor: pointer; transition: all 0.3s ease; text-align: center; font-size: 16px; position: relative; overflow: hidden; }
        .btn::before { content: ''; position: absolute; top: 0; left: -100%; width: 100%; height: 100%; background: linear-gradient(90deg, transparent, rgba(255, 255, 255, 0.2), transparent); transition: 0.5s; }
        .btn:hover::before { left: 100%; }
        .btn:hover { transform: translateY(-3px); box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3); }
        .btn-full { width: 100%; }
        .btn-outline { background: transparent; border: 2px solid var(--primary); color: var(--primary); }
        .btn-outline:hover { background: var(--primary); color: white; }
        .error-message, .success-message { font-size: 14px; margin-top: 10px; text-align: center; display: none; padding: 10px; border-radius: 8px; }
        .error-message { color: var(--danger); background: rgba(255, 46, 99, 0.1); }
        .success-message { color: var(--success); background: rgba(0, 255, 157, 0.1); }
        
        .dashboard { display: none; min-height: 100vh; }
        .header { display: flex; justify-content: space-between; align-items: center; padding: 25px 0; border-bottom: 1px solid rgba(255, 255, 255, 0.1); }
        .logo { font-size: 28px; font-weight: 800; background: linear-gradient(90deg, var(--primary), var(--accent)); -webkit-background-clip: text; -webkit-text-fill-color: transparent; cursor: pointer; display: flex; align-items: center; gap: 10px; text-shadow: var(--glow) rgba(0, 198, 255, 0.5); }
        .logo i { font-size: 32px; }
        .current-time { font-size: 16px; opacity: 0.7; background: rgba(255, 255, 255, 0.05); padding: 10px 20px; border-radius: 30px; }
        .user-info { display: flex; align-items: center; gap: 15px; }
        .user-avatar { width: 50px; height: 50px; border-radius: 50%; background: linear-gradient(135deg, var(--primary), var(--secondary)); display: flex; align-items: center; justify-content: center; font-weight: 700; font-size: 20px; box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3); }
        
        .main-content { display: grid; grid-template-columns: 300px 1fr; gap: 30px; padding: 30px 0; }
        .sidebar { background-color: var(--card-bg); border-radius: 20px; padding: 30px; height: fit-content; box-shadow: var(--card-shadow); border: 1px solid var(--card-border); position: sticky; top: 30px; }
        .nav-links { list-style: none; }
        .nav-links li { margin-bottom: 10px; }
        .nav-links a { display: flex; align-items: center; padding: 16px 20px; color: var(--light); text-decoration: none; border-radius: 12px; transition: all 0.3s ease; position: relative; overflow: hidden; }
        .nav-links a i { margin-right: 15px; width: 20px; text-align: center; font-size: 20px; transition: all 0.3s ease; }
        .nav-links a:hover, .nav-links a.active { background: linear-gradient(90deg, var(--primary), var(--secondary)); color: white; transform: translateX(5px); box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2); }
        .nav-links a.active::before { content: ''; position: absolute; top: 0; left: 0; width: 5px; height: 100%; background: var(--accent); }
        
        .dashboard-content { display: grid; grid-template-columns: repeat(2, 1fr); gap: 25px; }
        .card { background-color: var(--card-bg); border-radius: 20px; padding: 30px; box-shadow: var(--card-shadow); border: 1px solid var(--card-border); transition: transform 0.3s ease, box-shadow 0.3s ease; position: relative; overflow: hidden; }
        .card::before { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 5px; background: linear-gradient(90deg, var(--primary), var(--accent)); }
        .card:hover { transform: translateY(-10px); box-shadow: 0 20px 40px rgba(0, 0, 0, 0.4); }
        .card-full { grid-column: 1 / -1; }
        .card-header { display: flex; justify-content: space-between; align-items: center; margin-bottom: 25px; }
        .card-title { font-size: 22px; font-weight: 700; display: flex; align-items: center; gap: 10px; }
        .card-title i { color: var(--primary); }
        
        .stats-grid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 20px; margin-bottom: 30px; }
        .stat-card { background: linear-gradient(135deg, var(--primary), var(--secondary)); border-radius: 16px; padding: 30px; text-align: center; box-shadow: 0 10px 25px rgba(0, 0, 0, 0.3); transition: transform 0.3s ease; position: relative; overflow: hidden; }
        .stat-card::before { content: ''; position: absolute; top: 0; left: 0; width: 100%; height: 100%; background: linear-gradient(135deg, rgba(255,255,255,0.1), transparent); }
        .stat-card:hover { transform: translateY(-8px); box-shadow: 0 15px 30px rgba(0, 0, 0, 0.4); }
        .stat-value { font-size: 36px; font-weight: 800; margin-bottom: 10px; position: relative; z-index: 1; }
        .stat-label { font-size: 16px; opacity: 0.9; position: relative; z-index: 1; }
        
        .expense-form { display: none; grid-template-columns: repeat(2, 1fr); gap: 20px; margin-bottom: 25px; padding: 25px; background: rgba(255, 255, 255, 0.05); border-radius: 16px; }
        .expense-list { max-height: 500px; overflow-y: auto; padding-right: 10px; }
        .expense-list::-webkit-scrollbar { width: 6px; }
        .expense-list::-webkit-scrollbar-track { background: rgba(255, 255, 255, 0.05); border-radius: 10px; }
        .expense-list::-webkit-scrollbar-thumb { background: var(--primary); border-radius: 10px; }
        .expense-item { display: flex; justify-content: space-between; align-items: center; padding: 20px; border-bottom: 1px solid rgba(255, 255, 255, 0.1); transition: background 0.3s; border-radius: 12px; }
        .expense-item:hover { background: rgba(255, 255, 255, 0.05); transform: translateX(5px); }
        .expense-info h4 { margin-bottom: 8px; font-size: 18px; }
        .expense-meta { font-size: 14px; opacity: 0.7; display: flex; align-items: center; gap: 10px; }
        .expense-amount { font-weight: 700; font-size: 20px; }
        .expense-actions { display: flex; gap: 10px; }
        .action-btn { background: none; border: none; color: var(--light); cursor: pointer; font-size: 16px; transition: all 0.3s ease; padding: 8px; border-radius: 8px; width: 40px; height: 40px; display: flex; align-items: center; justify-content: center; }
        .action-btn.edit:hover { color: var(--success); background: rgba(0, 255, 157, 0.1); transform: scale(1.1); }
        .action-btn.delete:hover { color: var(--danger); background: rgba(255, 46, 99, 0.1); transform: scale(1.1); }
        
        .chart-container { height: 350px; margin-top: 20px; }
        
        .ai-assistant { position: fixed; bottom: 30px; right: 30px; z-index: 100; }
        .ai-toggle { width: 80px; height: 80px; border-radius: 50%; background: linear-gradient(135deg, var(--primary), var(--accent)); display: flex; align-items: center; justify-content: center; color: white; font-size: 32px; cursor: pointer; box-shadow: 0 10px 30px rgba(0, 0, 0, 0.4); transition: all 0.3s ease; animation: pulse 2s infinite; position: relative; }
        @keyframes pulse { 0% { box-shadow: 0 0 0 0 rgba(0, 198, 255, 0.7); } 70% { box-shadow: 0 0 0 20px rgba(0, 198, 255, 0); } 100% { box-shadow: 0 0 0 0 rgba(0, 198, 255, 0); } }
        .ai-toggle:hover { transform: scale(1.1) rotate(10deg); }
        .ai-chat { position: absolute; bottom: 100px; right: 0; width: 400px; height: 550px; background-color: var(--card-bg); border-radius: 20px; box-shadow: 0 20px 50px rgba(0, 0, 0, 0.5); display: none; flex-direction: column; overflow: hidden; border: 1px solid var(--card-border); }
        .ai-chat.active { display: flex; animation: slideUp 0.3s ease-out; }
        .ai-header { padding: 25px; background: linear-gradient(90deg, var(--primary), var(--secondary)); color: white; font-weight: 700; display: flex; align-items: center; gap: 15px; font-size: 18px; }
        .ai-messages { flex: 1; padding: 25px; overflow-y: auto; display: flex; flex-direction: column; gap: 20px; }
        .ai-messages::-webkit-scrollbar { width: 6px; }
        .ai-messages::-webkit-scrollbar-track { background: rgba(255, 255, 255, 0.05); border-radius: 10px; }
        .ai-messages::-webkit-scrollbar-thumb { background: var(--primary); border-radius: 10px; }
        .message { padding: 15px 20px; border-radius: 18px; max-width: 85%; line-height: 1.5; animation: messageSlide 0.3s ease-out; }
        @keyframes messageSlide { from { transform: translateY(10px); opacity: 0; } to { transform: translateY(0); opacity: 1; } }
        .message.user { background: linear-gradient(90deg, var(--primary), var(--secondary)); align-self: flex-end; border-bottom-right-radius: 5px; }
        .message.ai { background-color: rgba(255, 255, 255, 0.1); align-self: flex-start; border-bottom-left-radius: 5px; }
        .ai-input { display: flex; padding: 20px; border-top: 1px solid rgba(255, 255, 255, 0.1); gap: 10px; }
        .ai-input input { flex: 1; padding: 15px 20px; background-color: rgba(255, 255, 255, 0.08); border: 1px solid rgba(255, 255, 255, 0.1); border-radius: 12px; color: var(--light); font-size: 16px; }
        .ai-input input:focus { outline: none; border-color: var(--primary); box-shadow: 0 0 0 2px rgba(0, 198, 255, 0.3); }
        .ai-input button { background: linear-gradient(90deg, var(--primary), var(--secondary)); color: white; border: none; border-radius: 12px; padding: 15px 20px; cursor: pointer; transition: all 0.3s ease; display: flex; align-items: center; justify-content: center; width: 50px; }
        .ai-input button:hover { transform: translateY(-2px); box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2); }
        
        .home-btn { position: fixed; top: 30px; left: 30px; z-index: 100; }
        
        .tip-card { padding: 20px; background: rgba(255, 255, 255, 0.05); border-radius: 16px; margin-bottom: 20px; transition: transform 0.3s ease; border-left: 4px solid var(--primary); }
        .tip-card:hover { transform: translateX(5px); background: rgba(255, 255, 255, 0.08); }
        .tip-card h4 { margin-bottom: 10px; font-size: 18px; display: flex; align-items: center; gap: 10px; }
        .tip-card p { opacity: 0.8; line-height: 1.6; }
        
        .totals { background: rgba(255, 255, 255, 0.05); padding: 20px; border-radius: 16px; margin-top: 20px; }
        .totals p { display: flex; justify-content: space-between; margin: 12px 0; font-size: 18px; font-weight: 600; }
        .totals span { color: var(--success); }
        .totals .tax { color: var(--warning); }
        .totals .grand-total { color: var(--primary); font-size: 22px; border-top: 1px solid rgba(255, 255, 255, 0.1); padding-top: 15px; margin-top: 15px; }
        
        @media (max-width: 1400px) {
            .dashboard-content { grid-template-columns: 1fr; }
            .stats-grid { grid-template-columns: repeat(2, 1fr); }
            .expense-form { grid-template-columns: 1fr; }
        }
        @media (max-width: 1024px) {
            .main-content { grid-template-columns: 1fr; }
            .sidebar { display: none; }
            .ai-chat { width: 350px; height: 500px; }
        }
        @media (max-width: 768px) {
            .container { padding: 0 15px; }
            .stats-grid { grid-template-columns: 1fr; }
            .ai-chat { width: 320px; height: 450px; right: -20px; }
            .home-btn { top: 20px; left: 20px; }
            .header { flex-direction: column; gap: 20px; text-align: center; }
            .card { padding: 20px; }
            .auth-box { padding: 30px; }
        }
    </style>
</head>
<body>
    <div class="particles-container" id="particles-container"></div>

    <div class="auth-container" id="auth-section">
        <div class="auth-box">
            <div class="auth-header">
                <h1><i class="fas fa-chart-pie"></i> TotalCheck AI</h1>
                <p>Your Ultimate Finance Intelligence Platform</p>
            </div>
            
            <div class="auth-tabs">
                <div class="auth-tab active" data-tab="login">Sign In</div>
                <div class="auth-tab" data-tab="register">Create Account</div>
            </div>
            
            <form class="auth-form active" id="login-form">
                <div class="form-group">
                    <label for="login-email">Email</label>
                    <input type="email" id="login-email" class="form-control" placeholder="Enter your email" required>
                </div>
                <div class="form-group">
                    <label for="login-password">Password</label>
                    <input type="password" id="login-password" class="form-control" placeholder="Enter your password" required>
                </div>
                <button type="submit" class="btn btn-full">Sign In</button>
                <div class="error-message" id="login-error">Invalid email or password. Please try again or create an account.</div>
            </form>
            
            <form class="auth-form" id="register-form">
                <div class="form-group">
                    <label for="register-name">Full Name</label>
                    <input type="text" id="register-name" class="form-control" placeholder="Enter your full name" required>
                </div>
                <div class="form-group">
                    <label for="register-email">Email</label>
                    <input type="email" id="register-email" class="form-control" placeholder="Enter your email" required>
                </div>
                <div class="form-group">
                    <label for="register-password">Password</label>
                    <input type="password" id="register-password" class="form-control" placeholder="Create a password" required>
                </div>
                <div class="form-group">
                    <label for="register-confirm">Confirm Password</label>
                    <input type="password" id="register-confirm" class="form-control" placeholder="Confirm your password" required>
                </div>
                <div class="form-group">
                    <label for="currency">Currency</label>
                    <select id="currency" class="form-control" required>
                        <option value="USD">US Dollar ($)</option>
                        <option value="EUR">Euro (€)</option>
                        <option value="GBP">British Pound (£)</option>
                        <option value="AED" selected>UAE Dirham (د.إ)</option>
                        <option value="INR">Indian Rupee (₹)</option>
                        <option value="JPY">Japanese Yen (¥)</option>
                    </select>
                </div>
                <button type="submit" class="btn btn-full">Create Account</button>
                <div class="success-message" id="register-success">Account created successfully! You can now sign in.</div>
            </form>
        </div>
    </div>

    <div class="dashboard container" id="dashboard">
        <div class="header">
            <div class="logo" id="home-btn">
                <i class="fas fa-chart-pie"></i> TotalCheck AI
            </div>
            <div class="current-time" id="current-time"></div>
            <div class="user-info">
                <div class="user-avatar" id="user-avatar">JD</div>
                <div>
                    <div id="user-name">John Doe</div>
                    <div style="font-size: 14px; opacity: 0.7;" id="user-currency">د.إ Dirhams</div>
                </div>
                <button class="btn btn-outline" id="logout-btn" style="width: auto; padding: 12px 25px;">Logout</button>
            </div>
        </div>

        <div class="home-btn">
            <button class="btn" id="go-home-btn" style="width: auto; padding: 15px 25px;">
                <i class="fas fa-home"></i> Home
            </button>
        </div>

        <div class="main-content">
            <div class="sidebar">
                <ul class="nav-links">
                    <li><a href="#" class="active" data-section="dashboard"><i class="fas fa-chart-line"></i> Dashboard</a></li>
                    <li><a href="#" data-section="expenses"><i class="fas fa-wallet"></i> Expenses</a></li>
                    <li><a href="#" data-section="savings"><i class="fas fa-piggy-bank"></i> Savings</a></li>
                    <li><a href="#" data-section="budgets"><i class="fas fa-chart-pie"></i> Budgets</a></li>
                    <li><a href="#" data-section="transactions"><i class="fas fa-receipt"></i> Transactions</a></li>
                    <li><a href="#" data-section="notifications"><i class="fas fa-bell"></i> Notifications</a></li>
                </ul>
            </div>

            <div class="dashboard-content">
                <div class="stats-grid card-full">
                    <div class="stat-card">
                        <div class="stat-value" id="monthly-income">د.إ4,250</div>
                        <div class="stat-label">Monthly Income</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-value" id="monthly-expenses">د.إ2,850</div>
                        <div class="stat-label">Monthly Expenses</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-value" id="monthly-savings">د.إ1,400</div>
                        <div class="stat-label">Monthly Savings</div>
                    </div>
                    <div class="stat-card">
                        <div class="stat-value" id="savings-rate">32.9%</div>
                        <div class="stat-label">Savings Rate</div>
                    </div>
                </div>

                <div class="card card-full">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-chart-line"></i> Financial Overview</div>
                        <div class="card-actions">
                            <button class="btn btn-outline" style="width: auto; padding: 10px 20px;">
                                <i class="fas fa-download"></i> Export
                            </button>
                        </div>
                    </div>
                    <div class="chart-container">
                        <canvas id="financeChart"></canvas>
                    </div>
                </div>

                <div class="card">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-chart-pie"></i> Expense Breakdown</div>
                    </div>
                    <div class="chart-container">
                        <canvas id="expenseChart"></canvas>
                    </div>
                </div>

                <div class="card">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-lightbulb"></i> Today's AI Tips</div>
                    </div>
                    <div id="financial-tips">
                        <div class="tip-card">
                            <h4><i class="fas fa-shield-alt"></i> Emergency Fund</h4>
                            <p>You've saved د.إ1,400 this month. Consider allocating 20% to your emergency fund for financial security.</p>
                        </div>
                        <div class="tip-card">
                            <h4><i class="fas fa-chart-line"></i> Investment Opportunity</h4>
                            <p>With your current savings rate, you could invest د.إ500 monthly for long-term wealth building.</p>
                        </div>
                        <div class="tip-card">
                            <h4><i class="fas fa-shopping-cart"></i> Spending Alert</h4>
                            <p>Your shopping expenses increased by 15% this month. Consider setting a budget for discretionary spending.</p>
                        </div>
                    </div>
                </div>

                <div class="card card-full" id="expenses-section" style="display: none;">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-wallet"></i> Expense Tracking</div>
                        <button class="btn" style="width: auto; padding: 12px 25px;" id="add-expense-btn">
                            <i class="fas fa-plus"></i> Add Expense
                        </button>
                    </div>
                    <div class="expense-form" id="expense-form">
                        <div class="form-group">
                            <label for="expense-name">Expense Name</label>
                            <input type="text" id="expense-name" class="form-control" placeholder="Enter expense name">
                        </div>
                        <div class="form-group">
                            <label for="expense-amount">Amount</label>
                            <input type="number" id="expense-amount" class="form-control" placeholder="Enter amount">
                        </div>
                        <div class="form-group">
                            <label for="expense-category">Category</label>
                            <select id="expense-category" class="form-control">
                                <option value="food">Food & Dining</option>
                                <option value="transport">Transportation</option>
                                <option value="housing">Housing</option>
                                <option value="utilities">Utilities</option>
                                <option value="entertainment">Entertainment</option>
                                <option value="shopping">Shopping</option>
                                <option value="healthcare">Healthcare</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="expense-date">Date</label>
                            <input type="date" id="expense-date" class="form-control">
                        </div>
                        <div class="form-group">
                            <button type="button" class="btn" id="save-expense">Save Expense</button>
                        </div>
                        <div class="form-group">
                            <button type="button" class="btn btn-outline" id="cancel-expense">Cancel</button>
                        </div>
                    </div>
                    <div class="expense-list" id="expense-list"></div>
                    <div class="totals">
                        <p>Subtotal: <span id="subtotal">0.00</span></p>
                        <p>Tax 5%: <span class="tax" id="tax">0.00</span></p>
                        <p class="grand-total">Grand Total: <span id="grandTotal">0.00</span></p>
                    </div>
                </div>

                <div class="card card-full" id="savings-section" style="display: none;">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-piggy-bank"></i> Savings Goals</div>
                        <button class="btn" style="width: auto; padding: 12px 25px;" id="add-savings-btn">
                            <i class="fas fa-plus"></i> Add Goal
                        </button>
                    </div>
                    <div class="expense-form" id="savings-form" style="display: none;">
                        <div class="form-group">
                            <label for="savings-name">Goal Name</label>
                            <input type="text" id="savings-name" class="form-control" placeholder="Enter goal name">
                        </div>
                        <div class="form-group">
                            <label for="savings-target">Target Amount</label>
                            <input type="number" id="savings-target" class="form-control" placeholder="Enter target amount">
                        </div>
                        <div class="form-group">
                            <label for="savings-current">Current Amount</label>
                            <input type="number" id="savings-current" class="form-control" placeholder="Enter current amount">
                        </div>
                        <div class="form-group">
                            <label for="savings-deadline">Target Date</label>
                            <input type="date" id="savings-deadline" class="form-control">
                        </div>
                        <div class="form-group">
                            <button type="button" class="btn" id="save-savings">Save Goal</button>
                        </div>
                        <div class="form-group">
                            <button type="button" class="btn btn-outline" id="cancel-savings">Cancel</button>
                        </div>
                    </div>
                    <div class="expense-list" id="savings-list"></div>
                </div>

                <div class="card card-full" id="budgets-section" style="display: none;">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-chart-pie"></i> Budgets</div>
                        <button class="btn" style="width: auto; padding: 12px 25px;" id="add-budget-btn">
                            <i class="fas fa-plus"></i> Add Budget
                        </button>
                    </div>
                    <div class="expense-form" id="budget-form" style="display: none;">
                        <div class="form-group">
                            <label for="budget-category">Category</label>
                            <select id="budget-category" class="form-control">
                                <option value="food">Food & Dining</option>
                                <option value="transport">Transportation</option>
                                <option value="housing">Housing</option>
                                <option value="utilities">Utilities</option>
                                <option value="entertainment">Entertainment</option>
                                <option value="shopping">Shopping</option>
                                <option value="healthcare">Healthcare</option>
                                <option value="other">Other</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <label for="budget-amount">Budget Amount</label>
                            <input type="number" id="budget-amount" class="form-control" placeholder="Enter budget amount">
                        </div>
                        <div class="form-group">
                            <label for="budget-period">Period</label>
                            <select id="budget-period" class="form-control">
                                <option value="monthly">Monthly</option>
                                <option value="weekly">Weekly</option>
                                <option value="yearly">Yearly</option>
                            </select>
                        </div>
                        <div class="form-group">
                            <button type="button" class="btn" id="save-budget">Save Budget</button>
                        </div>
                        <div class="form-group">
                            <button type="button" class="btn btn-outline" id="cancel-budget">Cancel</button>
                        </div>
                    </div>
                    <div class="expense-list" id="budgets-list"></div>
                </div>

                <div class="card card-full" id="transactions-section" style="display: none;">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-receipt"></i> Recent Transactions</div>
                    </div>
                    <div class="expense-list" id="transactions-list">
                        <div class="expense-item">
                            <div class="expense-info">
                                <h4>Salary Deposit</h4>
                                <div class="expense-meta">
                                    <i class="fas fa-arrow-down" style="color: var(--success);"></i> Income • June 15, 2023
                                </div>
                            </div>
                            <div class="expense-amount" style="color: var(--success);">+د.إ4,250</div>
                        </div>
                        <div class="expense-item">
                            <div class="expense-info">
                                <h4>Groceries</h4>
                                <div class="expense-meta">
                                    <i class="fas fa-utensils"></i> Food & Dining • June 14, 2023
                                </div>
                            </div>
                            <div class="expense-amount" style="color: var(--danger);">-د.إ120</div>
                        </div>
                    </div>
                </div>

                <div class="card card-full" id="notifications-section" style="display: none;">
                    <div class="card-header">
                        <div class="card-title"><i class="fas fa-bell"></i> Notifications</div>
                    </div>
                    <div class="expense-list" id="notifications-list">
                        <div class="expense-item">
                            <div class="expense-info">
                                <h4>Budget Alert</h4>
                                <div class="expense-meta">
                                    You've exceeded your dining budget by 15% this month
                                </div>
                            </div>
                            <div class="expense-amount"><i class="fas fa-exclamation-triangle" style="color: var(--warning);"></i></div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div class="ai-assistant">
        <div class="ai-chat" id="ai-chat">
            <div class="ai-header">
                <i class="fas fa-robot"></i> TotalCheck AI Assistant
            </div>
            <div class="ai-messages" id="ai-messages">
                <div class="message ai">
                    Hello! I'm your TotalCheck AI assistant. I can help you analyze your finances, provide savings tips, and answer money-related questions. How can I assist you today?
                </div>
            </div>
            <div class="ai-input">
                <input type="text" id="ai-input" placeholder="Ask me about your finances...">
                <button id="ai-send"><i class="fas fa-paper-plane"></i></button>
            </div>
        </div>
        <div class="ai-toggle" id="ai-toggle">
            <i class="fas fa-robot"></i>
        </div>
    </div>

    <script>
        let userAccounts = JSON.parse(localStorage.getItem('totalCheckAccounts')) || [];
        let currentUser = null;
        let currentCurrency = 'AED';
        const currencySymbols = {'USD':'$','EUR':'€','GBP':'£','AED':'د.إ','INR':'₹','JPY':'¥'};
        let expenses = JSON.parse(localStorage.getItem('totalCheckExpenses')) || [];
        let savingsGoals = JSON.parse(localStorage.getItem('totalCheckSavings')) || [];
        let budgets = JSON.parse(localStorage.getItem('totalCheckBudgets')) || [];

        function createParticles() {
            const container = document.getElementById('particles-container');
            for (let i = 0; i < 50; i++) {
                const particle = document.createElement('div');
                particle.classList.add('particle');
                const size = Math.random() * 4 + 2;
                particle.style.width = `${size}px`;
                particle.style.height = `${size}px`;
                particle.style.left = `${Math.random() * 100}vw`;
                particle.style.top = `${Math.random() * 100}vh`;
                particle.style.animationDelay = `${Math.random() * 15}s`;
                container.appendChild(particle);
            }
        }

        function updateTime() {
            const now = new Date();
            const options = { weekday: 'long', year: 'numeric', month: 'long', day: 'numeric', hour: '2-digit', minute: '2-digit', second: '2-digit' };
            document.getElementById('current-time').textContent = now.toLocaleDateString('en-US', options);
        }

        function showDashboard() {
            document.querySelectorAll('.nav-links a').forEach(a => a.classList.remove('active'));
            document.querySelector('.nav-links a[data-section="dashboard"]').classList.add('active');
            document.querySelectorAll('.card-full').forEach(card => card.style.display = 'none');
            document.querySelectorAll('.card').forEach(card => {
                if (!card.id || card.id === 'expenses-section') card.style.display = 'none';
                else if (!card.id.includes('section')) card.style.display = 'block';
            });
            document.querySelector('.stats-grid').style.display = 'grid';
        }

        document.querySelectorAll('.auth-tab').forEach(tab => {
            tab.addEventListener('click', () => {
                document.querySelectorAll('.auth-tab').forEach(t => t.classList.remove('active'));
                document.querySelectorAll('.auth-form').forEach(f => f.classList.remove('active'));
                tab.classList.add('active');
                document.getElementById(`${tab.dataset.tab}-form`).classList.add('active');
                document.getElementById('login-error').style.display = 'none';
                document.getElementById('register-success').style.display = 'none';
            });
        });

        document.getElementById('login-form').addEventListener('submit', function(e) {
            e.preventDefault();
            const email = document.getElementById('login-email').value;
            const password = document.getElementById('login-password').value;
            const user = userAccounts.find(acc => acc.email === email && acc.password === password);
            if (user) {
                currentUser = user;
                currentCurrency = user.currency || 'AED';
                document.getElementById('auth-section').style.display = 'none';
                document.getElementById('dashboard').style.display = 'block';
                updateUserDashboard();
                initializeSampleData();
                createFinanceChart();
                createExpenseChart();
                setInterval(updateTime, 1000);
                updateTime();
            } else {
                document.getElementById('login-error').style.display = 'block';
            }
        });

        document.getElementById('register-form').addEventListener('submit', function(e) {
            e.preventDefault();
            const name = document.getElementById('register-name').value;
            const email = document.getElementById('register-email').value;
            const password = document.getElementById('register-password').value;
            const confirmPassword = document.getElementById('register-confirm').value;
            const currency = document.getElementById('currency').value;
            if (password !== confirmPassword) {
                alert('Passwords do not match!');
                return;
            }
            if (userAccounts.find(acc => acc.email === email)) {
                alert('An account with this email already exists!');
                return;
            }
            const newUser = { name, email, password, currency, createdAt: new Date().toISOString() };
            userAccounts.push(newUser);
            localStorage.setItem('totalCheckAccounts', JSON.stringify(userAccounts));
            document.getElementById('register-success').style.display = 'block';
            document.getElementById('register-form').reset();
            setTimeout(() => document.querySelector('.auth-tab[data-tab="login"]').click(), 2000);
        });

        function updateUserDashboard() {
            if (!currentUser) return;
            document.getElementById('user-name').textContent = currentUser.name;
            document.getElementById('user-currency').textContent = `${currencySymbols[currentCurrency]} ${currentCurrency}`;
            const initials = currentUser.name.split(' ').map(n => n[0]).join('').toUpperCase();
            document.getElementById('user-avatar').textContent = initials;
            updateCurrencyDisplay();
        }

        function updateCurrencyDisplay() {
            const symbol = currencySymbols[currentCurrency] || '$';
            document.getElementById('monthly-income').textContent = `${symbol}4,250`;
            document.getElementById('monthly-expenses').textContent = `${symbol}2,850`;
            document.getElementById('monthly-savings').textContent = `${symbol}1,400`;
            document.querySelectorAll('.expense-amount').forEach(el => {
                if (el.textContent.includes('$') || el.textContent.includes('€') || el.textContent.includes('£') || el.textContent.includes('د.إ')) {
                    el.textContent = el.textContent.replace(/\$|€|£|د\.إ/g, symbol);
                }
            });
        }

        document.getElementById('logout-btn').addEventListener('click', function() {
            currentUser = null;
            document.getElementById('dashboard').style.display = 'none';
            document.getElementById('auth-section').style.display = 'flex';
            document.getElementById('login-form').reset();
            document.getElementById('login-error').style.display = 'none';
        });

        document.getElementById('home-btn').addEventListener('click', showDashboard);
        document.getElementById('go-home-btn').addEventListener('click', showDashboard);

        document.querySelectorAll('.nav-links a').forEach(link => {
            link.addEventListener('click', function(e) {
                e.preventDefault();
                document.querySelectorAll('.nav-links a').forEach(a => a.classList.remove('active'));
                this.classList.add('active');
                document.querySelectorAll('.card-full').forEach(card => card.style.display = 'none');
                document.querySelector('.stats-grid').style.display = 'none';
                const section = this.getAttribute('data-section');
                if (section === 'dashboard') showDashboard();
                else document.getElementById(`${section}-section`).style.display = 'block';
            });
        });

        if (expenses.length === 0) {
            expenses = [
                { id: 1, name: "Groceries", amount: 120, category: "food", date: "2023-06-15" },
                { id: 2, name: "Gas", amount: 60, category: "transport", date: "2023-06-14" },
                { id: 3, name: "Netflix Subscription", amount: 15, category: "entertainment", date: "2023-06-10" },
                { id: 4, name: "Electricity Bill", amount: 85, category: "utilities", date: "2023-06-05" }
            ];
            localStorage.setItem('totalCheckExpenses', JSON.stringify(expenses));
        }

        document.getElementById('add-expense-btn').addEventListener('click', function() {
            document.getElementById('expense-form').style.display = 'grid';
        });

        document.getElementById('cancel-expense').addEventListener('click', function() {
            document.getElementById('expense-form').style.display = 'none';
            clearExpenseForm();
        });

        document.getElementById('save-expense').addEventListener('click', function() {
            const name = document.getElementById('expense-name').value;
            const amount = parseFloat(document.getElementById('expense-amount').value);
            const category = document.getElementById('expense-category').value;
            const date = document.getElementById('expense-date').value;
            if (name && amount && category && date) {
                const newExpense = { id: expenses.length > 0 ? Math.max(...expenses.map(e => e.id)) + 1 : 1, name, amount, category, date };
                expenses.push(newExpense);
                localStorage.setItem('totalCheckExpenses', JSON.stringify(expenses));
                renderExpenseList();
                clearExpenseForm();
                document.getElementById('expense-form').style.display = 'none';
                createFinanceChart();
                createExpenseChart();
                alert('Expense added successfully!');
            } else alert('Please fill in all fields');
        });

        function renderExpenseList() {
            const expenseList = document.getElementById('expense-list');
            expenseList.innerHTML = '';
            if (expenses.length === 0) {
                expenseList.innerHTML = '<div style="text-align: center; padding: 20px; opacity: 0.7;">No expenses recorded yet. Add your first expense!</div>';
                return;
            }
            const sortedExpenses = [...expenses].sort((a, b) => new Date(b.date) - new Date(a.date));
            const categoryIcons = {'food':'fas fa-utensils','transport':'fas fa-car','housing':'fas fa-home','utilities':'fas fa-bolt','entertainment':'fas fa-film','shopping':'fas fa-shopping-bag','healthcare':'fas fa-heartbeat','other':'fas fa-question'};
            const symbol = currencySymbols[currentCurrency] || '$';
            sortedExpenses.forEach(expense => {
                const expenseItem = document.createElement('div');
                expenseItem.className = 'expense-item';
                const dateObj = new Date(expense.date);
                const formattedDate = dateObj.toLocaleDateString('en-US', { month: 'short', day: 'numeric' });
                expenseItem.innerHTML = `
                    <div class="expense-info">
                        <h4>${expense.name}</h4>
                        <div class="expense-meta">
                            <i class="${categoryIcons[expense.category]}"></i> ${expense.category.charAt(0).toUpperCase() + expense.category.slice(1)} • ${formattedDate}
                        </div>
                    </div>
                    <div class="expense-amount">${symbol}${expense.amount.toFixed(2)}</div>
                    <div class="expense-actions">
                        <button class="action-btn delete" data-id="${expense.id}"><i class="fas fa-trash"></i></button>
                    </div>
                `;
                expenseList.appendChild(expenseItem);
            });
            updateTotals();
            document.querySelectorAll('.action-btn.delete').forEach(btn => {
                btn.addEventListener('click', function() {
                    const id = parseInt(this.getAttribute('data-id'));
                    deleteExpense(id);
                });
            });
        }

        function updateTotals() {
            let subtotal = 0;
            expenses.forEach(expense => subtotal += expense.amount);
            const tax = subtotal * 0.05;
            const grandTotal = subtotal + tax;
            const symbol = currencySymbols[currentCurrency] || '$';
            document.getElementById('subtotal').textContent = `${symbol}${subtotal.toFixed(2)}`;
            document.getElementById('tax').textContent = `${symbol}${tax.toFixed(2)}`;
            document.getElementById('grandTotal').textContent = `${symbol}${grandTotal.toFixed(2)}`;
        }

        function deleteExpense(id) {
            if (confirm('Are you sure you want to delete this expense?')) {
                expenses = expenses.filter(expense => expense.id !== id);
                localStorage.setItem('totalCheckExpenses', JSON.stringify(expenses));
                renderExpenseList();
                createFinanceChart();
                createExpenseChart();
            }
        }

        function clearExpenseForm() {
            document.getElementById('expense-name').value = '';
            document.getElementById('expense-amount').value = '';
            document.getElementById('expense-category').value = 'food';
            document.getElementById('expense-date').value = '';
        }

        if (savingsGoals.length === 0) {
            savingsGoals = [
                { id: 1, name: "Emergency Fund", target: 10000, current: 4500, deadline: "2024-12-31" },
                { id: 2, name: "Vacation Fund", target: 5000, current: 3000, deadline: "2023-12-31" },
                { id: 3, name: "Investment Account", target: 20000, current: 5000, deadline: "2025-12-31" }
            ];
            localStorage.setItem('totalCheckSavings', JSON.stringify(savingsGoals));
        }

        document.getElementById('add-savings-btn').addEventListener('click', function() {
            document.getElementById('savings-form').style.display = 'grid';
        });

        document.getElementById('cancel-savings').addEventListener('click', function() {
            document.getElementById('savings-form').style.display = 'none';
            clearSavingsForm();
        });

        document.getElementById('save-savings').addEventListener('click', function() {
            const name = document.getElementById('savings-name').value;
            const target = parseFloat(document.getElementById('savings-target').value);
            const current = parseFloat(document.getElementById('savings-current').value);
            const deadline = document.getElementById('savings-deadline').value;
            if (name && target && current >= 0 && deadline) {
                const newGoal = { id: savingsGoals.length > 0 ? Math.max(...savingsGoals.map(g => g.id)) + 1 : 1, name, target, current, deadline };
                savingsGoals.push(newGoal);
                localStorage.setItem('totalCheckSavings', JSON.stringify(savingsGoals));
                renderSavingsList();
                clearSavingsForm();
                document.getElementById('savings-form').style.display = 'none';
                alert('Savings goal added successfully!');
            } else alert('Please fill in all fields');
        });

        function renderSavingsList() {
            const savingsList = document.getElementById('savings-list');
            savingsList.innerHTML = '';
            if (savingsGoals.length === 0) {
                savingsList.innerHTML = '<div style="text-align: center; padding: 20px; opacity: 0.7;">No savings goals yet. Add your first goal!</div>';
                return;
            }
            const symbol = currencySymbols[currentCurrency] || '$';
            savingsGoals.forEach(goal => {
                const progress = (goal.current / goal.target) * 100;
                const goalItem = document.createElement('div');
                goalItem.className = 'expense-item';
                const deadlineObj = new Date(goal.deadline);
                const formattedDeadline = deadlineObj.toLocaleDateString('en-US', { month: 'short', day: 'numeric', year: 'numeric' });
                goalItem.innerHTML = `
                    <div class="expense-info">
                        <h4>${goal.name}</h4>
                        <div class="expense-meta">
                            <i class="fas fa-piggy-bank"></i> Target: ${symbol}${goal.target.toLocaleString()} • Progress: ${progress.toFixed(1)}%
                        </div>
                        <div style="margin-top: 10px; background: rgba(255, 255, 255, 0.1); border-radius: 10px; height: 8px; overflow: hidden;">
                            <div style="height: 100%; width: ${progress}%; background: linear-gradient(90deg, var(--primary), var(--accent));"></div>
                        </div>
                    </div>
                    <div class="expense-amount">${symbol}${goal.current.toLocaleString()}</div>
                    <div class="expense-actions">
                        <button class="action-btn delete" data-id="${goal.id}"><i class="fas fa-trash"></i></button>
                    </div>
                `;
                savingsList.appendChild(goalItem);
            });
            document.querySelectorAll('#savings-list .action-btn.delete').forEach(btn => {
                btn.addEventListener('click', function() {
                    const id = parseInt(this.getAttribute('data-id'));
                    deleteSavingsGoal(id);
                });
            });
        }

        function deleteSavingsGoal(id) {
            if (confirm('Are you sure you want to delete this savings goal?')) {
                savingsGoals = savingsGoals.filter(goal => goal.id !== id);
                localStorage.setItem('totalCheckSavings', JSON.stringify(savingsGoals));
                renderSavingsList();
            }
        }

        function clearSavingsForm() {
            document.getElementById('savings-name').value = '';
            document.getElementById('savings-target').value = '';
            document.getElementById('savings-current').value = '';
            document.getElementById('savings-deadline').value = '';
        }

        if (budgets.length === 0) {
            budgets = [
                { id: 1, category: "food", amount: 500, period: "monthly" },
                { id: 2, category: "transport", amount: 200, period: "monthly" },
                { id: 3, category: "utilities", amount: 300, period: "monthly" },
                { id: 4, category: "entertainment", amount: 150, period: "monthly" }
            ];
            localStorage.setItem('totalCheckBudgets', JSON.stringify(budgets));
        }

        document.getElementById('add-budget-btn').addEventListener('click', function() {
            document.getElementById('budget-form').style.display = 'grid';
        });

        document.getElementById('cancel-budget').addEventListener('click', function() {
            document.getElementById('budget-form').style.display = 'none';
            clearBudgetForm();
        });

        document.getElementById('save-budget').addEventListener('click', function() {
            const category = document.getElementById('budget-category').value;
            const amount = parseFloat(document.getElementById('budget-amount').value);
            const period = document.getElementById('budget-period').value;
            if (category && amount && period) {
                const existingBudget = budgets.find(b => b.category === category && b.period === period);
                if (existingBudget) existingBudget.amount = amount;
                else {
                    const newBudget = { id: budgets.length > 0 ? Math.max(...budgets.map(b => b.id)) + 1 : 1, category, amount, period };
                    budgets.push(newBudget);
                }
                localStorage.setItem('totalCheckBudgets', JSON.stringify(budgets));
                renderBudgetsList();
                clearBudgetForm();
                document.getElementById('budget-form').style.display = 'none';
                alert('Budget saved successfully!');
            } else alert('Please fill in all fields');
        });

        function renderBudgetsList() {
            const budgetsList = document.getElementById('budgets-list');
            budgetsList.innerHTML = '';
            if (budgets.length === 0) {
                budgetsList.innerHTML = '<div style="text-align: center; padding: 20px; opacity: 0.7;">No budgets set yet. Add your first budget!</div>';
                return;
            }
            const symbol = currencySymbols[currentCurrency] || '$';
            const categoryIcons = {'food':'fas fa-utensils','transport':'fas fa-car','housing':'fas fa-home','utilities':'fas fa-bolt','entertainment':'fas fa-film','shopping':'fas fa-shopping-bag','healthcare':'fas fa-heartbeat','other':'fas fa-question'};
            budgets.forEach(budget => {
                const categoryExpenses = expenses.filter(e => e.category === budget.category);
                const totalSpent = categoryExpenses.reduce((sum, expense) => sum + expense.amount, 0);
                const percentage = (totalSpent / budget.amount) * 100;
                const budgetItem = document.createElement('div');
                budgetItem.className = 'expense-item';
                budgetItem.innerHTML = `
                    <div class="expense-info">
                        <h4>${budget.category.charAt(0).toUpperCase() + budget.category.slice(1)}</h4>
                        <div class="expense-meta">
                            <i class="${categoryIcons[budget.category]}"></i> ${budget.period} Budget • Spent: ${symbol}${totalSpent.toFixed(2)} of ${symbol}${budget.amount.toFixed(2)}
                        </div>
                        <div style="margin-top: 10px; background: rgba(255, 255, 255, 0.1); border-radius: 10px; height: 8px; overflow: hidden;">
                            <div style="height: 100%; width: ${Math.min(percentage, 100)}%; background: ${percentage > 100 ? 'var(--danger)' : 'var(--success)'};"></div>
                        </div>
                    </div>
                    <div class="expense-amount" style="color: ${percentage > 100 ? 'var(--danger)' : 'var(--success)'};">${percentage.toFixed(1)}%</div>
                    <div class="expense-actions">
                        <button class="action-btn delete" data-id="${budget.id}"><i class="fas fa-trash"></i></button>
                    </div>
                `;
                budgetsList.appendChild(budgetItem);
            });
            document.querySelectorAll('#budgets-list .action-btn.delete').forEach(btn => {
                btn.addEventListener('click', function() {
                    const id = parseInt(this.getAttribute('data-id'));
                    deleteBudget(id);
                });
            });
        }

        function deleteBudget(id) {
            if (confirm('Are you sure you want to delete this budget?')) {
                budgets = budgets.filter(budget => budget.id !== id);
                localStorage.setItem('totalCheckBudgets', JSON.stringify(budgets));
                renderBudgetsList();
            }
        }

        function clearBudgetForm() {
            document.getElementById('budget-category').value = 'food';
            document.getElementById('budget-amount').value = '';
            document.getElementById('budget-period').value = 'monthly';
        }

        function createFinanceChart() {
            const ctx = document.getElementById('financeChart').getContext('2d');
            const monthlyData = calculateMonthlyTotals();
            if (window.financeChart instanceof Chart) window.financeChart.destroy();
            const symbol = currencySymbols[currentCurrency] || '$';
            window.financeChart = new Chart(ctx, {
                type: 'line',
                data: {
                    labels: monthlyData.months,
                    datasets: [{
                        label: 'Income',
                        data: monthlyData.income,
                        borderColor: '#00c6ff',
                        backgroundColor: 'rgba(0, 198, 255, 0.1)',
                        borderWidth: 3,
                        fill: true,
                        tension: 0.4
                    }, {
                        label: 'Expenses',
                        data: monthlyData.expenses,
                        borderColor: '#ff0080',
                        backgroundColor: 'rgba(255, 0, 128, 0.1)',
                        borderWidth: 3,
                        fill: true,
                        tension: 0.4
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { legend: { position: 'top', labels: { color: '#f8fafc', font: { size: 14 } } } },
                    scales: {
                        y: { beginAtZero: true, grid: { color: 'rgba(255, 255, 255, 0.1)' }, ticks: { color: '#f8fafc', callback: function(value) { return symbol + value; } } },
                        x: { grid: { color: 'rgba(255, 255, 255, 0.1)' }, ticks: { color: '#f8fafc' } }
                    }
                }
            });
        }

        function createExpenseChart() {
            const ctx = document.getElementById('expenseChart').getContext('2d');
            const categoryData = calculateCategoryTotals();
            if (window.expenseChart instanceof Chart) window.expenseChart.destroy();
            window.expenseChart = new Chart(ctx, {
                type: 'doughnut',
                data: {
                    labels: categoryData.categories,
                    datasets: [{
                        data: categoryData.amounts,
                        backgroundColor: ['#00c6ff', '#ff0080', '#00ff9d', '#ffbd00', '#7a00ff', '#ff2e63', '#2a9d8f', '#64748b'],
                        borderWidth: 0,
                        hoverOffset: 15
                    }]
                },
                options: {
                    responsive: true,
                    maintainAspectRatio: false,
                    plugins: { legend: { position: 'right', labels: { color: '#f8fafc', boxWidth: 15, padding: 15, font: { size: 12 } } } }
                }
            });
        }

        function calculateMonthlyTotals() {
            const months = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun'];
            const income = [4200, 4300, 4250, 4400, 4350, 4250];
            const expenses = [3100, 2950, 3200, 2800, 3050, 2850];
            return { months, income, expenses };
        }

        function calculateCategoryTotals() {
            const categories = {};
            expenses.forEach(expense => {
                if (categories[expense.category]) categories[expense.category] += expense.amount;
                else categories[expense.category] = expense.amount;
            });
            return { categories: Object.keys(categories), amounts: Object.values(categories) };
        }

        document.getElementById('ai-toggle').addEventListener('click', function() {
            document.getElementById('ai-chat').classList.toggle('active');
        });

        document.getElementById('ai-send').addEventListener('click', sendMessage);
        document.getElementById('ai-input').addEventListener('keypress', function(e) {
            if (e.key === 'Enter') sendMessage();
        });

        function sendMessage() {
            const input = document.getElementById('ai-input');
            const message = input.value.trim();
            if (message) {
                const userMessage = document.createElement('div');
                userMessage.className = 'message user';
                userMessage.textContent = message;
                document.getElementById('ai-messages').appendChild(userMessage);
                input.value = '';
                setTimeout(() => {
                    const aiMessage = document.createElement('div');
                    aiMessage.className = 'message ai';
                    if (message.toLowerCase().includes('budget') || message.toLowerCase().includes('save')) {
                        aiMessage.textContent = `Based on your spending patterns, I recommend allocating 50% to needs, 30% to wants, and 20% to savings. Your current savings rate is excellent at 32.9%!`;
                    } else if (message.toLowerCase().includes('expense') || message.toLowerCase().includes('spending')) {
                        aiMessage.textContent = `Your largest expense category is Food & Dining. Consider meal planning to reduce costs. You're spending ${currencySymbols[currentCurrency]}120 monthly on groceries which is reasonable.`;
                    } else if (message.toLowerCase().includes('investment') || message.toLowerCase().includes('invest')) {
                        aiMessage.textContent = `With your savings rate, you could invest ${currencySymbols[currentCurrency]}500 monthly. Consider low-cost index funds for long-term growth. Your emergency fund should cover 3-6 months of expenses.`;
                    } else if (message.toLowerCase().includes('debt') || message.toLowerCase().includes('loan')) {
                        aiMessage.textContent = 'If you have high-interest debt, prioritize paying it off before investing. The avalanche method (highest interest first) can save you the most money.';
                    } else if (message.toLowerCase().includes('currency') || message.toLowerCase().includes('dirham')) {
                        aiMessage.textContent = `Your account is set to use ${currentCurrency} (${currencySymbols[currentCurrency]}). All financial calculations are displayed in your selected currency.`;
                    } else aiMessage.textContent = 'I can help you with budgeting, saving strategies, expense tracking, and investment advice. What specific financial topic would you like to discuss?';
                    document.getElementById('ai-messages').appendChild(aiMessage);
                    document.getElementById('ai-messages').scrollTop = document.getElementById('ai-messages').scrollHeight;
                }, 1000);
                document.getElementById('ai-messages').scrollTop = document.getElementById('ai-messages').scrollHeight;
            }
        }

        function initializeSampleData() {
            const today = new Date().toISOString().split('T')[0];
            document.getElementById('expense-date').value = today;
            const threeMonthsFromNow = new Date();
            threeMonthsFromNow.setMonth(threeMonthsFromNow.getMonth() + 3);
            document.getElementById('savings-deadline').value = threeMonthsFromNow.toISOString().split('T')[0];
            renderExpenseList();
            renderSavingsList();
            renderBudgetsList();
        }

        window.addEventListener('load', function() {
            createParticles();
            document.getElementById('currency').value = 'AED';
            const isLoggedIn = false;
            if (isLoggedIn && userAccounts.length > 0) {
                currentUser = userAccounts[0];
                currentCurrency = currentUser.currency || 'AED';
                document.getElementById('auth-section').style.display = 'none';
                document.getElementById('dashboard').style.display = 'block';
                updateUserDashboard();
                initializeSampleData();
                createFinanceChart();
                createExpenseChart();
                setInterval(updateTime, 1000);
                updateTime();
            }
        });
    </script>
</body>
</html>
