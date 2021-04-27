---
title: Listar accessPackageResources
description: Recupere uma lista de objetos accesspackageresource.
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: be2ad10b946574ca48b93ada1d7833262f127059
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048558"
---
# <a name="list-accesspackageresources"></a><span data-ttu-id="389f2-103">Listar accessPackageResources</span><span class="sxs-lookup"><span data-stu-id="389f2-103">List accessPackageResources</span></span>

<span data-ttu-id="389f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="389f2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="389f2-105">Recuperar uma lista de [objetos accessPackageResource](../resources/accesspackageresource.md) em [um accessPackageCatalog](../resources/accesspackagecatalog.md).</span><span class="sxs-lookup"><span data-stu-id="389f2-105">Retrieve a list of [accessPackageResource](../resources/accesspackageresource.md) objects in an [accessPackageCatalog](../resources/accesspackagecatalog.md).</span></span>  <span data-ttu-id="389f2-106">Para solicitar para adicionar ou remover [um accessPackageResource,](../resources/accesspackageresource.md)use [criar accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span><span class="sxs-lookup"><span data-stu-id="389f2-106">To request to add or remove an [accessPackageResource](../resources/accesspackageresource.md), use [create accessPackageResourceRequest](accesspackageresourcerequest-post.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="389f2-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="389f2-107">Permissions</span></span>

<span data-ttu-id="389f2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="389f2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="389f2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="389f2-110">Permission type</span></span>                        | <span data-ttu-id="389f2-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="389f2-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="389f2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="389f2-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="389f2-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="389f2-113">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="389f2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="389f2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="389f2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="389f2-115">Not supported.</span></span> |
| <span data-ttu-id="389f2-116">Application</span><span class="sxs-lookup"><span data-stu-id="389f2-116">Application</span></span>                            | <span data-ttu-id="389f2-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="389f2-117">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="389f2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="389f2-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```

## <a name="optional-query-parameters"></a><span data-ttu-id="389f2-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="389f2-119">Optional query parameters</span></span>

<span data-ttu-id="389f2-120">Este método dá suporte a alguns parâmetros de consulta OData para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="389f2-120">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="389f2-121">Para obter informações gerais, acesse [Parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="389f2-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="389f2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="389f2-122">Request headers</span></span>

| <span data-ttu-id="389f2-123">Nome</span><span class="sxs-lookup"><span data-stu-id="389f2-123">Name</span></span>      |<span data-ttu-id="389f2-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="389f2-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="389f2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="389f2-125">Authorization</span></span> | <span data-ttu-id="389f2-p104">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="389f2-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="389f2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="389f2-128">Request body</span></span>

<span data-ttu-id="389f2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="389f2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="389f2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="389f2-130">Response</span></span>

<span data-ttu-id="389f2-131">Se tiver êxito, este método retornará um código de resposta e uma `200 OK` coleção de [objetos accessPackageResource](../resources/accesspackageresource.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="389f2-131">If successful, this method returns a `200 OK` response code and a collection of [accessPackageResource](../resources/accesspackageresource.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="389f2-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="389f2-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="389f2-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="389f2-133">Request</span></span>

<span data-ttu-id="389f2-134">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="389f2-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="389f2-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="389f2-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_accesspackageresources"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageCatalogs/{id}/accessPackageResources
```
# <a name="c"></a>[<span data-ttu-id="389f2-136">C#</span><span class="sxs-lookup"><span data-stu-id="389f2-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-accesspackageresources-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="389f2-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="389f2-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-accesspackageresources-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="389f2-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="389f2-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-accesspackageresources-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="389f2-139">Java</span><span class="sxs-lookup"><span data-stu-id="389f2-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-accesspackageresources-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="389f2-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="389f2-140">Response</span></span>

<span data-ttu-id="389f2-141">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="389f2-141">The following is an example of the response.</span></span>

> <span data-ttu-id="389f2-142">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="389f2-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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


