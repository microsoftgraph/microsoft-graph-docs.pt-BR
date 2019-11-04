---
title: Obter accessPackageCatalog
description: Recupere as propriedades e os relacionamentos do objeto accesspackagecatalog.
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: b3c12ba6922e3252c91cd456e17ad162be7a3e40
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37935079"
---
# <a name="get-accesspackagecatalog"></a><span data-ttu-id="3ee07-103">Obter accessPackageCatalog</span><span class="sxs-lookup"><span data-stu-id="3ee07-103">Get accessPackageCatalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ee07-104">Recupere as propriedades e os relacionamentos de um objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) .</span><span class="sxs-lookup"><span data-stu-id="3ee07-104">Retrieve the properties and relationships of an [accessPackageCatalog](../resources/accesspackagecatalog.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="3ee07-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="3ee07-105">Permissions</span></span>

<span data-ttu-id="3ee07-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="3ee07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="3ee07-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3ee07-108">Permission type</span></span>                        | <span data-ttu-id="3ee07-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="3ee07-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="3ee07-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3ee07-110">Delegated (work or school account)</span></span>     |  <span data-ttu-id="3ee07-111">EntitlementManagement. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="3ee07-111">EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="3ee07-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3ee07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3ee07-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ee07-113">Not supported.</span></span> |
| <span data-ttu-id="3ee07-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3ee07-114">Application</span></span>                            | <span data-ttu-id="3ee07-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3ee07-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3ee07-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3ee07-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3ee07-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="3ee07-117">Optional query parameters</span></span>

<span data-ttu-id="3ee07-118">Este método oferece suporte a alguns dos parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee07-118">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3ee07-119">Por exemplo, para recuperar os pacotes do Access em um catálogo, `$expand=accessPackages` inclua a consulta.</span><span class="sxs-lookup"><span data-stu-id="3ee07-119">For example, to retrieve the access packages in a catalog, include `$expand=accessPackages` in the query.</span></span> <span data-ttu-id="3ee07-120">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="3ee07-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3ee07-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee07-121">Request headers</span></span>

| <span data-ttu-id="3ee07-122">Nome</span><span class="sxs-lookup"><span data-stu-id="3ee07-122">Name</span></span>      |<span data-ttu-id="3ee07-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ee07-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="3ee07-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="3ee07-124">Authorization</span></span> | <span data-ttu-id="3ee07-125">\{token\} de portador.</span><span class="sxs-lookup"><span data-stu-id="3ee07-125">Bearer \{token\}.</span></span> <span data-ttu-id="3ee07-126">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3ee07-126">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="3ee07-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee07-127">Request body</span></span>

<span data-ttu-id="3ee07-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="3ee07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3ee07-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee07-129">Response</span></span>

<span data-ttu-id="3ee07-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [accessPackageCatalog](../resources/accesspackagecatalog.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee07-130">If successful, this method returns a `200 OK` response code and the requested [accessPackageCatalog](../resources/accesspackagecatalog.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3ee07-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="3ee07-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3ee07-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3ee07-132">Request</span></span>

<span data-ttu-id="3ee07-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="3ee07-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_accesspackagecatalog"
}-->

```http
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}
```

### <a name="response"></a><span data-ttu-id="3ee07-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="3ee07-134">Response</span></span>

<span data-ttu-id="3ee07-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="3ee07-135">The following is an example of the response.</span></span>

> <span data-ttu-id="3ee07-p104">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3ee07-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.accessPackageCatalog"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id":"360fa7de-90be-48dc-a2ce-fc40094a93dd",
    "description":"Sample access package catalog",
    "displayName":"Access package catalog for testing",
    "isExternallyVisible":false,
    "catalogType":"UserManaged",
    "catalogStatus":"Published",
    "createdDateTime":"2019-01-27T18:19:50.74Z",
    "modifiedDateTime":"2019-01-27T18:19:50.74Z",
    "createdBy":"TestGA@example.com",
    "modifiedBy":"TestGA@example.com"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get accessPackageCatalog",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
