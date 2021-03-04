---
title: Obter objetos de membros
description: " Retorna todos os grupos, unidades administrativas e funções de diretório das quais um usuário, grupo, entidades de serviço ou objeto de diretório é membro. Esta função é transitiva. "
localization_priority: Normal
author: keylimesoda
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 47ad4aa86e41ace7edc9e5b5eb0351557a94a7ae
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50436852"
---
# <a name="get-member-objects"></a><span data-ttu-id="d8bee-104">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="d8bee-104">Get member objects</span></span>

<span data-ttu-id="d8bee-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8bee-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="d8bee-106">Retorna todos os grupos, unidades administrativas e funções de diretório das quais um usuário, grupo, entidades de serviço ou objeto de diretório é membro.</span><span class="sxs-lookup"><span data-stu-id="d8bee-106">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="d8bee-107">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="d8bee-107">This function is transitive.</span></span> 
 > <span data-ttu-id="d8bee-108">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="d8bee-108">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="d8bee-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="d8bee-109">Permissions</span></span>
<span data-ttu-id="d8bee-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d8bee-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d8bee-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d8bee-112">Permission type</span></span>      | <span data-ttu-id="d8bee-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d8bee-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d8bee-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d8bee-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d8bee-115">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8bee-115">Directory.Read.All</span></span>    |
|<span data-ttu-id="d8bee-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d8bee-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d8bee-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d8bee-117">Not supported.</span></span>    |
|<span data-ttu-id="d8bee-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8bee-118">Application</span></span> | <span data-ttu-id="d8bee-119">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="d8bee-119">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d8bee-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bee-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="d8bee-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bee-121">Request headers</span></span>
| <span data-ttu-id="d8bee-122">Nome</span><span class="sxs-lookup"><span data-stu-id="d8bee-122">Name</span></span>       | <span data-ttu-id="d8bee-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8bee-123">Type</span></span> | <span data-ttu-id="d8bee-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bee-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d8bee-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d8bee-125">Authorization</span></span>  | <span data-ttu-id="d8bee-126">string</span><span class="sxs-lookup"><span data-stu-id="d8bee-126">string</span></span>  | <span data-ttu-id="d8bee-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d8bee-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d8bee-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d8bee-129">Content-Type</span></span>  | <span data-ttu-id="d8bee-130">application/json</span><span class="sxs-lookup"><span data-stu-id="d8bee-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d8bee-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bee-131">Request body</span></span>
<span data-ttu-id="d8bee-132">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d8bee-132">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="d8bee-133">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="d8bee-133">Parameter</span></span>    | <span data-ttu-id="d8bee-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8bee-134">Type</span></span>   |<span data-ttu-id="d8bee-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8bee-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d8bee-136">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="d8bee-136">securityEnabledOnly</span></span>|<span data-ttu-id="d8bee-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="d8bee-137">Boolean</span></span>| <span data-ttu-id="d8bee-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="d8bee-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="d8bee-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bee-140">Response</span></span>

<span data-ttu-id="d8bee-141">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d8bee-141">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8bee-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d8bee-142">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d8bee-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d8bee-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d8bee-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="d8bee-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="d8bee-145">C#</span><span class="sxs-lookup"><span data-stu-id="d8bee-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/directoryobject-getmemberobjects-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d8bee-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d8bee-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/directoryobject-getmemberobjects-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d8bee-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d8bee-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/directoryobject-getmemberobjects-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d8bee-148">Java</span><span class="sxs-lookup"><span data-stu-id="d8bee-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/directoryobject-getmemberobjects-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="d8bee-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="d8bee-149">Response</span></span>
<span data-ttu-id="d8bee-p106">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d8bee-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


