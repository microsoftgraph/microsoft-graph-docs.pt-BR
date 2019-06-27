---
title: Obter grupos de membros
description: Retornar todos os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro. Esta função é transitiva.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: cc893a7d45adaf3b22c4bba9c85daf9b3ca523c8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260757"
---
# <a name="get-member-groups"></a><span data-ttu-id="f5153-104">Obter grupos de membros</span><span class="sxs-lookup"><span data-stu-id="f5153-104">Get member groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5153-105">Retornar todos os grupos dos quais o usuário, grupo, entidade de serviço ou objeto de diretório especificado é um membro.</span><span class="sxs-lookup"><span data-stu-id="f5153-105">Return all the groups that the specified user, group, service principal or directory object is a member of.</span></span> <span data-ttu-id="f5153-106">Esta função é transitiva.</span><span class="sxs-lookup"><span data-stu-id="f5153-106">This function is transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="f5153-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="f5153-107">Permissions</span></span>
<span data-ttu-id="f5153-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f5153-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f5153-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f5153-110">Permission type</span></span>      | <span data-ttu-id="f5153-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f5153-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5153-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f5153-112">Delegated (work or school account)</span></span> | <span data-ttu-id="f5153-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5153-113">Directory.Read.All</span></span>    |
|<span data-ttu-id="f5153-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f5153-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5153-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f5153-115">Not supported.</span></span>    |
|<span data-ttu-id="f5153-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f5153-116">Application</span></span> | <span data-ttu-id="f5153-117">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="f5153-117">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5153-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f5153-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/getMemberGroups
POST /users/{id | userPrincipalName}/getMemberGroups
POST /groups/{id}/getMemberGroups
POST /servicePrincipals/{id}/getMemberGroups
POST /directoryObjects/{id}/getMemberGroups
```
## <a name="request-headers"></a><span data-ttu-id="f5153-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f5153-119">Request headers</span></span>
| <span data-ttu-id="f5153-120">Nome</span><span class="sxs-lookup"><span data-stu-id="f5153-120">Name</span></span>       | <span data-ttu-id="f5153-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5153-121">Type</span></span> | <span data-ttu-id="f5153-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5153-122">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f5153-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f5153-123">Authorization</span></span>  | <span data-ttu-id="f5153-124">string</span><span class="sxs-lookup"><span data-stu-id="f5153-124">string</span></span>  | <span data-ttu-id="f5153-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f5153-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f5153-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5153-127">Content-Type</span></span>  | <span data-ttu-id="f5153-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f5153-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5153-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f5153-129">Request body</span></span>
<span data-ttu-id="f5153-130">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f5153-130">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="f5153-131">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="f5153-131">Parameter</span></span>    | <span data-ttu-id="f5153-132">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5153-132">Type</span></span>   |<span data-ttu-id="f5153-133">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5153-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5153-134">securityEnabledOnly</span><span class="sxs-lookup"><span data-stu-id="f5153-134">securityEnabledOnly</span></span>|<span data-ttu-id="f5153-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5153-135">Boolean</span></span>| <span data-ttu-id="f5153-p105">**true** para especificar que somente grupos de segurança dos quais a entidade é membro devem ser retornados; **false** para especificar que todos os grupos e funções de diretório dos quais a entidade é membro devem ser retornados. **Observação**: a função só pode ser chamada em um usuário se o parâmetro for **true**.</span><span class="sxs-lookup"><span data-stu-id="f5153-p105">**true** to specify that only security groups that the entity is a member of should be returned; **false** to specify that all groups and directory roles that the entity is a member of should be returned. **Note**: The function can only be called on a user if the parameter is **true**.</span></span> |

## <a name="response"></a><span data-ttu-id="f5153-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5153-138">Response</span></span>

<span data-ttu-id="f5153-139">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto da coleção de cadeias de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f5153-139">If successful, this method returns `200 OK` response code and String collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f5153-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f5153-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="f5153-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f5153-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "directoryobject_getmembergroups"
}-->
```http
POST https://graph.microsoft.com/beta/me/getMemberGroups
Content-type: application/json

{
  "securityEnabledOnly": true
}
```

##### <a name="response"></a><span data-ttu-id="f5153-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="f5153-142">Response</span></span>
<span data-ttu-id="f5153-p106">Observação: O objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f5153-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(Edm.String)",
    "value": [
        "fee2c45b-915a-4a64-b130-f4eb9e75525e",
        "4fe90ae7-065a-478b-9400-e0a0e1cbd540",
        "e0c3beaf-eeb4-43d8-abc5-94f037a65697"
    ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f5153-145">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="f5153-145">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f5153-146">C#</span><span class="sxs-lookup"><span data-stu-id="f5153-146">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f5153-147">Javascript</span><span class="sxs-lookup"><span data-stu-id="f5153-147">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f5153-148">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="f5153-148">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/directoryobject_getmembergroups-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "directoryObject: getMemberGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryobject-getmembergroups.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
