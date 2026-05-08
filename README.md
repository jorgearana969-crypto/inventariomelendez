/* Reset and Base Styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Roboto', sans-serif;
    background-color: #f5f7fa;
    color: #333;
    line-height: 1.6;
}

.container {
    max-width: 1200px;
    margin: 0 auto;
    padding: 0 20px;
}

/* Header Styles */
.header {
    background-color: #1e88e5;
    color: white;
    padding: 20px 0;
    text-align: center;
    box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
    margin-bottom: 30px;
}

.header-subtitle {
    font-size: 1.1rem;
    margin-bottom: 10px;
    font-weight: 400;
}

.user-controls {
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 15px;
    font-size: 0.9rem;
}

.user-email {
    font-weight: 500;
}

.logout-link {
    color: white;
    text-decoration: none;
    display: flex;
    align-items: center;
    gap: 5px;
    opacity: 0.9;
}

.logout-link:hover {
    opacity: 1;
    text-decoration: underline;
}

/* Section Title */
.section-title {
    font-size: 1.8rem;
    margin-bottom: 25px;
    font-weight: 700;
    color: #333;
}

/* Dashboard Stats */
.stats-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 20px;
    margin-bottom: 30px;
}

.stat-card {
    background: white;
    padding: 20px;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    border: 1px solid #eee;
}

.stat-label {
    color: #888;
    font-size: 0.85rem;
    display: block;
    margin-bottom: 8px;
}

.stat-value {
    font-size: 1.6rem;
    font-weight: 500;
    color: #1e88e5;
}

.charts-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 15px;
    margin-bottom: 30px;
    max-width: 1000px;
    margin-left: auto;
    margin-right: auto;
}

.chart-card {
    background: white;
    padding: 15px;
    border-radius: 8px;
    box-shadow: 0 2px 8px rgba(0,0,0,0.05);
    border: 1px solid #eee;
    height: 220px;
    display: flex;
    flex-direction: column;
}

.chart-card h3 {
    font-size: 0.9rem;
    margin-bottom: 10px;
    color: #444;
    text-align: center;
    font-weight: 600;
}

.chart-card canvas {
    flex: 1;
    max-height: 160px !important;
}

/* Controls Container */
.controls-container {
    background: white;
    padding: 20px;
    border-radius: 8px 8px 0 0;
    border: 1px solid #eee;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 20px;
}

#search-input {
    flex: 1;
    padding: 10px 15px;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 0.95rem;
}

.filters-wrapper {
    display: flex;
    align-items: center;
    gap: 15px;
}

.filter-group {
    display: flex;
    flex-direction: column;
    gap: 2px;
}

.filter-group label {
    font-size: 0.75rem;
    color: #888;
}

.filter-group select {
    padding: 8px 10px;
    border: 1px solid #ddd;
    border-radius: 4px;
    font-size: 0.9rem;
    background: white;
}

.btn-primary {
    background-color: #1e88e5;
    color: white;
    padding: 10px 20px;
    border-radius: 4px;
    font-weight: 500;
}

.btn-primary:hover {
    background-color: #1976d2;
}

/* Table Styles */
.table-responsive {
    background: white;
    border-radius: 0 0 8px 8px;
    border: 1px solid #eee;
    border-top: none;
    overflow-x: auto;
}

.inventory-table {
    width: 100%;
    border-collapse: collapse;
    min-width: 800px;
}

.inventory-table th {
    background-color: #f8f9fa;
    padding: 15px;
    text-align: left;
    font-weight: 600;
    color: #444;
    border-bottom: 2px solid #eee;
}

.inventory-table td {
    padding: 15px;
    border-bottom: 1px solid #eee;
    vertical-align: middle;
}

.inventory-table tr:hover {
    background-color: #fcfcfc;
}

/* Tags */
.tag {
    padding: 4px 10px;
    border-radius: 20px;
    font-size: 0.8rem;
    font-weight: 500;
}

.tag-pvc {
    border: 1px solid #2196f3;
    color: #2196f3;
}

.tag-vidrio {
    border: 1px solid #9c27b0;
    color: #9c27b0;
}

.status-badge {
    padding: 5px 12px;
    border-radius: 20px;
    font-size: 0.8rem;
    color: white;
}

.status-disponible {
    background-color: #2e7d32;
}

