# <a name="defenderthreataction-enum-type"></a>tipo de enum defenderThreatAction

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Ação de padrão do Defender assuma detectadas ameaças de Malware.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Aplica a ação com base na definição de atualização.|
|clean|1|Limpe ameaça detectada.|
|quarentena|2|Quarentena ameaça detectada.|
|remover|3|Remova ameaça detectada.|
|permitir|4|Permitir ameaça detectada.|
|userDefined|5|Permitir que o usuário determinar a ação a ser executada com ameaça detectada.|
|bloquear|6|Bloquear ameaça detectada.|



