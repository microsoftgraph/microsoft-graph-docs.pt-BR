# <a name="localizednotificationmessage-resource-type"></a>tipo de recurso localizedNotificationMessage

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

O conteúdo do texto de um Modelo de mensagem de notificação para a localidade especificada.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar localizedNotificationMessages](../api/intune_notification_localizednotificationmessage_list.md)|Conjunto [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Listar propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Obter localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_get.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Ler propriedades e relações de objetos de [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Criar localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_create.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Criar um novo objeto de [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Excluir localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_delete.md)|Nenhum|Excluir [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|
|[Atualizar localizedNotificationMessage](../api/intune_notification_localizednotificationmessage_update.md)|[localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|Atualizar as propriedades de um objeto de [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|Última modificação de DateTime do objeto.|
|localidade|Cadeia de caracteres|A localidade para a qual esta mensagem se destina.|
|assunto|Cadeia de caracteres|O assunto do modelo da mensagem.|
|messageTemplate|Cadeia de caracteres|O conteúdo do modelo da mensagem.|
|isDefault|Booliano|Sinaliza para indicar se esta é ou não a localidade padrão do fallback de idioma. Esse sinalizador só pode ser definido. Para remover a definição, defina esta propriedade como verdadeira na outra Mensagem de notificação localizada.|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.localizedNotificationMessage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.localizedNotificationMessage",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "locale": "String",
  "subject": "String",
  "messageTemplate": "String",
  "isDefault": true
}
```



