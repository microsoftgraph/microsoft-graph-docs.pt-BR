# <a name="devicemanagementexchangeaccessstatereason-enum-type"></a>Tipo enumerado deviceManagementExchangeAccessStateReason

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Motivo do estado de acesso ao Exchange do dispositivo.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Nenhum motivo do estado de acesso descoberto do Exchange|
|unknown|1|Motivo do estado de acesso desconhecido|
|exchangeGlobalRule|2|Estado de acesso determinado pela regra Global do Exchange|
|exchangeIndividualRule|3|Estado de acesso determinado pela regra Individual do Exchange|
|exchangeDeviceRule|4|Estado de acesso determinado pela regra de Dispositivo do Exchange|
|exchangeUpgrade|5|Estado de acesso devido à atualização do Exchange|
|exchangeMailboxPolicy|6|Estado de acesso determinado pela Política de caixa de correio do Exchange|
|other|7|Estado de acesso determinado pelo Exchange|
|compliant|8|Estado de acesso concedido pelo desafio de conformidade|
|notCompliant|9|Estado de acesso revogado pelo desafio de conformidade|
|notEnrolled|10|Estado de acesso revogado pelo desafio de gerenciamento|
|unknownLocation|12|Estado de acesso devido a uma localização desconhecida|
|mfaRequired|13|Estado de acesso devido ao desafio MFA|
|azureADBlockDueToAccessPolicy|14|Estado de acesso revogado pela Política de acesso do AAD|
|compromisedPassword|15|Estado de acesso revogado por senha comprometida|
|deviceNotKnownWithManagedApp|16|Estado de acesso revogado pelo desafio de aplicativo gerenciado|








