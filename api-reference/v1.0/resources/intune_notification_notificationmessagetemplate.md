# <a name="notificationmessagetemplate-resource-type"></a>Tipo de recurso notificationMessageTemplate

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Mensagens de notificação são mensagens enviadas para usuários finais considerados não compatíveis com as políticas de conformidade definidas pelo administrador. Os administradores escolhem as notificações e as configuram no Console do administrador do Intune usando a página de criação de política de conformidade, na seção "Ações de não conformidade". Use o objeto notificationMessageTemplate para criar suas próprias notificações personalizadas para os administradores escolherem durante a configuração de ações de não conformidade.
## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar notificationMessageTemplates](../api/intune_notification_notificationmessagetemplate_list.md)|Conjunto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Listar propriedades e relações dos objetos [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Obter notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_get.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Ler propriedades e relações do objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Criar notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_create.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Criar um novo objeto de [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Excluir notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_delete.md)|Nenhum|Excluir um [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Atualizar notificationMessageTemplate](../api/intune_notification_notificationmessagetemplate_update.md)|[notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md)|Atualizar as propriedades de um objeto [notificationMessageTemplate](../resources/intune_notification_notificationmessagetemplate.md).|
|[Ação sendTestMessage](../api/intune_notification_notificationmessagetemplate_sendtestmessage.md)|Nenhum|Envia mensagens de teste usando o notificationMessageTemplate especificado no local padrão|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave da entidade.|
|lastModifiedDateTime|DateTimeOffset|DateTime da última modificação do objeto.|
|displayName|Cadeia de caracteres|Nome de exibição do modelo de mensagem de notificação.|
|defaultLocale|Cadeia de caracteres|A localidade padrão para fallback quando a localidade solicitada não está disponível.|
|brandingOptions|[notificationTemplateBrandingOptions](../resources/intune_notification_notificationtemplatebrandingoptions.md)|As opções de identidade visual do modelo de mensagem. A identidade visual é definida no Console do Admin do Intune. Os valores possíveis são: `none`, `includeCompanyLogo`, `includeCompanyName`, `includeContactInformation`.|

## <a name="relationships"></a>Relacionamentos
|Relação|Tipo|Descrição|
|:---|:---|:---|
|localizedNotificationMessages|Coleção [localizedNotificationMessage](../resources/intune_notification_localizednotificationmessage.md)|A lista de mensagens localizadas para esse modelo de mensagem de notificação.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.notificationMessageTemplate"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.notificationMessageTemplate",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "defaultLocale": "String",
  "brandingOptions": "String"
}
```








