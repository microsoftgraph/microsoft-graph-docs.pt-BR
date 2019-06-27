---
title: Obter um scopedRoleMember
description: Recupere um recurso scopedRoleMembership específico.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 9f56be38a68bccb3478afeb12716b0f52e560b89
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35258734"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="ab2aa-103">Obter um scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="ab2aa-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ab2aa-104">Recupere um recurso [scopedRoleMembership](../resources/scopedrolemembership.md) específico.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="ab2aa-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="ab2aa-105">Permissions</span></span>
<span data-ttu-id="ab2aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab2aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ab2aa-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab2aa-108">Permission type</span></span>      | <span data-ttu-id="ab2aa-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab2aa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab2aa-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab2aa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ab2aa-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ab2aa-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ab2aa-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab2aa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab2aa-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-113">Not supported.</span></span>    |
|<span data-ttu-id="ab2aa-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab2aa-114">Application</span></span> | <span data-ttu-id="ab2aa-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab2aa-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab2aa-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab2aa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ab2aa-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab2aa-117">Optional query parameters</span></span>
<span data-ttu-id="ab2aa-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ab2aa-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2aa-119">Request headers</span></span>
| <span data-ttu-id="ab2aa-120">Nome</span><span class="sxs-lookup"><span data-stu-id="ab2aa-120">Name</span></span>      |<span data-ttu-id="ab2aa-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="ab2aa-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ab2aa-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab2aa-122">Authorization</span></span>  | <span data-ttu-id="ab2aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ab2aa-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2aa-125">Request body</span></span>
<span data-ttu-id="ab2aa-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab2aa-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2aa-127">Response</span></span>

<span data-ttu-id="ab2aa-128">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [scopedRoleMembership](../resources/scopedrolemembership.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab2aa-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab2aa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ab2aa-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab2aa-130">Request</span></span>
<span data-ttu-id="ab2aa-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
##### <a name="response"></a><span data-ttu-id="ab2aa-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab2aa-132">Response</span></span>
<span data-ttu-id="ab2aa-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab2aa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="ab2aa-136">Código de exemplo do SDK</span><span class="sxs-lookup"><span data-stu-id="ab2aa-136">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="ab2aa-137">C#</span><span class="sxs-lookup"><span data-stu-id="ab2aa-137">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_scopedrolemember-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ab2aa-138">Javascript</span><span class="sxs-lookup"><span data-stu-id="ab2aa-138">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_scopedrolemember-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="ab2aa-139">Objetivo-C</span><span class="sxs-lookup"><span data-stu-id="ab2aa-139">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_scopedrolemember-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/administrativeunit-get-scopedrolemembers.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
