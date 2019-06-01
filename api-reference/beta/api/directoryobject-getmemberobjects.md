---
title: Obter objetos de membros
description: " Retorna todos os grupos, unidades administrativas e funções de diretório de que um usuário, grupo, entidades de serviço ou objeto de diretório é membro. Esta função é transitiva. "
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7dea7deaa7674fd64270daae2c13d0ba9203a618
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656066"
---
# <a name="get-member-objects"></a><span data-ttu-id="a6b3a-104">Obter objetos de membros</span><span class="sxs-lookup"><span data-stu-id="a6b3a-104">Get member objects</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

 <span data-ttu-id="a6b3a-105">Retorna todos os grupos, unidades administrativas e funções de diretório de que um usuário, grupo, entidades de serviço ou objeto de diretório é membro.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-105">Returns all the groups, administrative units and directory roles that a user, group, service principals or directory object is a member of.</span></span> <span data-ttu-id="a6b3a-106">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-106">This function is transitive.</span></span> 
 > <span data-ttu-id="a6b3a-107">Observação: Somente usuários podem ser membros de funções de diretório.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-107">Note: Only users can be members of directory roles.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6b3a-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a6b3a-108">Permissions</span></span>
<span data-ttu-id="a6b3a-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6b3a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a6b3a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6b3a-111">Permission type</span></span>      | <span data-ttu-id="a6b3a-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6b3a-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a6b3a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6b3a-113">Delegated (work or school account)</span></span> | <span data-ttu-id="a6b3a-114">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6b3a-114">Directory.Read.All</span></span>    |
|<span data-ttu-id="a6b3a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6b3a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6b3a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-116">Not supported.</span></span>    |
|<span data-ttu-id="a6b3a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6b3a-117">Application</span></span> | <span data-ttu-id="a6b3a-118">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="a6b3a-118">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6b3a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6b3a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberObjects
POST /users/{id | userPrincipalName}/getMemberObjects
POST /groups/{id}/getMemberObjects
POST /servicePrincipals/{id}/getMemberObjects
POST /directoryObjects/{id}/getMemberObjects

```
## <a name="request-headers"></a><span data-ttu-id="a6b3a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b3a-120">Request headers</span></span>
| <span data-ttu-id="a6b3a-121">Nome</span><span class="sxs-lookup"><span data-stu-id="a6b3a-121">Name</span></span>       | <span data-ttu-id="a6b3a-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6b3a-122">Type</span></span> | <span data-ttu-id="a6b3a-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b3a-123">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="a6b3a-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6b3a-124">Authorization</span></span>  | <span data-ttu-id="a6b3a-125">string</span><span class="sxs-lookup"><span data-stu-id="a6b3a-125">string</span></span>  | <span data-ttu-id="a6b3a-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6b3a-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a6b3a-128">Content-Type</span></span>  | <span data-ttu-id="a6b3a-129">application/json</span><span class="sxs-lookup"><span data-stu-id="a6b3a-129">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a6b3a-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b3a-130">Request body</span></span>
<span data-ttu-id="a6b3a-131">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-131">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="a6b3a-132">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a6b3a-132">Parameter</span></span>    | <span data-ttu-id="a6b3a-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6b3a-133">Type</span></span>   |<span data-ttu-id="a6b3a-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6b3a-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6b3a-135">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="a6b3a-135">securityEnabledOnly</span></span>|<span data-ttu-id="a6b3a-136">Booliano</span><span class="sxs-lookup"><span data-stu-id="a6b3a-136">Boolean</span></span>| <span data-ttu-id="a6b3a-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="a6b3a-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b3a-139">Response</span></span>

<span data-ttu-id="a6b3a-140">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-140">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6b3a-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6b3a-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a6b3a-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6b3a-142">Request</span></span>
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

##### <a name="response"></a><span data-ttu-id="a6b3a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6b3a-143">Response</span></span>
<span data-ttu-id="a6b3a-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6b3a-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="a6b3a-146">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="a6b3a-146">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="a6b3a-147">C#</span><span class="sxs-lookup"><span data-stu-id="a6b3a-147">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a6b3a-148">Javascript</span><span class="sxs-lookup"><span data-stu-id="a6b3a-148">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getmemberobjects-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-getmemberobjects.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
