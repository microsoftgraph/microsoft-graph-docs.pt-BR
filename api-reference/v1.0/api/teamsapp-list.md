---
title: Listar os aplicativos publicados a partir do catálogo de aplicativos do Microsoft Teams
description: 'Lista de aplicativos a partir do catálogo de aplicativos do Microsoft Teams. '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a19c852b4cca08b7318ef33cdf24929e5f4c3042
ms.sourcegitcommit: 2c60e38bb1b71ba958659f66ad4736495e520851
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/15/2019
ms.locfileid: "28016664"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="fe991-103">Listar os aplicativos publicados a partir do catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="fe991-103">List the published apps from the Microsoft Teams app catalog</span></span>



<span data-ttu-id="fe991-104">Listar os [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="fe991-104">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="fe991-105">Isso inclui aplicativos do repositório de Teams da Microsoft, bem como aplicativos de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="fe991-105">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="fe991-106">Para obter os aplicativos do catálogo de aplicativos da sua organização somente, especifique `Organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="fe991-106">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe991-107">Permissões</span><span class="sxs-lookup"><span data-stu-id="fe991-107">Permissions</span></span>

<span data-ttu-id="fe991-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="fe991-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="fe991-110">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="fe991-110">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="fe991-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fe991-111">Permission Type</span></span>                        | <span data-ttu-id="fe991-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fe991-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="fe991-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fe991-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="fe991-114">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe991-114">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="fe991-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fe991-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe991-116">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fe991-116">Not supported</span></span>|
| <span data-ttu-id="fe991-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fe991-117">Application</span></span>                            | <span data-ttu-id="fe991-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="fe991-118">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="fe991-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fe991-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fe991-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fe991-120">Optional query parameters</span></span>
<span data-ttu-id="fe991-121">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fe991-121">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fe991-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fe991-122">Request headers</span></span>

| <span data-ttu-id="fe991-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fe991-123">Header</span></span>        | <span data-ttu-id="fe991-124">Valor</span><span class="sxs-lookup"><span data-stu-id="fe991-124">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="fe991-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="fe991-125">Authorization</span></span> | <span data-ttu-id="fe991-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fe991-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe991-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fe991-128">Request body</span></span>
<span data-ttu-id="fe991-129">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="fe991-129">None.</span></span>

><span data-ttu-id="fe991-130">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsCatalogApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="fe991-130">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="fe991-131">Você pode usar qualquer uma das seguintes operações de filtro: igual, não-igual e, ou e não.</span><span class="sxs-lookup"><span data-stu-id="fe991-131">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="fe991-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe991-132">Response</span></span>
<span data-ttu-id="fe991-133">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsCatalogApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fe991-133">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fe991-134">Exemplos</span><span class="sxs-lookup"><span data-stu-id="fe991-134">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="fe991-135">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="fe991-135">Example 1</span></span>
<span data-ttu-id="fe991-136">O exemplo a seguir lista todos os aplicativos que são específicos para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="fe991-136">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="fe991-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe991-137">Request</span></span>
```
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="fe991-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe991-138">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

### <a name="example-2"></a><span data-ttu-id="fe991-139">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="fe991-139">Example 2</span></span>

<span data-ttu-id="fe991-140">O exemplo a seguir lista aplicativos com uma ID especificada.</span><span class="sxs-lookup"><span data-stu-id="fe991-140">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="fe991-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fe991-141">Request</span></span>
```
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="fe991-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="fe991-142">Response</span></span>
```
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod":"Organization"
    }
  ]
}
```

