---
title: Criar convite
description: Use esta API para criar um novo convite. O convite adiciona um usuário externo à organização.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ed6dbfe4991d3dc36fba8cf66ca0177a93effcf6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568072"
---
# <a name="create-invitation"></a>Criar convite

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Use essa API para criar um novo [convite](../resources/invitation.md). O convite adiciona um usuário externo à organização.

Ao criar um novo convite, você tem várias opções disponíveis:

1. À criação do convite, o Microsoft Graph pode enviar automaticamente um email de convite diretamente ao usuário convidado, ou seu aplicativo pode usar o *inviteRedeemUrl* retornado na resposta da criação para articular o seu próprio convite (por meio de seu mecanismo de comunicação de preferência) para o usuário convidado. Se você decidir fazer com que o Microsoft Graph envie um email de convite automaticamente, poderá controlar o conteúdo e o idioma do email usando [ *invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).
2. Quando o usuário é convidado, uma entidade de usuário (do userType Convidado) é criada e, agora, pode ser usada para o controle do acesso aos recursos. O usuário convidado precisa passar pelo processo de resgate para acessar os recursos para os quais ele foi convidado.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).


|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Sem suporte.    |
|Aplicativo | User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Cabeçalho       | Valor |
|:---------------|:--------|
| Autorização  | {token} de portador. Obrigatório.  |
| Content-Type  | application/json  |

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça uma representação JSON do objeto [invitation](../resources/invitation.md).

A tabela a seguir mostra as propriedades que são necessárias ao criar um convite.

| Parâmetro | Tipo | Descrição|
|:---------------|:--------|:----------|
|invitedUserEmailAddress |string | O endereço de email do usuário que você está convidando.|
|inviteRedirectUrl |string |A URL para a qual o usuário será redirecionado após o resgate.|

## <a name="response"></a>Resposta

Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [invitation](../resources/invitation.md) no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo da solicitação.
<!-- {
  "blockType": "request",
  "name": "create_user_from_users"
}-->
```http
POST https://graph.microsoft.com/beta/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.com"
}
```

##### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.invitation"
} -->
```http
HTTP/1.1 201 OK
Content-type: application/json
Content-length: 551

{
  "id": "7b92124c-9fa9-406f-8b8e-225df8376ba9",
  "inviteRedeemUrl": "https://invitations.microsoft.com/redeem/?tenant=04dcc6ab-388a-4559-b527-fbec656300ea&user=7b92124c-9fa9-406f-8b8e-225df8376ba9&ticket=VV9dmiExBsfRIVNFjb9ITj9VXAd07Ypv4gTg%2f8PiuJs%3d&lc=1033&ver=2.0",
  "invitedUserDisplayName": "yyy",
  "invitedUserEmailAddress": "yyy@test.com",
  "sendInvitationMessage": false,
  "invitedUserMessageInfo": {
     "messageLanguage": null,
     "ccRecipients": [
          {
             "emailAddress": {
                 "name": null,
                 "address": null
              }
          }
     ],
     "customizedMessageBody": null
  },
  "inviteRedirectUrl": "https://myapp.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```
