---
author: kevklam
title: Conceder permissão
description: Conceder uma lista de usuários acesso para usar o link especificado
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4dedd3614c043a622ba659bf1986f7d216ac7ac1
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50475174"
---
# <a name="permission-grant"></a><span data-ttu-id="35ec2-103">permission: grant</span><span class="sxs-lookup"><span data-stu-id="35ec2-103">permission: grant</span></span>

<span data-ttu-id="35ec2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35ec2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35ec2-105">Conceda aos usuários acesso a um link representado por uma [permissão][].</span><span class="sxs-lookup"><span data-stu-id="35ec2-105">Grant users access to a link represented by a [permission][].</span></span>

## <a name="permissions"></a><span data-ttu-id="35ec2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="35ec2-106">Permissions</span></span>

<span data-ttu-id="35ec2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="35ec2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="35ec2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="35ec2-109">Permission type</span></span>                   | <span data-ttu-id="35ec2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="35ec2-110">Permissions (from least to most privileged)</span></span>              |
|:----------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="35ec2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="35ec2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="35ec2-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ec2-112">Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="35ec2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="35ec2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="35ec2-114">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="35ec2-114">Not supported</span></span>    |
|<span data-ttu-id="35ec2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="35ec2-115">Application</span></span> | <span data-ttu-id="35ec2-116">Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35ec2-116">Files.ReadWrite.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="35ec2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="35ec2-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /shares/{encoded-sharing-url}/permission/grant
```

## <a name="request-headers"></a><span data-ttu-id="35ec2-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="35ec2-118">Request headers</span></span>

| <span data-ttu-id="35ec2-119">Nome</span><span class="sxs-lookup"><span data-stu-id="35ec2-119">Name</span></span>          | <span data-ttu-id="35ec2-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="35ec2-120">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="35ec2-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="35ec2-121">Authorization</span></span> | <span data-ttu-id="35ec2-122">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="35ec2-122">Bearer \{token\}.</span></span> <span data-ttu-id="35ec2-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="35ec2-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="35ec2-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="35ec2-124">Request body</span></span>

<span data-ttu-id="35ec2-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="35ec2-125">In the request body, provide a JSON object with the following parameters.</span></span>

<!-- { "blockType": "ignored", "scopes": "files.readwrite" } -->

```json
{
  "recipients": [
    { "@odata.type": "microsoft.graph.driveRecipient" }
  ],
  "roles": [ "read | write"]
}
```

| <span data-ttu-id="35ec2-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="35ec2-126">Parameter</span></span>          | <span data-ttu-id="35ec2-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="35ec2-127">Type</span></span>                           | <span data-ttu-id="35ec2-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="35ec2-128">Description</span></span>
|:-------------------|:-------------------------------|:-------------------------
| <span data-ttu-id="35ec2-129">destinatários</span><span class="sxs-lookup"><span data-stu-id="35ec2-129">recipients</span></span>         | <span data-ttu-id="35ec2-130">Coleção([driveRecipient][])</span><span class="sxs-lookup"><span data-stu-id="35ec2-130">Collection([driveRecipient][])</span></span> | <span data-ttu-id="35ec2-131">Uma coleção de destinatários que receberão acesso.</span><span class="sxs-lookup"><span data-stu-id="35ec2-131">A collection of recipients who will receive access.</span></span>
| <span data-ttu-id="35ec2-132">funções</span><span class="sxs-lookup"><span data-stu-id="35ec2-132">roles</span></span>              | <span data-ttu-id="35ec2-133">Collection(String)</span><span class="sxs-lookup"><span data-stu-id="35ec2-133">Collection(String)</span></span>             | <span data-ttu-id="35ec2-134">Se o link for um link de "acesso existente", especificará funções a serem concedidas aos usuários.</span><span class="sxs-lookup"><span data-stu-id="35ec2-134">If the link is an "existing access" link, specifies roles to be granted to the users.</span></span> <span data-ttu-id="35ec2-135">Caso contrário, deverá corresponder à função do link.</span><span class="sxs-lookup"><span data-stu-id="35ec2-135">Otherwise must match the role of the link.</span></span>

<span data-ttu-id="35ec2-136">Para ver uma lista de funções disponíveis, consulte [roles property values](../resources/permission.md#roles-property-values).</span><span class="sxs-lookup"><span data-stu-id="35ec2-136">For a list of available roles, see [roles property values](../resources/permission.md#roles-property-values).</span></span>

## <a name="response"></a><span data-ttu-id="35ec2-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="35ec2-137">Response</span></span>

<span data-ttu-id="35ec2-138">Se tiver êxito, este método retornará um código `200 OK` de resposta e uma coleção [de][] permissões no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="35ec2-138">If successful, this method returns a `200 OK` response code and a [permission][] collection in the response body.</span></span>

<span data-ttu-id="35ec2-139">Uma [permissão][] que representa o link atualizado sempre será retornada no conjunto de resultados sobre o sucesso.</span><span class="sxs-lookup"><span data-stu-id="35ec2-139">A [permission][] representing the updated link will always be returned in the result set on success.</span></span> <span data-ttu-id="35ec2-140">O link atualizado pode ser identificado pela presença de uma faceta 'link' contendo a propriedade 'escopo'.</span><span class="sxs-lookup"><span data-stu-id="35ec2-140">The updated link can be identified by the presence of a 'link' facet containing the 'scope' property.</span></span> <span data-ttu-id="35ec2-141">Em alguns casos, pode ser possível que o link atualizado tenha uma URL diferente do link original, nesse caso, a nova URL deve ser usada.</span><span class="sxs-lookup"><span data-stu-id="35ec2-141">In some cases it may be possible that the updated link has a different URL than the original link, in which case the new URL should be used.</span></span>

<span data-ttu-id="35ec2-142">Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="35ec2-142">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>


## <a name="example"></a><span data-ttu-id="35ec2-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="35ec2-143">Example</span></span>

<span data-ttu-id="35ec2-144">Este exemplo concede aos usuários john@contoso.com e ryan@external.com acesso a um link de compartilhamento sem modificar outras permissões existentes no link.</span><span class="sxs-lookup"><span data-stu-id="35ec2-144">This example grants the users john@contoso.com and ryan@external.com access to a sharing link without modifying other existing permissions on the link.</span></span>

### <a name="request"></a><span data-ttu-id="35ec2-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="35ec2-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="35ec2-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="35ec2-146">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "permission-grant", "scopes": "files.readwrite", "target": "action" } -->

```http
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
# <a name="c"></a>[<span data-ttu-id="35ec2-147">C#</span><span class="sxs-lookup"><span data-stu-id="35ec2-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/permission-grant-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="35ec2-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="35ec2-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/permission-grant-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="35ec2-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="35ec2-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/permission-grant-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="35ec2-150">Java</span><span class="sxs-lookup"><span data-stu-id="35ec2-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/permission-grant-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="35ec2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="35ec2-151">Response</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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

