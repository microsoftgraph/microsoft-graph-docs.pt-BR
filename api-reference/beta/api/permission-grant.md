---
author: kevklam
ms.author: kevinlam
title: Conceder permissão
description: Conceder a uma lista de usuários acesso para usar o link especificado
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: ca427092b169b0a7e9ea13697ee0252c354f3246
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35992448"
---
# <a name="grant-permission"></a><span data-ttu-id="bdd43-103">Conceder permissão</span><span class="sxs-lookup"><span data-stu-id="bdd43-103">Grant permission</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bdd43-104">Conceder aos usuários acesso a um link representado por uma [permissão][].</span><span class="sxs-lookup"><span data-stu-id="bdd43-104">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="bdd43-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="bdd43-105">Permissions</span></span>

<span data-ttu-id="bdd43-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bdd43-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdd43-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bdd43-108">Permission type</span></span>                   | <span data-ttu-id="bdd43-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bdd43-109">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="bdd43-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bdd43-110">Delegated (work or school account)</span></span> | <span data-ttu-id="bdd43-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd43-111">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="bdd43-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bdd43-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdd43-113">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="bdd43-113">Not supported</span></span>    |
|<span data-ttu-id="bdd43-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bdd43-114">Application</span></span> | <span data-ttu-id="bdd43-115">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdd43-115">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bdd43-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd43-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="bdd43-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd43-117">Request headers</span></span>

| <span data-ttu-id="bdd43-118">Nome</span><span class="sxs-lookup"><span data-stu-id="bdd43-118">Name</span></span>          | <span data-ttu-id="bdd43-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd43-119">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="bdd43-120">Autorização</span><span class="sxs-lookup"><span data-stu-id="bdd43-120">Authorization</span></span> | <span data-ttu-id="bdd43-121">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="bdd43-121">Bearer \{token\}.</span></span> <span data-ttu-id="bdd43-122">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bdd43-122">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="bdd43-123">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd43-123">Request body</span></span>

