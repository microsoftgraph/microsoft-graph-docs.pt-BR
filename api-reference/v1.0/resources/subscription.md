# <a name="subscription-resource-type"></a>Tipo de Recurso de Assinatura
Uma assinatura permite que um aplicativo cliente receba notificações sobre dados no Microsoft Graph. Atualmente, as assinaturas estão habilitadas para as seguintes coleções de dados:

1. Email, eventos e contatos do Outlook
1. Conversas de Grupos do Office.
1. Itens raiz de unidade no OneDrive 


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.subscription"
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "expirationDateTime": "string (timestamp)",
  "id": "string (identifier)",
  "clientState": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|changeType|string|Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula.|
|notificationUrl|string|A URL do ponto de extremidade que receberá as notificações. Esta URL tem que usar o protocolo HTTPS.|
|recurso|cadeia de caracteres|Especifica o recurso que será monitorado para detectar alterações. Não inclua a URL base ("https://graph.microsoft.com/v1.0/").|
|expirationDateTime|[dateTime](http://tools.ietf.org/html/rfc3339)|Especifica a data e a hora em que a assinatura de webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
|clientState|string|Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação.|
|id|string|Identificador exclusivo da assinatura. Somente leitura.|

## <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso
| Recurso | Tempo de Expiração Máximo |
|:---------------------|:--------------------|
|Email| 4230 minutos.|
|Calendário| 4230 minutos.|
|Contatos| 4230 minutos.|
|Conversas em grupo| 4230 minutos.|
|Itens raiz de unidade| 43.200 minutos. Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor máximo. Valores maiores não serão permitidos nos próximos lançamentos. |

## <a name="relationships"></a>Relações
Nenhuma


## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar assinatura](../api/subscription_post_subscriptions.md) | [subscription](subscription.md) |Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados.|
|[Atualizar assinatura](../api/subscription_update.md) | [subscription](subscription.md) |Renova uma assinatura atualizando seu tempo de expiração.|
|[Obter assinatura](../api/subscription_get.md) | [subscription](subscription.md) |Lê as propriedades e as relações do objeto subscription.|
|[Excluir assinatura](../api/subscription_delete.md) | Nenhuma |Exclui um objeto subscription.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
