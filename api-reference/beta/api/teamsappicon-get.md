---
title: Obter teamsAppIcon
description: Recupere um ícone associado a uma definição específica de um aplicativo do Teams.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1ccada523f670df173304fafd43747a63444e7e2
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882635"
---
# <a name="get-teamsappicon"></a><span data-ttu-id="c39b2-103">Obter teamsAppIcon</span><span class="sxs-lookup"><span data-stu-id="c39b2-103">Get teamsAppIcon</span></span>

<span data-ttu-id="c39b2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c39b2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c39b2-105">Recuperar um [ícone de aplicativo do Teams](../resources/teamsappicon.md) associado a uma [definição específica](../resources/teamsappdefinition.md) de um [aplicativo](../resources/teamsapp.md).</span><span class="sxs-lookup"><span data-stu-id="c39b2-105">Retrieve a [Teams app icon](../resources/teamsappicon.md) associated with a specific [definition](../resources/teamsappdefinition.md) of an [app](../resources/teamsapp.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c39b2-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="c39b2-106">Permissions</span></span>

<span data-ttu-id="c39b2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c39b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c39b2-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c39b2-109">Permission Type</span></span>                        | <span data-ttu-id="c39b2-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c39b2-110">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="c39b2-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c39b2-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c39b2-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="c39b2-112">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="c39b2-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c39b2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c39b2-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c39b2-114">Not supported.</span></span>                                                   |
| <span data-ttu-id="c39b2-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c39b2-115">Application</span></span>                            | <span data-ttu-id="c39b2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c39b2-116">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="c39b2-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c39b2-117">HTTP request</span></span>

<span data-ttu-id="c39b2-118">**Obter ícone de cor de uma definição de aplicativo do Teams**</span><span class="sxs-lookup"><span data-stu-id="c39b2-118">**Get color icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon
```

<span data-ttu-id="c39b2-119">**Obter o ícone de contorno de uma definição de aplicativo do Teams**</span><span class="sxs-lookup"><span data-stu-id="c39b2-119">**Get outline icon of a Teams app definition**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c39b2-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="c39b2-120">Optional query parameters</span></span>

<span data-ttu-id="c39b2-121">Esta operação dá suporte aos `$select` `$expand` [parâmetros de consulta e OData](/graph/query-parameters) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="c39b2-121">This operation supports the `$select` and `$expand` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c39b2-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c39b2-122">Request headers</span></span>

| <span data-ttu-id="c39b2-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c39b2-123">Header</span></span>           | <span data-ttu-id="c39b2-124">Valor</span><span class="sxs-lookup"><span data-stu-id="c39b2-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="c39b2-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="c39b2-125">Authorization</span></span>    | <span data-ttu-id="c39b2-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c39b2-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c39b2-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c39b2-128">Request body</span></span>

<span data-ttu-id="c39b2-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="c39b2-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c39b2-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="c39b2-130">Response</span></span>

<span data-ttu-id="c39b2-131">Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [teamsAppIcon](../resources/teamsappicon.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c39b2-131">If successful, this method returns a `200 OK` response code and a [teamsAppIcon](../resources/teamsappicon.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c39b2-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="c39b2-132">Examples</span></span>

### <a name="example-1-get-color-icon-of-a-custom-teams-app"></a><span data-ttu-id="c39b2-133">Exemplo 1: Obter ícone de cor de um *aplicativo* personalizado do Teams</span><span class="sxs-lookup"><span data-stu-id="c39b2-133">Example 1: Get color icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="c39b2-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c39b2-134">Request</span></span>

<span data-ttu-id="c39b2-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c39b2-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_coloricon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon
```

#### <a name="response"></a><span data-ttu-id="c39b2-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c39b2-136">Response</span></span>

<span data-ttu-id="c39b2-137">O exemplo a seguir mostra a resposta para um aplicativo organizacional.</span><span class="sxs-lookup"><span data-stu-id="c39b2-137">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="c39b2-138">**Observação**: acessar a imagem real [do](teamworkhostedcontent-get.md) ícone do aplicativo personalizado exige que um token do Microsoft Graph seja definido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c39b2-138">**Note**: Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/$entity",
    "id": "aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "webUrl": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/$value"
}
```

### <a name="example-2-get-outline-icon-of-a-custom-teams-app"></a><span data-ttu-id="c39b2-139">Exemplo 2: Obter o ícone de contorno de um *aplicativo* personalizado do Teams</span><span class="sxs-lookup"><span data-stu-id="c39b2-139">Example 2: Get outline icon of a *custom* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="c39b2-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c39b2-140">Request</span></span>

<span data-ttu-id="c39b2-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c39b2-141">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_customapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon
```

#### <a name="response"></a><span data-ttu-id="c39b2-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c39b2-142">Response</span></span>

