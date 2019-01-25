---
title: Lista connectorGroups
description: Recupere uma lista de objetos connectorgroup.
localization_priority: Normal
ms.openlocfilehash: a12c156f486a158e2d5a7d5885b0d8817f28e1c9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508633"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="e3591-103">Lista connectorGroups</span><span class="sxs-lookup"><span data-stu-id="e3591-103">List connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e3591-104">Recupere uma lista de objetos connectorgroup.</span><span class="sxs-lookup"><span data-stu-id="e3591-104">Retrieve a list of connectorgroup objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="e3591-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="e3591-105">Permissions</span></span>
<span data-ttu-id="e3591-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e3591-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3591-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e3591-108">Permission type</span></span>      | <span data-ttu-id="e3591-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e3591-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e3591-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e3591-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e3591-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e3591-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e3591-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e3591-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e3591-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e3591-113">Not supported.</span></span>    |
|<span data-ttu-id="e3591-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e3591-114">Application</span></span> | <span data-ttu-id="e3591-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3591-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e3591-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e3591-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /connectorGroups
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e3591-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e3591-117">Optional query parameters</span></span>
<span data-ttu-id="e3591-118">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e3591-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e3591-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e3591-119">Request headers</span></span>
| <span data-ttu-id="e3591-120">Nome</span><span class="sxs-lookup"><span data-stu-id="e3591-120">Name</span></span>      |<span data-ttu-id="e3591-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="e3591-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e3591-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e3591-122">Authorization</span></span>  | <span data-ttu-id="e3591-123"> de portador</span><span class="sxs-lookup"><span data-stu-id="e3591-123">Bearer.</span></span> <span data-ttu-id="e3591-124">Obrigatório</span><span class="sxs-lookup"><span data-stu-id="e3591-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3591-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e3591-125">Request body</span></span>
<span data-ttu-id="e3591-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e3591-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3591-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3591-127">Response</span></span>

<span data-ttu-id="e3591-128">Se tiver êxito, este método retornará um `200 OK` código de resposta e a coleção de objetos [connectorGroup](../resources/connectorgroup.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e3591-128">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e3591-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e3591-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e3591-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e3591-130">Request</span></span>
<span data-ttu-id="e3591-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e3591-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```http
GET https://graph.microsoft.com/{ver}/connectorGroups
```
##### <a name="response"></a><span data-ttu-id="e3591-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e3591-132">Response</span></span>
<span data-ttu-id="e3591-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e3591-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectorGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
