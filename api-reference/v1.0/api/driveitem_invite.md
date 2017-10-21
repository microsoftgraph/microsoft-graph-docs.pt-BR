---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
ms.openlocfilehash: 5be2060c190434c4b9d587d20fe68d69786b3aa5
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/28/2017
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="a3b80-102">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="a3b80-102">Send a sharing invitation</span></span>

<span data-ttu-id="a3b80-p101">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a3b80-p101">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3b80-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="a3b80-105">Permissions</span></span>

<span data-ttu-id="a3b80-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a3b80-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a3b80-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a3b80-108">Permission type</span></span>      | <span data-ttu-id="a3b80-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a3b80-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3b80-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a3b80-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a3b80-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b80-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3b80-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a3b80-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a3b80-113">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b80-113">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a3b80-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a3b80-114">Application</span></span> | <span data-ttu-id="a3b80-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3b80-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3b80-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b80-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="a3b80-117">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a3b80-117">Request body</span></span>

<span data-ttu-id="a3b80-118">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a3b80-118">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite" } -->

```json
{
  "requireSignIn": false,
  "sendInvitation": false,
  "roles": [ "read | write"],
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" },
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "message": "string"
}
```

| <span data-ttu-id="a3b80-119">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a3b80-119">Parameter</span></span>        | <span data-ttu-id="a3b80-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="a3b80-120">Type</span></span>                                            | <span data-ttu-id="a3b80-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="a3b80-121">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="a3b80-122">destinatários</span><span class="sxs-lookup"><span data-stu-id="a3b80-122">recipients</span></span>       | <span data-ttu-id="a3b80-123">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="a3b80-123">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="a3b80-124">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="a3b80-124">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="a3b80-125">mensagem</span><span class="sxs-lookup"><span data-stu-id="a3b80-125">message</span></span>          | <span data-ttu-id="a3b80-126">String</span><span class="sxs-lookup"><span data-stu-id="a3b80-126">String</span></span>                                          | <span data-ttu-id="a3b80-p103">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="a3b80-p103">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="a3b80-129">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="a3b80-129">requireSignIn</span></span>    | <span data-ttu-id="a3b80-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="a3b80-130">Boolean</span></span>                                         | <span data-ttu-id="a3b80-131">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="a3b80-131">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="a3b80-132">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="a3b80-132">sendInvitation</span></span>   | <span data-ttu-id="a3b80-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="a3b80-133">Boolean</span></span>                                         | <span data-ttu-id="a3b80-134">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="a3b80-134">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="a3b80-135">funções</span><span class="sxs-lookup"><span data-stu-id="a3b80-135">roles</span></span>            | <span data-ttu-id="a3b80-136">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="a3b80-136">Collection(String)</span></span>                              | <span data-ttu-id="a3b80-137">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="a3b80-137">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="a3b80-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a3b80-138">Example</span></span>

<span data-ttu-id="a3b80-139">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.org" com uma mensagem sobre um arquivo no qual ele está colaborando.</span><span class="sxs-lookup"><span data-stu-id="a3b80-139">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="a3b80-140">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="a3b80-140">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="a3b80-141">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a3b80-141">HTTP Request</span></span>

<span data-ttu-id="a3b80-142">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3b80-142">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

<!-- { "blockType": "request", "name": "send-sharing-invite", "@odata.type": "microsoft.graph.inviteParameters", "scopes": "files.readwrite", "target": "action" } -->

```http
POST /me/drive/items/{item-id}/invite
Content-type: application/json

{
  "recipients": [
    {
      "email": "ryan@contoso.org"
    }
  ],
  "message": "Here's the file that we're collaborating on.",
  "requireSignIn": true,
  "sendInvitation": true,
  "roles": [ "write" ]
}
```

### <a name="response"></a><span data-ttu-id="a3b80-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a3b80-143">Response</span></span>

<span data-ttu-id="a3b80-144">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a3b80-144">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "grantedTo": {
        "user": {
          "displayName": "Ryan Gregg",
          "id": "42F177F1-22C0-4BE3-900D-4507125C5C20"
        }
      },
      "id": "CCFC7CA3-7A19-4D57-8CEF-149DB9DDFA62",
      "invitation": {
        "email": "ryan@contoso.com",
        "signInRequired": true
      },
      "roles": [ "write" ]
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="a3b80-145">Comentários</span><span class="sxs-lookup"><span data-stu-id="a3b80-145">Remarks</span></span>

* <span data-ttu-id="a3b80-146">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="a3b80-146">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive Personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="a3b80-147">Para obter uma lista das funções disponíveis, confira [Funções de enumeração](../resources/permission.md#roles-enumeration).</span><span class="sxs-lookup"><span data-stu-id="a3b80-147">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration).</span></span>

## <a name="error-responses"></a><span data-ttu-id="a3b80-148">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="a3b80-148">Error Responses</span></span>

<span data-ttu-id="a3b80-149">Veja mais informações sobre como os erros são retornados no tópico [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="a3b80-149">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: ../../../concepts/errors.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
