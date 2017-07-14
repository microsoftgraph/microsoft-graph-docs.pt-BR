# gerenciador de convites
<a id="invitation-manager" class="xliff"></a>

Use o gerenciador de convites para criar um convite para adicionar um usuário externo à organização. 

O processo de convite usa o fluxo a seguir:

* Um convite é criado
* Um convite é enviado ao usuário convidado (contendo um link do convite)
* O usuário convidado clica no link do convite, entra e recupera o convite, e a criação da entidade de usuário que representa o usuário convidado é concluída
* O usuário é redirecionado para uma página específica após a conclusão do resgate

A criação de um convite retornará uma URL de resgate na resposta (*inviteRedeemUrl*). A API de criação de convite pode enviar automaticamente um email que contém a URL de resgate ao usuário convidado, definindo-se *sendInvitationMessage* como true. Você também pode personalizar a mensagem será enviada ao usuário convidado. Em vez disso, se você desejar enviar a URL de resgate por outros meios, poderá definir *sendInvitationMessage* como false e usar a URL de resgate da resposta para criar sua própria comunicação. Atualmente, não há qualquer API para execução do processo de resgate. O usuário convidado tem que clicar no link *inviteRedeemUrl* enviado na comunicação na etapa anterior e passar pelo processo de resgate interativo em um navegador. Após a conclusão, o usuário convidado torna-se um usuário externo na organização.


## Métodos
<a id="methods" class="xliff"></a>
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Criar convite](../api/invitation_post.md) | invitation | Escreva as propriedades e os relacionamentos do objeto invitation.|

## Propriedades
<a id="properties" class="xliff"></a>
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|invitedUserDisplayName|String|O nome de exibição do usuário que está sendo convidado.|
|invitedUserEmailAddress|String|O endereço de email do usuário que está sendo convidado. Obrigatório.|
|invitedUserMessageInfo|[invitedUserMessageInfo](invitedusermessageinfo.md)|Configurações adicionais para a mensagem que está sendo enviada ao usuário convidado, incluindo a lista de destinatários cc, o idioma e o texto da mensagem de personalização.|
|sendInvitationMessage|Boolean|Indica se um email deve ser enviado ao usuário que está sendo convidado ou não. O padrão é false.|
|inviteRedirectUrl|String|A URL para a qual o usuário deve ser redirecionado após o resgate do convite. Obrigatório.|
|inviteRedeemUrl|String|A URL que o usuário pode usar para resgatar o convite. Somente leitura|
|invitedUserType|String|O userType do usuário que está sendo convidado. Por padrão, é Convidado. Você pode convidar como Membro se não for administrador da empresa. |
|status|String|O status do convite. Valores possíveis: PendingAcceptance, Completed, InProgress, e Error|

## Relações
<a id="relationships" class="xliff"></a>
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|invitedUser|[User](user.md)|O usuário criado como parte da criação do convite. Somente leitura|

## Representação JSON
<a id="json-representation" class="xliff"></a>
Veja a seguir uma representação JSON do recurso

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.invitations" } -->
```json
{
  "invitedUserDisplayName": "string",
  "invitedUserEmailAddress": "string",
  "invitedUserMessageInfo": {"@odata.type": "microsoft.graph.invitedUserMessageInfo"},
  "sendInvitationMessage": false,
  "inviteRedirectUrl": "string",
  "inviteRedeemUrl": "string",
  "status": "string",

  "invitedUser": [{"@odata.type": "microsoft.graph.user"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2016-22-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "invitation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
