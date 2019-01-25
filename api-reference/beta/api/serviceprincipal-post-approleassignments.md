---
title: Criar appRoleAssignment
description: Use essa API para criar um novo appRoleAssignment.
localization_priority: Normal
ms.openlocfilehash: 70993bf1e5402c3fab7229269fbc007602813c40
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528764"
---
# <a name="create-approleassignment"></a><span data-ttu-id="25915-103">Criar appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="25915-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="25915-104">Use essa API para criar um novo appRoleAssignment.</span><span class="sxs-lookup"><span data-stu-id="25915-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="25915-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="25915-105">Permissions</span></span>
<span data-ttu-id="25915-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="25915-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25915-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="25915-108">Permission type</span></span>      | <span data-ttu-id="25915-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="25915-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="25915-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="25915-110">Delegated (work or school account)</span></span> | <span data-ttu-id="25915-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="25915-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="25915-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="25915-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="25915-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25915-113">Not supported.</span></span>    |
|<span data-ttu-id="25915-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="25915-114">Application</span></span> | <span data-ttu-id="25915-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="25915-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="25915-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25915-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="25915-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="25915-117">Request headers</span></span>
| <span data-ttu-id="25915-118">Nome</span><span class="sxs-lookup"><span data-stu-id="25915-118">Name</span></span>       | <span data-ttu-id="25915-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="25915-119">Type</span></span> | <span data-ttu-id="25915-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="25915-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="25915-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="25915-121">Authorization</span></span>  | <span data-ttu-id="25915-122">string</span><span class="sxs-lookup"><span data-stu-id="25915-122">string</span></span>  | <span data-ttu-id="25915-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="25915-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="25915-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25915-125">Request body</span></span>
<span data-ttu-id="25915-126">No corpo da solicitação, fornece uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="25915-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="25915-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="25915-127">Response</span></span>

<span data-ttu-id="25915-128">Se tiver êxito, este método retornará `201 Created` objeto response de código e [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25915-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25915-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25915-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="25915-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25915-130">Request</span></span>
<span data-ttu-id="25915-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="25915-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="25915-132">No corpo da solicitação, fornece uma representação JSON do objeto [appRoleAssignment](../resources/approleassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="25915-132">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="25915-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="25915-133">Response</span></span>
<span data-ttu-id="25915-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="25915-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-post-approleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
