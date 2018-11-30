---
title: Listar os aplicativos publicados a partir do catálogo de aplicativos do Microsoft Teams
description: 'Lista de aplicativos a partir do catálogo de aplicativos do Microsoft Teams. '
ms.openlocfilehash: 84b5576ed2a7d38783e45b1384c79f05c9ea418b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041039"
---
# <a name="list-the-published-apps-from-the-microsoft-teams-app-catalog"></a><span data-ttu-id="a5bc8-103">Listar os aplicativos publicados a partir do catálogo de aplicativos do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="a5bc8-103">List the published apps from the Microsoft Teams app catalog</span></span>

> <span data-ttu-id="a5bc8-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a5bc8-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a5bc8-106">Listar os [aplicativos](../resources/teamsapp.md) do catálogo de aplicativos do Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-106">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span> <span data-ttu-id="a5bc8-107">Isso inclui aplicativos do repositório de Teams da Microsoft, bem como aplicativos de catálogo de aplicativos da sua organização (o catálogo de aplicativos do inquilino).</span><span class="sxs-lookup"><span data-stu-id="a5bc8-107">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="a5bc8-108">Para obter os aplicativos do catálogo de aplicativos da sua organização somente, especifique `Organization` como o **distributionMethod** no recurso [teamsCatalogApp](../resources/teamsapp.md) .</span><span class="sxs-lookup"><span data-stu-id="a5bc8-108">To get apps from your organization's app catalog only, specify `Organization` as the **distributionMethod** in the [teamsCatalogApp](../resources/teamsapp.md) resource.</span></span>

## <a name="permissions"></a><span data-ttu-id="a5bc8-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="a5bc8-109">Permissions</span></span>

<span data-ttu-id="a5bc8-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span><span class="sxs-lookup"><span data-stu-id="a5bc8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="a5bc8-112">**Observação:** Somente os administradores globais podem chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-112">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="a5bc8-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a5bc8-113">Permission Type</span></span>                        | <span data-ttu-id="a5bc8-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a5bc8-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="a5bc8-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a5bc8-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="a5bc8-116">AppCatalog.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5bc8-116">AppCatalog.ReadWrite.All</span></span> |
| <span data-ttu-id="a5bc8-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a5bc8-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5bc8-118">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a5bc8-118">Not supported</span></span>|
| <span data-ttu-id="a5bc8-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a5bc8-119">Application</span></span>                            | <span data-ttu-id="a5bc8-120">Sem suporte</span><span class="sxs-lookup"><span data-stu-id="a5bc8-120">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5bc8-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a5bc8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5bc8-122">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="a5bc8-122">Optional query parameters</span></span>
<span data-ttu-id="a5bc8-123">Este método oferece suporte a $filter, $select, e $expand [OData parâmetros de consulta](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-123">This method supports the $filter, $select, and $expand [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a5bc8-124">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bc8-124">Request headers</span></span>

| <span data-ttu-id="a5bc8-125">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a5bc8-125">Header</span></span>        | <span data-ttu-id="a5bc8-126">Valor</span><span class="sxs-lookup"><span data-stu-id="a5bc8-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="a5bc8-127">Autorização</span><span class="sxs-lookup"><span data-stu-id="a5bc8-127">Authorization</span></span> | <span data-ttu-id="a5bc8-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a5bc8-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bc8-130">Request body</span></span>
<span data-ttu-id="a5bc8-131">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-131">None.</span></span>

><span data-ttu-id="a5bc8-132">**Observação:** Você pode filtrar em qualquer um dos campos do objeto [teamsCatalogApp](../resources/teamsapp.md) para diminuir a lista de resultados.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-132">**Note:** You can filter on any of the fields of the [teamsCatalogApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="a5bc8-133">Você pode usar qualquer uma das seguintes operações de filtro: igual, não-igual e, ou e não.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-133">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="response"></a><span data-ttu-id="a5bc8-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5bc8-134">Response</span></span>
<span data-ttu-id="a5bc8-135">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de objetos [teamsCatalogApp](../resources/teamsapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-135">If successful, this method returns a `200 OK` response code and a list of [teamsCatalogApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a5bc8-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="a5bc8-136">Examples</span></span>
### <a name="example-1"></a><span data-ttu-id="a5bc8-137">Exemplo 1</span><span class="sxs-lookup"><span data-stu-id="a5bc8-137">Example 1</span></span>
<span data-ttu-id="a5bc8-138">O exemplo a seguir lista todos os aplicativos que são específicos para seu locatário.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="a5bc8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bc8-139">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```

#### <a name="response"></a><span data-ttu-id="a5bc8-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5bc8-140">Response</span></span>
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

### <a name="example-2"></a><span data-ttu-id="a5bc8-141">Exemplo 2</span><span class="sxs-lookup"><span data-stu-id="a5bc8-141">Example 2</span></span>

<span data-ttu-id="a5bc8-142">O exemplo a seguir lista aplicativos com uma ID especificada.</span><span class="sxs-lookup"><span data-stu-id="a5bc8-142">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="a5bc8-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a5bc8-143">Request</span></span>
```
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```

#### <a name="response"></a><span data-ttu-id="a5bc8-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="a5bc8-144">Response</span></span>
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

