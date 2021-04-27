---
title: Criar convite
description: Use essa API para criar um novo convite. O convite adiciona um usuário externo à organização.
localization_priority: Normal
author: Sammak
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 99fb4703e4ae2b4d8714475577c7e34c1c34c8c6
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053661"
---
# <a name="create-invitation"></a><span data-ttu-id="94a7f-104">Criar convite</span><span class="sxs-lookup"><span data-stu-id="94a7f-104">Create invitation</span></span>

<span data-ttu-id="94a7f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="94a7f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="94a7f-p102">Use essa API para criar um novo [convite](../resources/invitation.md). O convite adiciona um usuário externo à organização.</span><span class="sxs-lookup"><span data-stu-id="94a7f-p102">Use this API to create a new [invitation](../resources/invitation.md). Invitation adds an external user to the organization.</span></span>

<span data-ttu-id="94a7f-108">Ao criar um novo convite, você tem várias opções disponíveis:</span><span class="sxs-lookup"><span data-stu-id="94a7f-108">When creating a new invitation you have several options available:</span></span>

1. <span data-ttu-id="94a7f-p103">À criação do convite, o Microsoft Graph pode enviar automaticamente um email de convite diretamente ao usuário convidado, ou seu aplicativo pode usar o *inviteRedeemUrl* retornado na resposta da criação para articular o seu próprio convite (por meio de seu mecanismo de comunicação de preferência) para o usuário convidado. Se você decidir fazer com que o Microsoft Graph envie um email de convite automaticamente, poderá controlar o conteúdo e o idioma do email usando [ *invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span><span class="sxs-lookup"><span data-stu-id="94a7f-p103">On invitation creation, Microsoft Graph can automatically send an invitation email directly to the invited user, or your app can use the *inviteRedeemUrl* returned in the creation response to craft your own invitation (through your communication mechanism of choice) to the invited user. If you decide to have Microsoft Graph send an invitation email automatically, you can control the content and language of the email using [*invitedUserMessageInfo*](../resources/invitedusermessageinfo.md).</span></span>
2. <span data-ttu-id="94a7f-p104">Quando o usuário é convidado, uma entidade de usuário (do userType Convidado) é criada e, agora, pode ser usada para o controle do acesso aos recursos. O usuário convidado precisa passar pelo processo de resgate para acessar os recursos para os quais ele foi convidado.</span><span class="sxs-lookup"><span data-stu-id="94a7f-p104">When the user is invited, a user entity (of userType Guest) is created and can now be used to control access to resources. The invited user has to go through the redemption process to access any resources he has been invited to.</span></span>

## <a name="permissions"></a><span data-ttu-id="94a7f-113">Permissões</span><span class="sxs-lookup"><span data-stu-id="94a7f-113">Permissions</span></span>
<span data-ttu-id="94a7f-p105">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94a7f-p105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="94a7f-116">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94a7f-116">Permission type</span></span>      | <span data-ttu-id="94a7f-117">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="94a7f-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="94a7f-118">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94a7f-118">Delegated (work or school account)</span></span> | <span data-ttu-id="94a7f-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a7f-119">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span>    |
|<span data-ttu-id="94a7f-120">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94a7f-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="94a7f-121">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94a7f-121">Not supported.</span></span>    |
|<span data-ttu-id="94a7f-122">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94a7f-122">Application</span></span> | <span data-ttu-id="94a7f-123">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94a7f-123">User.Invite.All, User.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="94a7f-124">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94a7f-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /invitations
```
## <a name="request-headers"></a><span data-ttu-id="94a7f-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94a7f-125">Request headers</span></span>
| <span data-ttu-id="94a7f-126">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94a7f-126">Header</span></span>       | <span data-ttu-id="94a7f-127">Valor</span><span class="sxs-lookup"><span data-stu-id="94a7f-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="94a7f-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="94a7f-128">Authorization</span></span>  | <span data-ttu-id="94a7f-p106">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94a7f-p106">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="94a7f-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="94a7f-131">Content-Type</span></span>  | <span data-ttu-id="94a7f-132">application/json</span><span class="sxs-lookup"><span data-stu-id="94a7f-132">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="94a7f-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94a7f-133">Request body</span></span>
<span data-ttu-id="94a7f-134">No corpo da solicitação, forneça uma representação JSON do objeto [invitation](../resources/invitation.md).</span><span class="sxs-lookup"><span data-stu-id="94a7f-134">In the request body, supply a JSON representation of an [invitation](../resources/invitation.md) object.</span></span>

<span data-ttu-id="94a7f-135">A tabela a seguir mostra as propriedades que são necessárias ao criar um convite.</span><span class="sxs-lookup"><span data-stu-id="94a7f-135">The following table shows the properties that are required when you create a invitation.</span></span>

| <span data-ttu-id="94a7f-136">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="94a7f-136">Parameter</span></span> | <span data-ttu-id="94a7f-137">Tipo</span><span class="sxs-lookup"><span data-stu-id="94a7f-137">Type</span></span> | <span data-ttu-id="94a7f-138">Descrição</span><span class="sxs-lookup"><span data-stu-id="94a7f-138">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94a7f-139">invitedUserEmailAddress</span><span class="sxs-lookup"><span data-stu-id="94a7f-139">invitedUserEmailAddress</span></span> |<span data-ttu-id="94a7f-140">string</span><span class="sxs-lookup"><span data-stu-id="94a7f-140">string</span></span> | <span data-ttu-id="94a7f-141">O endereço de email do usuário que você está convidando.</span><span class="sxs-lookup"><span data-stu-id="94a7f-141">The email address of the user you are inviting.</span></span>|
|<span data-ttu-id="94a7f-142">inviteRedirectUrl</span><span class="sxs-lookup"><span data-stu-id="94a7f-142">inviteRedirectUrl</span></span> |<span data-ttu-id="94a7f-143">string</span><span class="sxs-lookup"><span data-stu-id="94a7f-143">string</span></span> |<span data-ttu-id="94a7f-144">A URL para a qual o usuário será redirecionado após o resgate.</span><span class="sxs-lookup"><span data-stu-id="94a7f-144">The URL that the user will be redirected to after redemption.</span></span>|

## <a name="response"></a><span data-ttu-id="94a7f-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a7f-145">Response</span></span>

<span data-ttu-id="94a7f-146">Se bem-sucedido, este método retorna um código de resposta `201 Created` e um objeto [invitation](../resources/invitation.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a7f-146">If successful, this method returns `201 Created` response code and [invitation](../resources/invitation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94a7f-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94a7f-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="94a7f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94a7f-148">Request</span></span>
<span data-ttu-id="94a7f-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94a7f-149">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="94a7f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="94a7f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_invitation_post"
}-->
```http
POST https://graph.microsoft.com/beta/invitations
Content-type: application/json
Content-length: 551

{
  "invitedUserEmailAddress": "yyy@test.com",
  "inviteRedirectUrl": "https://myapp.contoso.com"
}
```
# <a name="c"></a>[<span data-ttu-id="94a7f-151">C#</span><span class="sxs-lookup"><span data-stu-id="94a7f-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-invitation-post-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="94a7f-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="94a7f-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-invitation-post-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="94a7f-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="94a7f-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-invitation-post-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="94a7f-154">Java</span><span class="sxs-lookup"><span data-stu-id="94a7f-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-invitation-post-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="94a7f-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="94a7f-155">Response</span></span>
<span data-ttu-id="94a7f-156">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94a7f-156">Here is an example of the response.</span></span> <span data-ttu-id="94a7f-157">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="94a7f-157">Note: The response object shown here might be shortened for readability.</span></span>
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
  "inviteRedirectUrl": "https://myapp.contoso.com/",
  "status": "Completed",
  "invitedUser":  [ {  "id": "243b1de4-ad9f-421c-a933-d55305fb165d" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->


