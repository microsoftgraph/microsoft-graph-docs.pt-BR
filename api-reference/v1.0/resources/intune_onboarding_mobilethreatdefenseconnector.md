# <a name="mobilethreatdefenseconnector-resource-type"></a>Tipo de recurso mobileThreatDefenseConnector

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Entidade que representa uma conexão com o parceiro de defesa contra ameaças móveis.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mobileThreatDefenseConnectors](../api/intune_onboarding_mobilethreatdefenseconnector_list.md)|Coleção [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Lista propriedades e relações dos objetos [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Obter mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_get.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Propriedades de leitura e relações do objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Criar mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_create.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Cria um novo objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Excluir mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_delete.md)|Nenhuma|Exclui um [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|
|[Atualizar mobileThreatDefenseConnector](../api/intune_onboarding_mobilethreatdefenseconnector_update.md)|[mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md)|Atualiza as propriedades de um objeto [mobileThreatDefenseConnector](../resources/intune_onboarding_mobilethreatdefenseconnector.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|lastHeartbeatDateTime|DateTimeOffset|Carimbo de data/hora da última pulsação após a opção habilitada pelo administrador Conectar-se ao MTP|
|partnerState|Cadeia de caracteres|Estado do parceiro deste locatário. Os valores possíveis são: `unavailable`, `available`, `enabled`, `unresponsive`.|
|androidEnabled|Booliano|Botão Ativar ou Desativar do Android|
|androidDeviceBlockedOnMissingPartnerData|Booliano|Para o Android, os administradores com permissão para configurar devem receber dados do parceiro de sincronização de dados antes de serem considerados compatíveis|
|iosDeviceBlockedOnMissingPartnerData|Booliano|Para o iOS, os administradores com permissão para configurar devem receber dados do parceiro de sincronização de dados antes de serem considerados compatíveis|
|partnerUnsupportedOsVersionBlocked|Booliano|Permite que o administrador bloqueie dispositivos nas plataformas habilitadas que não atenderem aos requisitos de versão mínima|
|iosEnabled|Booliano|Botão Ativar ou Desativar do iOS|
|partnerUnresponsivenessThresholdInDays|Int32|Obtém ou define dias de tolerância por locatário à falta de resposta para esta integração de parceiro|

## <a name="relationships"></a>Relações
Nenhuma
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileThreatDefenseConnector"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileThreatDefenseConnector",
  "id": "String (identifier)",
  "lastHeartbeatDateTime": "String (timestamp)",
  "partnerState": "String",
  "androidEnabled": true,
  "androidDeviceBlockedOnMissingPartnerData": true,
  "iosDeviceBlockedOnMissingPartnerData": true,
  "partnerUnsupportedOsVersionBlocked": true,
  "iosEnabled": true,
  "partnerUnresponsivenessThresholdInDays": 1024
}
```



