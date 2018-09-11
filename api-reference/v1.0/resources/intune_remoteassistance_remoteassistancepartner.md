# <a name="remoteassistancepartner-resource-type"></a>Tipo de recurso remoteAssistancePartner

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Recursos de remoteAssistPartner representam metadados e status de um determinado serviço de Parceiro de assistência remota.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar remoteAssistancePartners](../api/intune_remoteassistance_remoteassistancepartner_list.md)|Conjunto [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Listar propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Obter remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_get.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Ler propriedades e relações de objetos de [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Criar remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_create.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Criar um novo objeto de [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Excluir remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_delete.md)|Nenhum|Excluir [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Atualizar remoteAssistancePartner](../api/intune_remoteassistance_remoteassistancepartner_update.md)|[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md)|Atualizar as propriedades de um objeto de [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).|
|[Ação beginOnboarding](../api/intune_remoteassistance_remoteassistancepartner_beginonboarding.md)|Nenhum|Ainda não documentado|
|[ação de desconectar](../api/intune_remoteassistance_remoteassistancepartner_disconnect.md)|Nenhum|Ainda não documentado|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do parceiro.|
|displayName|Cadeia de caracteres|Nome de exibição do parceiro.|
|onboardingUrl|Cadeia de caracteres|URL do portal de integração do parceiro, no qual um administrador pode configurar o serviço de assistência remota.|
|onboardingStatus|[remoteAssistanceOnboardingStatus](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|TBD. Os valores possíveis são: `notOnboarded`, `onboarding`, `onboarded`.|
|lastConnectionDateTime|DateTimeOffset|Carimbo de data/hora da última solicitação enviada ao Intune pelo parceiro TEM.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.remoteAssistancePartner"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "String (identifier)",
  "displayName": "String",
  "onboardingUrl": "String",
  "onboardingStatus": "String",
  "lastConnectionDateTime": "String (timestamp)"
}
```








