---
title: Obter appRoleAssignment
description: Recupere as propriedades e os relacionamentos do objeto approleassignment.
localization_priority: Priority
ms.openlocfilehash: 610120c2c72b89f5af5555d59b2d58bcc09e5f1d
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2019
ms.locfileid: "29577001"
---
# <a name="get-approleassignment"></a><span data-ttu-id="4cfe3-103">Obter appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="4cfe3-103">Get appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cfe3-104">Recupere as propriedades e os relacionamentos do objeto approleassignment.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-104">Retrieve the properties and relationships of chartlegend object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4cfe3-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="4cfe3-105">Permissions</span></span>
<span data-ttu-id="4cfe3-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="4cfe3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cfe3-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4cfe3-108">Permission type</span></span>      | <span data-ttu-id="4cfe3-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="4cfe3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cfe3-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4cfe3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4cfe3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="4cfe3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="4cfe3-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4cfe3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4cfe3-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-113">Not supported.</span></span>    |
|<span data-ttu-id="4cfe3-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4cfe3-114">Application</span></span> | <span data-ttu-id="4cfe3-115">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cfe3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4cfe3-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4cfe3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="4cfe3-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="4cfe3-117">Optional query parameters</span></span>
<span data-ttu-id="4cfe3-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4cfe3-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfe3-119">Request headers</span></span>
| <span data-ttu-id="4cfe3-120">Nome</span><span class="sxs-lookup"><span data-stu-id="4cfe3-120">Name</span></span>       | <span data-ttu-id="4cfe3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cfe3-121">Type</span></span> | <span data-ttu-id="4cfe3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cfe3-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="4cfe3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4cfe3-123">Authorization</span></span>  | <span data-ttu-id="4cfe3-124">string</span><span class="sxs-lookup"><span data-stu-id="4cfe3-124">string</span></span>  | <span data-ttu-id="4cfe3-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="4cfe3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfe3-127">Request body</span></span>
<span data-ttu-id="4cfe3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4cfe3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cfe3-129">Response</span></span>

<span data-ttu-id="4cfe3-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [appRoleAssignment](../resources/approleassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-130">If successful, this method returns a `200 OK` response code and a [section](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4cfe3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4cfe3-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cfe3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4cfe3-132">Request</span></span>
<span data-ttu-id="4cfe3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
##### <a name="response"></a><span data-ttu-id="4cfe3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="4cfe3-134">Response</span></span>
<span data-ttu-id="4cfe3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4cfe3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
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
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
