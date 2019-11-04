---
title: Listar accessPackageResources
description: Recupere uma lista de objetos accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ebb1d6ce33c2f10da19162d40f097c1043af62e8
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935076"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="2a8e4-103">Listar accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="2a8e4-103">List accessPackageResources</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a8e4-104">Recupere uma lista de objetos [accessPackageResource](../resources/accesspackageresource.md) em um [accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="2a8e4-104">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2a8e4-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="2a8e4-105">Permissions</span></span>

<span data-ttu-id="2a8e4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a8e4-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2a8e4-108">Permission type</span></span>                        | <span data-ttu-id="2a8e4-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2a8e4-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a8e4-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2a8e4-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="2a8e4-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="2a8e4-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="2a8e4-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2a8e4-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a8e4-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-113">Not supported.</span></span> |
| <span data-ttu-id="2a8e4-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2a8e4-114">Application</span></span>                            | <span data-ttu-id="2a8e4-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a8e4-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2a8e4-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a8e4-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2a8e4-117">Optional query parameters</span></span>

<span data-ttu-id="2a8e4-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="2a8e4-119">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="2a8e4-119">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a8e4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2a8e4-120">Request headers</span></span>

| <span data-ttu-id="2a8e4-121">Nome</span><span class="sxs-lookup"><span data-stu-id="2a8e4-121">Name</span></span>      |<span data-ttu-id="2a8e4-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="2a8e4-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a8e4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="2a8e4-123">Authorization</span></span> | <span data-ttu-id="2a8e4-124">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-124">Bearer \{token\}.</span></span> <span data-ttu-id="2a8e4-125">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a8e4-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2a8e4-126">Request body</span></span>

<span data-ttu-id="2a8e4-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a8e4-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a8e4-128">Response</span></span>

<span data-ttu-id="2a8e4-129">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma coleção de objetos [accessPackageResource](../resources/accesspackageresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-129">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a8e4-130">Exemplos</span><span class="sxs-lookup"><span data-stu-id="2a8e4-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a8e4-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2a8e4-131">Request</span></span>

<span data-ttu-id="2a8e4-132">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

### <a name="response"></a><span data-ttu-id="2a8e4-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2a8e4-133">Response</span></span>

<span data-ttu-id="2a8e4-134">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-134">The following is an example of the response.</span></span>

> <span data-ttu-id="2a8e4-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2a8e4-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageResource",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "400279ff-8e85-4dcf-b1d6-d3a6be372951",
      "displayName": "Faculty cafeteria ordering",
      "description": "Example application",
      "url": "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/",
      "resourceType": "Application",
      "originId": "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List accessPackageResources",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
