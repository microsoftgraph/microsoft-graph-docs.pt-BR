# <a name="subscription-resource-type"></a>tipo de recurso de assinatura

Uma assinatura permite que um aplicativo cliente receba notificações sobre as alterações de dados no Microsoft Graph. Atualmente, as assinaturas são habilitadas para os seguintes recursos:

- Email, eventos e contatos do Outlook
- Conversas de Grupos do Office
- Itens raiz de unidade no OneDrive
- Usuários e grupos do Azure Active Directory

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.subscription",
  "@odata.annotations": [
    {
      "capabilities": {
        "skippable": false,
        "toppable": false,
        "countable": false,
        "expandable": false,
        "filterable": false,
        "referenceable": false,
        "selectable": false,
        "sortable": false
      }
    }
  ]
}-->

```json
{
  "changeType": "string",
  "notificationUrl": "string",
  "resource": "string",
  "applicationId" : "string",
  "expirationDateTime": "String (timestamp)",
  "id": "string (identifier)",
  "clientState": "string",
  "creatorId": "string"
}
```

## <a name="properties"></a>Propriedades

| Propriedade | Tipo | Descrição |
|:---------|:-----|:------------|
| changeType | sequência de caracteres | Obrigatório. Indica o tipo de alteração no recurso inscrito que gerará uma notificação. Os valores com suporte são: `created`, `updated`, `deleted`. Vários valores podem ser combinados usando uma lista separada por vírgula.<br><br>Nota: Notificações de item de raiz de unidade suportam somente a `updated` changeType. Suporte a notificações de usuários e grupos `updated` e `deleted` changeType.|
| notificationUrl | sequência de caracteres | Obrigatório. A URL do ponto de extremidade que receberá as notificações. Essa URL deve usar o protocolo HTTPS. |
| recurso | sequência de caracteres | Obrigatório. Especifica o recurso cujas alterações serão monitoradas. Não incluir a URL base (`https://graph.microsoft.com/v1.0/`). |
| expirationDateTime | [dateTime](http://tools.ietf.org/html/rfc3339) | Obrigatório. Especifica a data e a hora em que a assinatura do webhook expira. O horário está em UTC e pode ser uma quantidade de tempo desde a criação da assinatura que varia para o recurso assinado.  Confira na tabela abaixo o tempo máximo permitido para a assinatura. |
| clientState | sequência de caracteres | Opcional. Especifica o valor da propriedade `clientState` enviada pelo serviço em cada notificação. O comprimento máximo é de 128 caracteres. O cliente pode verificar se a notificação foi proveniente do serviço comparando o valor da propriedade `clientState` enviada com a assinatura com o valor da propriedade `clientState` recebida com cada notificação. |
| id | sequência de caracteres | Identificador exclusivo da assinatura. Somente leitura. |
| applicationId | cadeia de caracteres | Identificador do aplicativo usado para criar a assinatura. Somente leitura. |
| creatorId | cadeia de caracteres | Identificador do usuário ou da entidade de serviço que criou a assinatura. Se o aplicativo usou permissões delegadas para criar a assinatura, esse campo contém o ID do usuário conectado em nome do qual o aplicativo foi chamado. Se o aplicativo usou as permissões do aplicativo, esse campo contém o id da entidade de serviço correspondente para o aplicativo. Somente leitura. |

## <a name="maximum-length-of-subscription-per-resource-type"></a>Tamanho máximo da assinatura por tipo de recurso

| Recurso            | Tempo de Expiração Máximo  |
|:--------------------|:-------------------------|
| Email                | 4230 minutos (menos de 3 dias)    |
| Calendário            | 4230 minutos (menos de 3 dias)    |
| Contatos            | 4230 minutos (menos de 3 dias)    |
| Conversas em grupo | 4230 minutos (menos de 3 dias)    |
| Itens raiz de unidade    | 4230 minutos (menos de 3 dias)    |

> **Observação:** Os aplicativos existentes e os novos aplicativos não devem ultrapassar o valor máximo. No futuro, quaisquer solicitações para criar ou renovar uma assinatura além do valor máximo, falhará.

## <a name="relationships"></a>Relacionamentos

Nenhum

## <a name="methods"></a>Métodos

| Método | Tipo de retorno | Descrição |
|:-------|:------------|:------------|
| [Criar assinatura](../api/subscription_post_subscriptions.md) | [assinatura](subscription.md) | Assina um aplicativo de escuta para receber notificações quando dados do Microsoft Graph são alterados. |
| [Atualizar assinatura](../api/subscription_update.md) | [assinatura](subscription.md) | Renova uma assinatura atualizando seu tempo de expiração. |
| [Assinaturas de lista](../api/subscription_list.md) | [assinatura](subscription.md) | Lista as assinaturas ativas. |
| [Obter assinatura](../api/subscription_get.md) | [assinatura](subscription.md) | Lê as propriedades e as relações do objeto subscription. |
| [Excluir assinatura](../api/subscription_delete.md) | Nenhuma |Exclui um objeto subscription. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "subscription resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
