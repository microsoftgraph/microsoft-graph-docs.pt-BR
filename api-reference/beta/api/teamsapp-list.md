---
title: Listar os aplicativos publicados do catálogo de aplicativos do Microsoft Teams
description: 'Listar aplicativos do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: d7e406a1d6bbef99bc5aa6c9e6670b446b78950e
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2020
ms.locfileid: "44290711"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="e92f1-103">Listar os aplicativos publicados do catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="e92f1-103">List the published apps from the Microsoft Teams app catalog</span></span>

<span data-ttu-id="e92f1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e92f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e92f1-105">Listar [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="e92f1-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="e92f1-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="e92f1-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="e92f1-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, especifique `Organization` como **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="e92f1-107">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="e92f1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="e92f1-108">Permissions</span></span>

<span data-ttu-id="e92f1-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="e92f1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

| <span data-ttu-id="e92f1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e92f1-111">Permission Type</span></span>                        | <span data-ttu-id="e92f1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e92f1-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="e92f1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e92f1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="e92f1-114">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e92f1-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="e92f1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e92f1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e92f1-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="e92f1-116">Not supported</span></span>                       |
| <span data-ttu-id="e92f1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e92f1-117">Application</span></span>                            | <span data-ttu-id="e92f1-118">AppCatalog. Read. All, AppCatalog. ReadWrite. All, Directory. Read. All, Directory. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="e92f1-118">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e92f1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e92f1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e92f1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e92f1-120">Optional query parameters</span></span>

<span data-ttu-id="e92f1-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e92f1-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e92f1-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e92f1-122">Request headers</span></span>

| <span data-ttu-id="e92f1-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e92f1-123">Header</span></span>        | <span data-ttu-id="e92f1-124">Valor</span><span class="sxs-lookup"><span data-stu-id="e92f1-124">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="e92f1-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="e92f1-125">Authorization</span></span> | <span data-ttu-id="e92f1-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e92f1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e92f1-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e92f1-128">Request body</span></span>

<span data-ttu-id="e92f1-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e92f1-129">None.</span></span>

> <span data-ttu-id="e92f1-130">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsCatalogApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="e92f1-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="e92f1-131">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="e92f1-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="e92f1-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="e92f1-132">Response</span></span>

<span data-ttu-id="e92f1-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsCatalogApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e92f1-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e92f1-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e92f1-134">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="e92f1-135">Exemplo 1: listar todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="e92f1-135">Example 1: List all applications</span></span>

<span data-ttu-id="e92f1-136">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="e92f1-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="e92f1-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e92f1-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="e92f1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e92f1-138">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="e92f1-139">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="e92f1-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="e92f1-140">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="e92f1-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="e92f1-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e92f1-141">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="e92f1-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="e92f1-142">Response</span></span>

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

