# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo enumerado firewallPacketQueueingMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallPacketQueueingMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado pelo Intune, não substituir o valor padrão de dispositivo configurado pelo usuário|
|disabled|1|Desativar o serviço de enfileiramento de pacotes|
|queueInbound|2|Pacotes criptografados na fila de entrada|
|queueOutbound|3|Pacotes descriptografados na fila de saída para encaminhamento|
|queueBoth|4|Pacotes nas filas de entrada e saída|