<span data-ttu-id="bdd43-124">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bdd43-124">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="bdd43-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="bdd43-125">Parameter</span></span>          | <span data-ttu-id="bdd43-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="bdd43-126">Type</span></span>                           | <span data-ttu-id="bdd43-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="bdd43-127">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="bdd43-128">recipients</span><span class="sxs-lookup"><span data-stu-id="bdd43-128">recipients</span></span>         | <span data-ttu-id="bdd43-129">Coleção ([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="bdd43-129">Collection([driveRecipient][])</span></span> | <span data-ttu-id="bdd43-130">Uma coleção de destinatários que receberão acesso.</span><span class="sxs-lookup"><span data-stu-id="bdd43-130">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="bdd43-131">funções</span><span class="sxs-lookup"><span data-stu-id="bdd43-131">roles</span></span>              | <span data-ttu-id="bdd43-132">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="bdd43-132">Collection(String)</span></span>             | <span data-ttu-id="bdd43-133">Se o link for um link "acesso existente", especifica as funções a serem concedidas aos usuários.</span><span class="sxs-lookup"><span data-stu-id="bdd43-133">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="bdd43-134">Caso contrário, deve corresponder à função do link.</span><span class="sxs-lookup"><span data-stu-id="bdd43-134">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="bdd43-135">Para obter uma lista das funções disponíveis, consulte [Funções de enumeração](../resources/permission.md#roles-enumeration-values).</span><span class="sxs-lookup"><span data-stu-id="bdd43-135">For a list of available roles, see [Roles enumeration](../resources/permission.md#roles-enumeration-values).</span></span>

## <a name="response"></a><span data-ttu-id="bdd43-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd43-136">Response</span></span>

<span data-ttu-id="bdd43-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [permissões][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bdd43-137">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="bdd43-138">Uma [permissão][] que representa o link atualizado sempre será retornada no conjunto de resultados no êxito.</span><span class="sxs-lookup"><span data-stu-id="bdd43-138">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="bdd43-139">O link updated pode ser identificado pela presença de uma faceta ' link ' que contém a propriedade ' Scope '.</span><span class="sxs-lookup"><span data-stu-id="bdd43-139">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="bdd43-140">Em alguns casos, pode ser possível que o link atualizado tenha uma URL diferente da conexão original, caso em que a nova URL deve ser usada.</span><span class="sxs-lookup"><span data-stu-id="bdd43-140">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="bdd43-141">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="bdd43-141">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="bdd43-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bdd43-142">Example</span></span>

<span data-ttu-id="bdd43-143">Este exemplo concede aos usuários john@contoso.com e ryan@external.com acesso a um link de compartilhamento sem modificar outras permissões existentes no link.</span><span class="sxs-lookup"><span data-stu-id="bdd43-143">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="bdd43-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bdd43-144">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="bdd43-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdd43-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "send-sharing-invite", "scopes": "files.readwrite", "target": "action" } -->

```json
POST https://graph.microsoft.com/beta/shares/{encoded-sharing-url}/permission/grant
Content-type: application/json

{
  "recipients": [
    {
      "email": "john@contoso.com"
    },
    {
      "email": "ryan@external.com"
    }
  ],
  "roles": ["read"]
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="bdd43-146">C#</span><span class="sxs-lookup"><span data-stu-id="bdd43-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/send-sharing-invite-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdd43-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="bdd43-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/send-sharing-invite-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdd43-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="bdd43-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/send-sharing-invite-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bdd43-149">Java</span><span class="sxs-lookup"><span data-stu-id="bdd43-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/send-sharing-invite-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="bdd43-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="bdd43-150">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "5fab944a-47ec-48d0-a9b5-5178a926d00f",
      "link": {
        "preventsDownload": false,
        "scope": "users",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/design/EZexPoDjW4dMtKFUfAl6BK4BvIUuss52hLYzihBfx-PD6Q"
      },
      "roles": [
        "read"
      ]
    }
  ]
}
```

><span data-ttu-id="bdd43-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdd43-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="bdd43-153">Se o link for um link de [acesso existente](../resources/permission.md#existing-access-link) , serão retornadas permissões adicionais representando o seguinte:</span><span class="sxs-lookup"><span data-stu-id="bdd43-153">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="bdd43-154">Permissões de tipo de usuário que representam destinatários que receberam o acesso com êxito.</span><span class="sxs-lookup"><span data-stu-id="bdd43-154">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="bdd43-155">Eles podem ser identificados por presença da propriedade **concedidoto** .</span><span class="sxs-lookup"><span data-stu-id="bdd43-155">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="bdd43-156">Permissões de tipo de link que representam convites que precisam ser enviados a usuários externos não reconhecidos para que eles tenham acesso.</span><span class="sxs-lookup"><span data-stu-id="bdd43-156">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="bdd43-157">Eles podem ser identificados pela presença de uma faceta de [convite](../resources/sharinginvitation.md) .</span><span class="sxs-lookup"><span data-stu-id="bdd43-157">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="bdd43-158">Essas entradas conterá um [link][sharing-link] com a URL do convite, e a coleção grantedToIdentities indicará os usuários para os quais o link deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="bdd43-158">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```json
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "hasPassword": false,
      "id": "00000000-0000-0000-0000-000000000000",
      "link": {
        "preventsDownload": false,
        "scope": "existingAccess",
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/teams/design/shareddocs/Document.docx"
      },
      "roles": [
        "read"
      ]
    },
    {
      "grantedTo": {
        "user": {
          "displayName": "John Smith",
          "email": "john@contoso.com",
          "id": "47aecee2-d061-4730-8ecb-4c61360441ae"
        }
      },
      "id": "aTowIy5mfG1lbWJlcnNoaXB8bGltaXRlZDJAa2xhbW9kYi5vbm1pY3Jvc29mdC5jb20",
      "roles": [
        "read"
      ]
    },
    {
      "grantedToIdentities": [
        {
          "user": {
            "email": "ryan@external.com"
          }
        }
      ],
      "invitation": {
        "signInRequired": true
      },
      "roles": [
        "read"
      ],
      "link": {
        "type": "view",
        "webUrl": "https://contoso.sharepoint.com/:t:/g/teams/design/EZexPoDjW4dMtKFUfAl6BK4Bw_F7gFH63O310A7lDtK0mQ"
      }
    }
  ]
}

```

><span data-ttu-id="bdd43-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="bdd43-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="bdd43-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bdd43-160">All the properties will be returned from an actual call.</span></span>



[driveRecipient]: ../resources/driverecipient.md
[error-response]: /graph/errors
[permissão]: ../resources/permission.md
[permission]: ../resources/permission.md
[sharing-link]: ../resources/sharinglink.md

<!-- {
  "type": "#page.annotation",
  "description": "Add permissions to an item and optionally send a sharing notification.",
  "keywords": "retrieve,item,metadata",
  "section": "documentation",
  "tocPath": "Sharing/Add permissions"
} -->
