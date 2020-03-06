---
title: Listar os aplicativos publicados do catálogo de aplicativos do Microsoft Teams
description: 'Listar aplicativos do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7295ac860f681db8182e66484f2df4dadb7fe5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42509325"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="a61ef-103">Listar os aplicativos publicados do catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a61ef-103">List the published apps from the Microsoft Teams app catalog</span></span>

<span data-ttu-id="a61ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a61ef-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a61ef-105">Listar [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a61ef-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="a61ef-106">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="a61ef-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="a61ef-107">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, `Organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a61ef-107">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a61ef-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="a61ef-108">Permissions</span></span>

<span data-ttu-id="a61ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a61ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

> <span data-ttu-id="a61ef-111">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a61ef-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="a61ef-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a61ef-112">Permission Type</span></span>                        | <span data-ttu-id="a61ef-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a61ef-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="a61ef-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a61ef-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a61ef-115">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a61ef-115">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="a61ef-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a61ef-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a61ef-117">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a61ef-117">Not supported</span></span>                       |
| <span data-ttu-id="a61ef-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a61ef-118">Application</span></span>                            | <span data-ttu-id="a61ef-119">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a61ef-119">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="a61ef-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a61ef-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a61ef-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a61ef-121">Optional query parameters</span></span>

<span data-ttu-id="a61ef-122">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a61ef-122">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a61ef-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a61ef-123">Request headers</span></span>

| <span data-ttu-id="a61ef-124">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a61ef-124">Header</span></span>        | <span data-ttu-id="a61ef-125">Valor</span><span class="sxs-lookup"><span data-stu-id="a61ef-125">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="a61ef-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="a61ef-126">Authorization</span></span> | <span data-ttu-id="a61ef-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a61ef-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a61ef-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a61ef-129">Request body</span></span>

<span data-ttu-id="a61ef-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a61ef-130">None.</span></span>

> <span data-ttu-id="a61ef-131">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsCatalogApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="a61ef-131">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="a61ef-132">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="a61ef-132">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="a61ef-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a61ef-133">Response</span></span>

<span data-ttu-id="a61ef-134">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de objetos [teamsCatalogApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a61ef-134">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a61ef-135">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a61ef-135">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="a61ef-136">Exemplo 1: listar todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="a61ef-136">Example 1: List all applications</span></span>

<span data-ttu-id="a61ef-137">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a61ef-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="a61ef-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a61ef-138">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a61ef-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a61ef-139">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="a61ef-140">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="a61ef-140">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="a61ef-141">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="a61ef-141">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="a61ef-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a61ef-142">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="a61ef-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a61ef-143">Response</span></span>

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
