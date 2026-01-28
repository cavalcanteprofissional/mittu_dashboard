# 📊 Mittu Dashboard

[![Streamlit](https://img.shields.io/badge/Streamlit-1.53.1-red)](https://streamlit.io/)
[![Python](https://img.shields.io/badge/Python-3.14+-blue)](https://www.python.org/)
[![Poetry](https://img.shields.io/badge/Poetry-1.8.0-60A5FA)](https://python-poetry.org/)

A comprehensive Streamlit dashboard for project management data visualization, built with Python and managed using Poetry for dependency management.

## 🚀 Quick Start

### Prerequisites

- **Python 3.14+**
- **Poetry** installed ([Installation Guide](https://python-poetry.org/docs/#installation))

### Installation & Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/cavalcanteprofissional/mittu_dashboard.git
   cd mittu_dashboard
   ```

2. **Install dependencies with Poetry**
   ```bash
   poetry install
   ```

3. **Run the dashboard**
   ```bash
   poetry run streamlit run dashboard.py
   ```

4. **Open your browser**
   Navigate to `http://localhost:8501`

## 📁 Project Structure

```
mittu_dashboard/
├── pyproject.toml          # Poetry configuration & dependencies
├── poetry.lock             # Locked dependency versions
├── dashboard.py            # Main Streamlit application (440 lines)
├── .gitignore              # Git ignore patterns
├── README.md               # This file
└── data/
    └── joined_projects_data.csv  # Project management data
```

## ✨ Features

### 📈 Key Performance Indicators
- **Total Projects**: Overall project count
- **Status Distribution**: Projects by current status
- **Completion Rate**: Average percentage completed
- **Cost Variance**: Budget vs actual spending

### 📊 Visualizations
- **Status Pie Chart**: Interactive breakdown of project statuses
- **Cost Comparison**: Planned vs actual costs by department
- **Area Analysis**: Comprehensive department-wise metrics
- **Detailed Data Table**: Expandable formatted project data

### 🎯 Dashboard Components
- Real-time data processing with Pandas
- Interactive charts using Plotly
- Responsive layout for all screen sizes
- Brazilian Portuguese currency formatting
- Color-coded status indicators

## 🛠️ Technology Stack

| Technology | Version | Purpose |
|------------|---------|---------|
| **Streamlit** | 1.53.1 | Web application framework |
| **Pandas** | 2.3.3 | Data processing & analysis |
| **Plotly** | 5.24.1 | Interactive visualizations |
| **NumPy** | 1.26.4 | Numerical operations |
| **Poetry** | 1.8.0 | Dependency management |

## 📋 Data Schema

The dashboard processes project management data with the following key fields:

- `project_id`: Unique project identifier
- `status`: Current project status (em dia, atrasado, critico, etc.)
- `area`: Department/area responsible
- `conclusao`: Completion percentage
- `valor`: Actual costs incurred
- `custo_previsto`: Planned/budgeted costs
- `inicio`: Project start date
- `prazo`: Project deadline

## 🎨 Status Color Coding

| Status | Color | Description |
|--------|-------|-------------|
| em dia | 🟢 Sea Green | On schedule |
| atrasado | 🟠 Dark Orange | Delayed |
| critico | 🔴 Crimson | Critical |
| pausado | ⚫ Slate Gray | Paused |
| concluido | 🔵 Steel Blue | Completed |
| andamento | 🟢 Medium Sea Green | In progress |

## 🔧 Development

### Adding New Features

1. Modify `dashboard.py` with new functionality
2. Update dependencies in `pyproject.toml` if needed
3. Test with `poetry run streamlit run dashboard.py`

### Environment Management

```bash
# Check Poetry environment
poetry env info

# Update dependencies
poetry update

# Add new package
poetry add package_name
```

## 📝 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📞 Support

For questions or support, please open an issue on the [GitHub repository](https://github.com/cavalcanteprofissional/mittu_dashboard/issues).

---

**Built with ❤️ using Streamlit and Poetry**