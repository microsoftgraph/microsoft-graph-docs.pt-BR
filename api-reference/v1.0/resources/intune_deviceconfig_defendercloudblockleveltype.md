# <a name="defendercloudblockleveltype-enum-type"></a>tipo enumerado defenderCloudBlockLevelType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis de nível de bloqueio na nuvem
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notConfigured|0|Valor padrão, usa o padrão do nível de bloqueio do antivírus do Windows Defender e fornece detecção forte sem aumentar o risco de detecção de arquivos legítimos|
|high|1|Alto aplica um alto nível de detecção.|
|highPlus|2|Alto + usa o nível alto e aplica medidas de proteção adicionais|
|zeroTolerance|3|Tolerância zero bloqueia todos os executáveis desconhecidos|