.status-bajo-stock {
    background-color: #ef6c00;
}

.status-agotado {
    background-color: #c62828;
}

/* Actions */
.action-btn {
    background: none;
    border: none;
    cursor: pointer;
    font-size: 1.1rem;
    margin: 0 5px;
    transition: color 0.3s;
}

.edit-btn {
    color: #1976d2;
}

.delete-btn {
    color: #d32f2f;
}

/* Modal Styles */
.modal {
    display: none;
    position: fixed;
    z-index: 2000;
    left: 0;
    top: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0,0,0,0.6);
    backdrop-filter: blur(3px);
    overflow-y: auto;
    padding: 20px 0;
}

.modal-content {
    background-color: white;
    margin: 20px auto;
    padding: 0;
    border-radius: 12px;
    width: 90%;
    max-width: 600px;
    box-shadow: 0 15px-35px rgba(0,0,0,0.2);
    animation: modalFadeIn 0.3s ease-out;
}

@keyframes modalFadeIn {
    from { transform: translateY(-30px); opacity: 0; }
    to { transform: translateY(0); opacity: 1; }
}

.modal-header {
    padding: 20px 25px;
    border-bottom: 1px solid #eee;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.modal-header h3 {
    margin: 0;
    color: #1976d2;
}

.close-modal {
    font-size: 1.8rem;
    font-weight: bold;
    color: #999;
    cursor: pointer;
    line-height: 1;
}

.close-modal:hover {
    color: #333;
}

#product-form {
    padding: 25px;
}

.form-row {
    display: flex;
    gap: 20px;
    margin-bottom: 20px;
}

.form-row .form-group {
    flex: 1;
    margin-bottom: 0;
}

.modal-footer {
    padding: 20px 0 0;
    display: flex;
    justify-content: flex-end;
    gap: 12px;
    border-top: 1px solid #eee;
    margin-top: 10px;
}

.btn-secondary {
    background-color: #f5f5f5;
    color: #666;
    border: 1px solid #ddd;
}

.btn-secondary:hover {
    background-color: #eeeeee;
}

/* Responsive adjustments */
@media (max-width: 768px) {
    .controls-container {
        flex-direction: column;
        align-items: stretch;
    }
    
    .filters-wrapper {
        justify-content: space-between;
    }
    
    .header h1 {
        font-size: 1.8rem;
    }
}

/* Login Page Styles */
.login-page {
    height: 100vh;
    display: flex;
    align-items: center;
    justify-content: center;
    background: linear-gradient(135deg, #1976d2 0%, #1565c0 100%);
}

.login-container {
    width: 100%;
    max-width: 400px;
    padding: 20px;
}

.login-card {
    background: white;
    padding: 40px;
    border-radius: 12px;
    box-shadow: 0 10px 25px rgba(0,0,0,0.2);
}

.login-header {
    text-align: center;
    margin-bottom: 30px;
}

.login-header i {
    font-size: 3rem;
    color: #1976d2;
    margin-bottom: 15px;
}

.login-header h2 {
    color: #333;
    font-size: 1.5rem;
    margin-bottom: 5px;
}

.login-header p {
    color: #666;
    font-size: 0.9rem;
}

.form-group {
    margin-bottom: 20px;
}

.form-group label {
    display: block;
    margin-bottom: 8px;
    font-size: 0.9rem;
    color: #555;
}

.input-wrapper {
    position: relative;
}

.input-wrapper i {
    position: absolute;
    left: 12px;
    top: 50%;
    transform: translateY(-50%);
    color: #999;
}

.input-wrapper input {
    width: 100%;
    padding: 12px 12px 12px 40px;
    border: 1px solid #ddd;
    border-radius: 6px;
    font-size: 1rem;
    transition: border-color 0.3s;
}

.input-wrapper input:focus {
    outline: none;
    border-color: #1976d2;
}

.btn-block {
    width: 100%;
    justify-content: center;
    padding: 12px;
    font-size: 1rem;
    margin-top: 10px;
}

.error-message {
    color: #d32f2f;
    background-color: #ffebee;
    padding: 10px;
    border-radius: 4px;
    font-size: 0.85rem;
    margin-bottom: 15px;
    text-align: center;
    border: 1px solid #ffcdd2;
}

