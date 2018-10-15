# <a name="manageddevicepartnerreportedhealthstate-enum-type"></a>tipo enumerado managedDevicePartnerReportedHealthState

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Integridades de dispositivo disponíveis para a Integridade de Dispositivo da API
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Integridade de dispositivo ainda não foi relatada|
|activated|1|Dispositivo foi ativado por um parceiro de defesa contra ameaças móveis, mas a integridade ainda não foi relatada.|
|deactivated|2|O dispositivo foi desativado por um parceiro de defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|secured|3|Dispositivo é considerado protegido pelo parceiro de defesa contra ameaças móveis.|
|lowSeverity|4|Dispositivo é considerado de baixa ameaça pelo parceiro de defesa contra ameaças móveis.|
|mediumSeverity|5|Dispositivo é considerado ameaça média pelo parceiro de defesa contra ameaças móveis.|
|highSeverity|6|Dispositivo é considerado ameaça alta pelo parceiro defesa contra ameaças móveis.|
|unresponsive|7|Dispositivo é considerado como não respondendo pelo parceiro defesa contra ameaças móveis. A integridade do dispositivo não é conhecida.|
|compromised|8|Dispositivo é considerado comprometido pelo parceiro de defesa contra ameaças. Isso significa que o dispositivo tem uma ameaça ou o risco ativo que não pode ser facilmente corrigido pelo usuário final. O usuário deve entrar em contato com o administrador de TI.|
|misconfigured|9|Dispositivo é considerado configurado incorretamente com o parceiro de defesa contra ameaças. Isso significa que falta um perfil ou configuração necessária para que o parceiro de defesa contra ameaças funcione corretamente, portanto não é possível concluir a análise de riscos e ameaças.|








