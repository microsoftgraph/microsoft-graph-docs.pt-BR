---
title: Listar os aplicativos publicados do catálogo de aplicativos do Microsoft Teams
description: 'Listar aplicativos do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 1e4d9348cbb28ed0daf1ec48459378935d78e0a2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32544648"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="a8379-103">Listar os aplicativos publicados do catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a8379-103">List the published apps from the Microsoft Teams app catalog</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a8379-104">Listar [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a8379-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="a8379-105">Isso inclui os aplicativos do Microsoft Teams Store, bem como os aplicativos do catálogo de aplicativos da sua organização (o catálogo de aplicativos do locatário).</span><span class="sxs-lookup"><span data-stu-id="a8379-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="a8379-106">Para obter aplicativos apenas do catálogo de aplicativos da sua organização, `Organization` especifique como **DistributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a8379-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a8379-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="a8379-107">Permissions</span></span>

<span data-ttu-id="a8379-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a8379-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions_reference).</span></span>

> <span data-ttu-id="a8379-110">**Observação:** Somente os administradores globais podem chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a8379-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="a8379-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a8379-111">Permission Type</span></span>                        | <span data-ttu-id="a8379-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a8379-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="a8379-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a8379-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="a8379-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a8379-114">AppCatalog.ReadWrite.All</span></span>            |
| <span data-ttu-id="a8379-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a8379-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a8379-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8379-116">Not supported</span></span>                       |
| <span data-ttu-id="a8379-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a8379-117">Application</span></span>                            | <span data-ttu-id="a8379-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a8379-118">Not supported</span></span>                       |

## <a name="http-request"></a><span data-ttu-id="a8379-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a8379-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a8379-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a8379-120">Optional query parameters</span></span>

<span data-ttu-id="a8379-121">Este método dá suporte aos [Parâmetros de consulta OData](/graph/query-parameters) $filter, $select e $expand para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a8379-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a8379-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a8379-122">Request headers</span></span>

| <span data-ttu-id="a8379-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a8379-123">Header</span></span>        | <span data-ttu-id="a8379-124">Valor</span><span class="sxs-lookup"><span data-stu-id="a8379-124">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="a8379-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="a8379-125">Authorization</span></span> | <span data-ttu-id="a8379-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a8379-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a8379-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a8379-128">Request body</span></span>

<span data-ttu-id="a8379-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a8379-129">None.</span></span>

> <span data-ttu-id="a8379-130">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsCatalogApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="a8379-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="a8379-131">Você pode usar qualquer uma das seguintes operações de filtro: igual, não igual, e, ou, e não.</span><span class="sxs-lookup"><span data-stu-id="a8379-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="a8379-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8379-132">Response</span></span>

<span data-ttu-id="a8379-133">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de objetos [teamsCatalogApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a8379-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a8379-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a8379-134">Examples</span></span>

### <a name="example-1-list-all-applications"></a><span data-ttu-id="a8379-135">Exemplo 1: listar todos os aplicativos</span><span class="sxs-lookup"><span data-stu-id="a8379-135">Example 1: List all applications</span></span>

<span data-ttu-id="a8379-136">O exemplo a seguir lista todos os aplicativos específicos do seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a8379-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="a8379-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8379-137">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="a8379-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8379-138">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="a8379-139">Exemplo 2: listar aplicativos com uma determinada ID</span><span class="sxs-lookup"><span data-stu-id="a8379-139">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="a8379-140">O exemplo a seguir lista os aplicativos com uma determinada ID.</span><span class="sxs-lookup"><span data-stu-id="a8379-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="a8379-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a8379-141">Request</span></span>

```http
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="a8379-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="a8379-142">Response</span></span>

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

<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/teamsapp-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
