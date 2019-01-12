---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Enviar um convite para acessar um item
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: f428fe7b8a61fc158d4175f50fb287760e25d524
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27945973"
---
# <a name="send-a-sharing-invitation"></a><span data-ttu-id="b1b9c-102">Enviar um convite de compartilhamento</span><span class="sxs-lookup"><span data-stu-id="b1b9c-102">Send a sharing invitation</span></span>

> <span data-ttu-id="b1b9c-103">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b1b9c-104">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b1b9c-p102">Envia um convite de compartilhamento para um **DriveItem**. Um convite de compartilhamento fornece permissões para os destinatários e, opcionalmente, envia um email aos destinatários para notificá-los de que o item foi compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-p102">Sends a sharing invitation for a **DriveItem**. A sharing invitation provides permissions to the recipients and optionally sends an email to the recipients to notify them the item was shared.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1b9c-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="b1b9c-107">Permissions</span></span>

<span data-ttu-id="b1b9c-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b1b9c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1b9c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b1b9c-110">Permission type</span></span>      | <span data-ttu-id="b1b9c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="b1b9c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1b9c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b1b9c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b1b9c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b9c-113">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1b9c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b1b9c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1b9c-115">Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b9c-115">Files.ReadWrite, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="b1b9c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b1b9c-116">Application</span></span> | <span data-ttu-id="b1b9c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1b9c-117">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1b9c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1b9c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{drive-id}/items/{item-id}/invite
POST /groups/{group-id}/drive/items/{item-id}/invite
POST /me/drive/items/{item-id}/invite
POST /sites/{siteId}/drive/items/{itemId}/invite
POST /users/{userId}/drive/items/{itemId}/invite
```

## <a name="request-body"></a><span data-ttu-id="b1b9c-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b1b9c-119">Request body</span></span>

<span data-ttu-id="b1b9c-120">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-120">In the request body, provide a JSON object with the following parameters.</span></span>

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

| <span data-ttu-id="b1b9c-121">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="b1b9c-121">Parameter</span></span>        | <span data-ttu-id="b1b9c-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="b1b9c-122">Type</span></span>                                            | <span data-ttu-id="b1b9c-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="b1b9c-123">Description</span></span>                                                                                                |
|:-----------------|:------------------------------------------------|:-----------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="b1b9c-124">destinatários</span><span class="sxs-lookup"><span data-stu-id="b1b9c-124">recipients</span></span>       | <span data-ttu-id="b1b9c-125">Collection([DriveRecipient](../resources/driverecipient.md))</span><span class="sxs-lookup"><span data-stu-id="b1b9c-125">Collection([DriveRecipient](../resources/driverecipient.md))</span></span> | <span data-ttu-id="b1b9c-126">Uma coleção dos destinatários que receberão o acesso e o convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-126">A collection of recipients who will receive access and the sharing invitation.</span></span>                                            |
| <span data-ttu-id="b1b9c-127">mensagem</span><span class="sxs-lookup"><span data-stu-id="b1b9c-127">message</span></span>          | <span data-ttu-id="b1b9c-128">String</span><span class="sxs-lookup"><span data-stu-id="b1b9c-128">String</span></span>                                          | <span data-ttu-id="b1b9c-p104">Uma mensagem de texto sem formatação que está incluída no convite de compartilhamento. Comprimento máximo de 2000 caracteres.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-p104">A plain text formatted message that is included in the sharing invitation. Maximum length 2000 characters.</span></span> |
| <span data-ttu-id="b1b9c-131">requireSignIn</span><span class="sxs-lookup"><span data-stu-id="b1b9c-131">requireSignIn</span></span>    | <span data-ttu-id="b1b9c-132">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1b9c-132">Boolean</span></span>                                         | <span data-ttu-id="b1b9c-133">Especifica onde o destinatário do convite precisa entrar para exibir o item compartilhado.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-133">Specifies where the recipient of the invitation is required to sign-in to view the shared item.</span></span>            |
| <span data-ttu-id="b1b9c-134">sendInvitation</span><span class="sxs-lookup"><span data-stu-id="b1b9c-134">sendInvitation</span></span>   | <span data-ttu-id="b1b9c-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="b1b9c-135">Boolean</span></span>                                         | <span data-ttu-id="b1b9c-136">Especifica se um email ou uma postagem é gerado (false) ou se a permissão é recém-criada (true).</span><span class="sxs-lookup"><span data-stu-id="b1b9c-136">Specifies if an email or post is generated (false) or if the permission is just created (true).</span></span>            |
| <span data-ttu-id="b1b9c-137">funções</span><span class="sxs-lookup"><span data-stu-id="b1b9c-137">roles</span></span>            | <span data-ttu-id="b1b9c-138">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="b1b9c-138">Collection(String)</span></span>                              | <span data-ttu-id="b1b9c-139">Especifique as funções que são concedidas aos destinatários do convite de compartilhamento.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-139">Specify the roles that are be granted to the recipients of the sharing invitation.</span></span>                         |

## <a name="example"></a><span data-ttu-id="b1b9c-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b1b9c-140">Example</span></span>

<span data-ttu-id="b1b9c-141">Este exemplo envia um convite de compartilhamento para um usuário com o endereço de email "ryan@contoso.org" com uma mensagem sobre um arquivo no qual ele está colaborando.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-141">This example sends a sharing invitation to a user with email address "ryan@contoso.org" with a message about a file being collaborated on.</span></span>
<span data-ttu-id="b1b9c-142">O convite concede acesso de leitura e gravação ao arquivo para Ryan.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-142">The invitation grants Ryan read-write access to the file.</span></span>

### <a name="http-request"></a><span data-ttu-id="b1b9c-143">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b1b9c-143">HTTP Request</span></span>

<span data-ttu-id="b1b9c-144">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto de coleção [permission](../resources/permission.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-144">If successful, this method returns `200 OK` response code and [permission](../resources/permission.md) collection object in the response body.</span></span>

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

### <a name="response"></a><span data-ttu-id="b1b9c-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="b1b9c-145">Response</span></span>

<span data-ttu-id="b1b9c-146">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-146">Here is an example of the response.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="b1b9c-147">Comentários</span><span class="sxs-lookup"><span data-stu-id="b1b9c-147">Remarks</span></span>

* <span data-ttu-id="b1b9c-148">[Drives](../resources/drive.md) com **driveType** de `personal` (OneDrive Pessoal) não podem criar ou alterar as permissões no DriveItem raiz.</span><span class="sxs-lookup"><span data-stu-id="b1b9c-148">[Drives](../resources/drive.md) with a **driveType** of `personal` (OneDrive personal) cannot create or modify permissions on the root DriveItem.</span></span>
* <span data-ttu-id="b1b9c-149">Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="b1b9c-149">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="error-responses"></a><span data-ttu-id="b1b9c-150">Respostas de erro</span><span class="sxs-lookup"><span data-stu-id="b1b9c-150">Error Responses</span></span>

<span data-ttu-id="b1b9c-151">Saiba mais sobre como os erros são retornados em [Respostas de erro][error-response].</span><span class="sxs-lookup"><span data-stu-id="b1b9c-151">Read the [Error Responses][error-response] topic for more information about how errors are returned.</span></span>


[error-response]: /graph/errors

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
