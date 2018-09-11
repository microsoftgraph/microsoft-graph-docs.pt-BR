# <a name="windowsdeliveryoptimizationmode-enum-type"></a>tipo enumerado windowsDeliveryOptimizationMode

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entregar modo de otimização para distribuição de mesmo nível
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Permitir que o usuário configure.|
|httpOnly|1|Apenas HTTP, nenhum emparelhamento|
|httpWithPeeringNat|2|Padrão do sistema operacional – Http misturados com correspondência atrás do mesmo conversor de endereços de rede|
|httpWithPeeringPrivateGroup|3|HTTP misturado com emparelhamento entre um grupo privado|
|httpWithInternetPeering|4|HTTP misturado com correspondência de Internet|
|simpleDownload|99|Modo de download simples sem emparelhamento|
|bypassMode|100|Modo de bypass. Não usar a otimização de entrega e usar o BITS|








