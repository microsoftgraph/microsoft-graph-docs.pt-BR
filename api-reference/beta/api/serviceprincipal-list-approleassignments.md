---
title: 'servicePrincipal: listar appRoleAssignments'
description: Recupere uma lista de objetos approleassignment.
localization_priority: Normal
ms.openlocfilehash: d9134985359a76b3d26b93aa675cdd82284a17b4
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29574653"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="d4e0c-103">servicePrincipal: listar appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="d4e0c-103">servicePrincipal: List appRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4e0c-104">Recupere uma lista de objetos approleassignment.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-104">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="d4e0c-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d4e0c-105">Permissions</span></span>
<span data-ttu-id="d4e0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4e0c-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d4e0c-108">Permission type</span></span>      | <span data-ttu-id="d4e0c-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4e0c-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4e0c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4e0c-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4e0c-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d4e0c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4e0c-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-113">Not supported.</span></span>    |
|<span data-ttu-id="d4e0c-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d4e0c-114">Application</span></span> | <span data-ttu-id="d4e0c-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4e0c-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4e0c-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d4e0c-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4e0c-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d4e0c-117">Optional query parameters</span></span>
<span data-ttu-id="d4e0c-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d4e0c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e0c-119">Request headers</span></span>
| <span data-ttu-id="d4e0c-120">Nome</span><span class="sxs-lookup"><span data-stu-id="d4e0c-120">Name</span></span>       | <span data-ttu-id="d4e0c-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="d4e0c-121">Type</span></span> | <span data-ttu-id="d4e0c-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="d4e0c-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4e0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d4e0c-123">Authorization</span></span>  | <span data-ttu-id="d4e0c-124">string</span><span class="sxs-lookup"><span data-stu-id="d4e0c-124">string</span></span>  | <span data-ttu-id="d4e0c-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4e0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e0c-127">Request body</span></span>
<span data-ttu-id="d4e0c-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4e0c-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e0c-129">Response</span></span>

<span data-ttu-id="d4e0c-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-130">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4e0c-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d4e0c-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4e0c-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d4e0c-132">Request</span></span>
<span data-ttu-id="d4e0c-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="d4e0c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d4e0c-134">Response</span></span>
<span data-ttu-id="d4e0c-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d4e0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