><span data-ttu-id="35ec2-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35ec2-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<span data-ttu-id="35ec2-154">Se o link for um link [de acesso](../resources/permission.md#existing-access-link) existente, permissões adicionais serão retornadas representando o seguinte:</span><span class="sxs-lookup"><span data-stu-id="35ec2-154">If the link is an [existing access](../resources/permission.md#existing-access-link) link, additional permissions will be returned representing the following:</span></span>

- <span data-ttu-id="35ec2-155">Permissões de tipo de usuário que representam destinatários que tiveram acesso concedido com êxito.</span><span class="sxs-lookup"><span data-stu-id="35ec2-155">User-type permissions representing recipients who were successfully granted access.</span></span> <span data-ttu-id="35ec2-156">Eles podem ser identificados pela presença da **propriedade grantedTo.**</span><span class="sxs-lookup"><span data-stu-id="35ec2-156">These can be identified by presence of the **grantedTo** property.</span></span>
- <span data-ttu-id="35ec2-157">Permissões de tipo de link que representam convites que precisam ser enviados a usuários externos não reconhecedos para que eles obtenham acesso.</span><span class="sxs-lookup"><span data-stu-id="35ec2-157">Link-type permissions representing invitations that need to be sent to unrecognized external users for them to gain access.</span></span> <span data-ttu-id="35ec2-158">Eles podem ser identificados pela presença de uma faceta [de](../resources/sharinginvitation.md) convite.</span><span class="sxs-lookup"><span data-stu-id="35ec2-158">These can be identified by the presence of an [invitation](../resources/sharinginvitation.md) facet.</span></span> <span data-ttu-id="35ec2-159">Essas entradas conterão um [link][sharing-link] com a URL do convite e a coleção grantedToIdentities indicará os usuários aos quais o link deve ser enviado.</span><span class="sxs-lookup"><span data-stu-id="35ec2-159">These entries will contain a [link][sharing-link] with the invitation URL, and the grantedToIdentities collection will indicate the users to whom the link should be sent.</span></span>

<!-- { "blockType": "response", "@odata.type": "Collection(microsoft.graph.permission)", "truncated": true } -->

```http
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

><span data-ttu-id="35ec2-160">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="35ec2-160">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="35ec2-161">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="35ec2-161">All the properties will be returned from an actual call.</span></span>



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


