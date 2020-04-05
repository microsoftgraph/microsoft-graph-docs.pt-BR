---
author: kevklam
ms.author: kevinlam
title: Conceder permissão
description: Conceder a uma lista de usuários acesso para usar o link especificado
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 901b5c7b7e67b0d45a0d4891b239fa950d864119
ms.sourcegitcommit: 6db0b7a473594653dda332ce7da45ea2ad90772b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/04/2020
ms.locfileid: "43146391"
---
# <a name="permission-grant"></a><span data-ttu-id="68fd9-103">permissão: Grant</span><span class="sxs-lookup"><span data-stu-id="68fd9-103">permission: grant</span></span>

<span data-ttu-id="68fd9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68fd9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="68fd9-105">Conceder aos usuários acesso a um link representado por uma [permissão][].</span><span class="sxs-lookup"><span data-stu-id="68fd9-105">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="68fd9-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="68fd9-106">Permissions</span></span>

<span data-ttu-id="68fd9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="68fd9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="68fd9-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="68fd9-109">Permission type</span></span>                   | <span data-ttu-id="68fd9-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="68fd9-110">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="68fd9-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="68fd9-111">Delegated (work or school account)</span></span> | <span data-ttu-id="68fd9-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68fd9-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="68fd9-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="68fd9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68fd9-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="68fd9-114">Not supported</span></span>    |
|<span data-ttu-id="68fd9-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="68fd9-115">Application</span></span> | <span data-ttu-id="68fd9-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68fd9-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68fd9-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="68fd9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="68fd9-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="68fd9-118">Request headers</span></span>

| <span data-ttu-id="68fd9-119">Nome</span><span class="sxs-lookup"><span data-stu-id="68fd9-119">Name</span></span>          | <span data-ttu-id="68fd9-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="68fd9-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="68fd9-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="68fd9-121">Authorization</span></span> | <span data-ttu-id="68fd9-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="68fd9-122">Bearer \{token\}.</span></span> <span data-ttu-id="68fd9-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="68fd9-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68fd9-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="68fd9-124">Request body</span></span>

<span data-ttu-id="68fd9-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="68fd9-125">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="68fd9-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="68fd9-126">Parameter</span></span>          | <span data-ttu-id="68fd9-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="68fd9-127">Type</span></span>                           | <span data-ttu-id="68fd9-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="68fd9-128">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="68fd9-129">destinatários</span><span class="sxs-lookup"><span data-stu-id="68fd9-129">recipients</span></span>         | <span data-ttu-id="68fd9-130">Coleção ([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="68fd9-130">Collection([driveRecipient][])</span></span> | <span data-ttu-id="68fd9-131">Uma coleção de destinatários que receberão acesso.</span><span class="sxs-lookup"><span data-stu-id="68fd9-131">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="68fd9-132">funções</span><span class="sxs-lookup"><span data-stu-id="68fd9-132">roles</span></span>              | <span data-ttu-id="68fd9-133">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="68fd9-133">Collection(String)</span></span>             | <span data-ttu-id="68fd9-134">Se o link for um link "acesso existente", especifica as funções a serem concedidas aos usuários.</span><span class="sxs-lookup"><span data-stu-id="68fd9-134">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="68fd9-135">Caso contrário, deve corresponder à função do link.</span><span class="sxs-lookup"><span data-stu-id="68fd9-135">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="68fd9-136">Para obter uma lista de funções disponíveis, consulte [funções valores de propriedade](../resources/permission.md#roles-property-values).</span><span class="sxs-lookup"><span data-stu-id="68fd9-136">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="response"></a><span data-ttu-id="68fd9-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="68fd9-137">Response</span></span>

<span data-ttu-id="68fd9-138">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de [permissões][] no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="68fd9-138">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="68fd9-139">Uma [permissão][] que representa o link atualizado sempre será retornada no conjunto de resultados no êxito.</span><span class="sxs-lookup"><span data-stu-id="68fd9-139">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="68fd9-140">O link updated pode ser identificado pela presença de uma faceta ' link ' que contém a propriedade ' Scope '.</span><span class="sxs-lookup"><span data-stu-id="68fd9-140">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="68fd9-141">Em alguns casos, pode ser possível que o link atualizado tenha uma URL diferente da conexão original, caso em que a nova URL deve ser usada.</span><span class="sxs-lookup"><span data-stu-id="68fd9-141">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="68fd9-142">Leia o tópico [respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="68fd9-142">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="68fd9-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="68fd9-143">Example</span></span>

<span data-ttu-id="68fd9-144">Este exemplo concede aos usuários john@contoso.com e ryan@external.com acesso a um link de compartilhamento sem modificar outras permissões existentes no link.</span><span class="sxs-lookup"><span data-stu-id="68fd9-144">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="68fd9-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="68fd9-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="68fd9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="68fd9-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

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
# <a name="c"></a>[<span data-ttu-id="68fd9-147">C#</span><span class="sxs-lookup"><span data-stu-id="68fd9-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="68fd9-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="68fd9-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="68fd9-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="68fd9-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="68fd9-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="68fd9-150">Response</span></span>

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

><span data-ttu-id="68fd9-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68fd9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="68fd9-153">Se o link for um link de [acesso existente](../resources/permission.md#existing-access-link) , serão retornadas permissões adicionais representando o seguinte:</span><span class="sxs-lookup"><span data-stu-id="68fd9-153">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="68fd9-154">Permissões de tipo de usuário que representam destinatários que receberam o acesso com êxito.</span><span class="sxs-lookup"><span data-stu-id="68fd9-154">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="68fd9-155">Eles podem ser identificados por presença da propriedade **concedidoto** .</span><span class="sxs-lookup"><span data-stu-id="68fd9-155">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="68fd9-156">Permissões de tipo de link que representam convites que precisam ser enviados a usuários externos não reconhecidos para que eles tenham acesso.</span><span class="sxs-lookup"><span data-stu-id="68fd9-156">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="68fd9-157">Eles podem ser identificados pela presença de uma faceta de [convite](../resources/sharinginvitation.md) .</span><span class="sxs-lookup"><span data-stu-id="68fd9-157">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="68fd9-158">Essas entradas conterá um [link][sharing-link] com a URL do convite, e a coleção grantedToIdentities indicará os usuários para os quais o link deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="68fd9-158">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

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

><span data-ttu-id="68fd9-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="68fd9-159">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="68fd9-160">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="68fd9-160">All the properties will be returned from an actual call.</span></span>



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
