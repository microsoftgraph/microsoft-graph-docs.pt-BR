# <a name="firewallpacketqueueingmethodtype-enum-type"></a>tipo de enum firewallPacketQueueingMethodType

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Valores possíveis para firewallPacketQueueingMethod
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Nenhum valor configurado por Intune, não substituir o valor padrão de dispositivo configurada pelo usuário|
|desabilitado|1|Desabilitar o serviço de enfileiramento de pacotes|
|queueInbound|2|Os pacotes criptografados entrados de fila|
|queueOutbound|3|Fila descriptografados para encaminhamento de pacotes de saída|
|queueBoth|4|Pacotes de entrada e saídos da fila|