<span data-ttu-id="c39b2-143">O exemplo a seguir mostra a resposta para um aplicativo organizacional.</span><span class="sxs-lookup"><span data-stu-id="c39b2-143">The following example shows the response for an organizational app.</span></span> 
> <span data-ttu-id="c39b2-144">**Observação**: acessar a imagem real [do](teamworkhostedcontent-get.md) ícone do aplicativo personalizado exige que um token do Microsoft Graph seja definido na solicitação.</span><span class="sxs-lookup"><span data-stu-id="c39b2-144">**Note**:  Accessing the actual [image of the custom app's icon](teamworkhostedcontent-get.md) requires a Microsoft Graph token to be set on the request.</span></span>


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/outlineIcon/$entity",
    "id": "aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWIxYzU0Mzg0NGE5ZmFjY2Y2YWI4NDdkNWY0NTU0ZGU0L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "webUrl": "https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value"
}
```


### <a name="example-3-get-color-icon-of-a-store-teams-app"></a><span data-ttu-id="c39b2-145">Exemplo 3: Obter ícone de cor de um *aplicativo do* Teams da loja</span><span class="sxs-lookup"><span data-stu-id="c39b2-145">Example 3: Get color icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="c39b2-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c39b2-146">Request</span></span>

<span data-ttu-id="c39b2-147">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c39b2-147">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/colorIcon/
```


#### <a name="response"></a><span data-ttu-id="c39b2-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="c39b2-148">Response</span></span>

<span data-ttu-id="c39b2-149">O exemplo a seguir mostra a resposta para um aplicativo da loja.</span><span class="sxs-lookup"><span data-stu-id="c39b2-149">The following example shows the response for a store app.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://canary.graph.microsoft.com/testprodbetateamsgraphdev/$metadata#appCatalogs/teamsApps('95de633a-083e-42f5-b444-a4295d8e9314')/appDefinitions('OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk')/colorIcon/$entity",
    "id": "aHR0cHM6Ly9zdGF0aWNzLnRlYW1zLmNkbi5vZmZpY2UubmV0L2V2ZXJncmVlbi1hc3NldHMvYXBwcy85NWRlNjMzYS0wODNlLTQyZjUtYjQ0NC1hNDI5NWQ4ZTkzMTRfbGFyZ2VJbWFnZS5wbmc/dj0xLjAuNQ==",
    "webUrl": "https://statics.teams.cdn.office.net/evergreen-assets/apps/95de633a-083e-42f5-b444-a4295d8e9314_largeImage.png?v=1.0.5"
}
```

### <a name="example-4-get-outline-icon-of-a-store-teams-app"></a><span data-ttu-id="c39b2-150">Exemplo 4: Obter o ícone de contorno de um *aplicativo do* Teams da loja</span><span class="sxs-lookup"><span data-stu-id="c39b2-150">Example 4: Get outline icon of a *store* Teams app</span></span>

#### <a name="request"></a><span data-ttu-id="c39b2-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c39b2-151">Request</span></span>

<span data-ttu-id="c39b2-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="c39b2-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_teamsappicon_outlineicon_publicapp"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/95de633a-083e-42f5-b444-a4295d8e9314/appDefinitions/OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk/outlineIcon/
```


#### <a name="response"></a><span data-ttu-id="c39b2-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="c39b2-153">Response</span></span>

<span data-ttu-id="c39b2-154">O exemplo a seguir mostra a resposta para um aplicativo da loja.</span><span class="sxs-lookup"><span data-stu-id="c39b2-154">The following example shows the response for a store app.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamsAppIcon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('95de633a-083e-42f5-b444-a4295d8e9314')/appDefinitions('OTVkZTYzM2EtMDgzZS00MmY1LWI0NDQtYTQyOTVkOGU5MzE0IyMxLjAuNSMjUHVibGlzaGVk')/outlineIcon/$entity",
    "id": "aHR0cHM6Ly9zdGF0aWNzLnRlYW1zLmNkbi5vZmZpY2UubmV0L2V2ZXJncmVlbi1hc3NldHMvYXBwcy85NWRlNjMzYS0wODNlLTQyZjUtYjQ0NC1hNDI5NWQ4ZTkzMTRfc21hbGxJbWFnZS5wbmc/dj0xLjAuNQ==",
    "webUrl": "https://statics.teams.cdn.office.net/evergreen-assets/apps/95de633a-083e-42f5-b444-a4295d8e9314_smallImage.png?v=1.0.5"
}
```

## <a name="see-also"></a><span data-ttu-id="c39b2-155">Confira também</span><span class="sxs-lookup"><span data-stu-id="c39b2-155">See also</span></span>

- [<span data-ttu-id="c39b2-156">Obter conteúdo hospedado no ícone do aplicativo</span><span class="sxs-lookup"><span data-stu-id="c39b2-156">Get hosted content in app's icon</span></span>](teamworkhostedcontent-get.md)
- [<span data-ttu-id="c39b2-157">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="c39b2-157">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
