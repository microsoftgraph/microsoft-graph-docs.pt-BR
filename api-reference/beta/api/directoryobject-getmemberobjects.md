---
title: Obter objetos de membros
description: " Retorna todos os grupos, unidades administrativas e funções de diretório de que um usuário, grupo, entidades de serviço ou objeto de diretório é membro. Esta função é transitiva. "
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ee0db6cdaac92d722c2cfab21104eae5e3a09581
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/15/2019
ms.locfileid: "36417379"
---
# <a name="get-member-objects"></a><span data-ttu-id="6788b-104">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="6788b-104">Get member objects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="6788b-105">Retorna todos os grupos, unidades administrativas e funções de diretório de que um usuário, grupo, entidades de serviço ou objeto de diretório é membro.</span><span class="sxs-lookup"><span data-stu-id="6788b-105">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="6788b-106">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="6788b-106">This function is transitive.</span></span> 
 > <span data-ttu-id="6788b-107">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="6788b-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="6788b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="6788b-108">Permissions</span></span>
<span data-ttu-id="6788b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6788b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6788b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6788b-111">Permission type</span></span>      | <span data-ttu-id="6788b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6788b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6788b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6788b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="6788b-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6788b-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="6788b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6788b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6788b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6788b-116">Not supported.</span></span>    |
|<span data-ttu-id="6788b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6788b-117">Application</span></span> | <span data-ttu-id="6788b-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6788b-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6788b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6788b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="6788b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6788b-120">Request headers</span></span>
| <span data-ttu-id="6788b-121">Nome</span><span class="sxs-lookup"><span data-stu-id="6788b-121">Name</span></span>       | <span data-ttu-id="6788b-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="6788b-122">Type</span></span> | <span data-ttu-id="6788b-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="6788b-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6788b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="6788b-124">Authorization</span></span>  | <span data-ttu-id="6788b-125">string</span><span class="sxs-lookup"><span data-stu-id="6788b-125">string</span></span>  | <span data-ttu-id="6788b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6788b-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6788b-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6788b-128">Content-Type</span></span>  | <span data-ttu-id="6788b-129">application/json</span><span class="sxs-lookup"><span data-stu-id="6788b-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6788b-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6788b-130">Request body</span></span>
<span data-ttu-id="6788b-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6788b-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="6788b-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="6788b-132">Parameter</span></span>    | <span data-ttu-id="6788b-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="6788b-133">Type</span></span>   |<span data-ttu-id="6788b-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="6788b-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6788b-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="6788b-135">securityEnabledOnly</span></span>|<span data-ttu-id="6788b-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="6788b-136">Boolean</span></span>| <span data-ttu-id="6788b-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="6788b-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="6788b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6788b-139">Response</span></span>

<span data-ttu-id="6788b-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6788b-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6788b-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6788b-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="6788b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6788b-142">Request</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="6788b-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="6788b-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "directoryobject_getmemberobjects"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberObjects
Content-type: application/json

{
  "securityEnabledOnly": true
}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="6788b-144">C#</span><span class="sxs-lookup"><span data-stu-id="6788b-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="6788b-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6788b-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="6788b-146">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="6788b-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="6788b-147">Resposta</span><span class="sxs-lookup"><span data-stu-id="6788b-147">Response</span></span>
<span data-ttu-id="6788b-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6788b-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "string",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "c9ee2d50-9e8a-4352-b97c-4c2c99557c22",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
