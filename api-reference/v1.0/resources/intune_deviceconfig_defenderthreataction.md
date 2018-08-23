# <a name="defenderthreataction-enum-type"></a>Tipo enumerado defenderThreatAction

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ação padrão do Defender para assumir as ameaças de malware detectadas.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Aplique a ação com base na definição de atualização.|
|clean|1|Apague a ameaça detectada.|
|quarantine|2|Coloque a ameaça detectada em quarentena.|
|remove|3|Remova a ameaça detectada.|
|allow|4|Permita a ameaça detectada.|
|userDefined|5|Permita que o usuário determine a ação a ser tomada para a ameaça detectada.|
|block|6|Bloqueie a ameaça detectada.|



