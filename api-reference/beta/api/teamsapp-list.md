---
title: Listar teamsApp
description: 'Listar aplicativos do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 46a3efdf2e5644bcca119a290c83f86c1e8ad60a
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/18/2020
ms.locfileid: "46790501"
---
# <a name="list-teamsapp"></a><span data-ttu-id="fa2f9-103">Listar teamsApp</span><span class="sxs-lookup"><span data-stu-id="fa2f9-103">List teamsApp</span></span>

<span data-ttu-id="fa2f9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fa2f9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fa2f9-105">Listar [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="fa2f9-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="fa2f9-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="fa2f9-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `organization` como **distributionMethod** na solicitação.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa2f9-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="fa2f9-108">Permissions</span></span>

<span data-ttu-id="fa2f9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fa2f9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="fa2f9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fa2f9-111">Permission Type</span></span>                        | <span data-ttu-id="fa2f9-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fa2f9-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="fa2f9-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fa2f9-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fa2f9-114">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="fa2f9-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="fa2f9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fa2f9-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa2f9-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fa2f9-116">Not supported</span></span>                       |
| <span data-ttu-id="fa2f9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fa2f9-117">Application</span></span>                            | <span data-ttu-id="fa2f9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa2f9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fa2f9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fa2f9-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fa2f9-120">Optional query parameters</span></span>

<span data-ttu-id="fa2f9-121">Este método suporta o `$filter`, `$select`, e `$expand` [parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

> <span data-ttu-id="fa2f9-122">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-122">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="fa2f9-123">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-123">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fa2f9-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f9-124">Request headers</span></span>

| <span data-ttu-id="fa2f9-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fa2f9-125">Header</span></span>        | <span data-ttu-id="fa2f9-126">Valor</span><span class="sxs-lookup"><span data-stu-id="fa2f9-126">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="fa2f9-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="fa2f9-127">Authorization</span></span> | <span data-ttu-id="fa2f9-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fa2f9-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f9-130">Request body</span></span>

<span data-ttu-id="fa2f9-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa2f9-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa2f9-132">Response</span></span>

<span data-ttu-id="fa2f9-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-133">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fa2f9-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fa2f9-134">Examples</span></span>

### <a name="example-1-list-all-applications-in-a-tenant"></a><span data-ttu-id="fa2f9-135">Exemplo 1: listar todos os aplicativos em um locatário</span><span class="sxs-lookup"><span data-stu-id="fa2f9-135">Example 1: List all applications in a tenant</span></span>

<span data-ttu-id="fa2f9-136">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="fa2f9-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f9-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="fa2f9-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa2f9-138">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="fa2f9-139">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="fa2f9-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="fa2f9-140">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="fa2f9-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="fa2f9-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fa2f9-141">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="fa2f9-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fa2f9-142">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```
