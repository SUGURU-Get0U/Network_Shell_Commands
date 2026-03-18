## 🛠️ Cheat Sheet: Análise de Sistema e Inicialização (Windows/Linux)
> Notas sobre Hardware, Firmware (UEFI/BIOS) e Particionamento (GPT/MBR).

## 🪟 Windows (PowerShell - Foco em Adm de Sistemas)
Se as ferramentas gráficas (`msinfo32` ou `diskmgmt.msc`) estiverem bloqueadas por permissão de administrador:

### 1. Verificar Tabela de Partição (GPT vs MBR)
```powershell
Get-Disk | Select-Object Number, FriendlyName, PartitionStyle, Size
