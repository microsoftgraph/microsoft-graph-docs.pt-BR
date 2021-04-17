---
title: Obter o trabalho em equipeHostedContent
description: Recupere o conteúdo hospedado em um teamsAppIcon.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1b5fde96ffaad34360603751398473357d82e1fd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882634"
---
# <a name="get-teamworkhostedcontent"></a><span data-ttu-id="d9f73-103">Obter o trabalho em equipeHostedContent</span><span class="sxs-lookup"><span data-stu-id="d9f73-103">Get teamworkHostedContent</span></span>

<span data-ttu-id="d9f73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9f73-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d9f73-105">Recupere o [conteúdo hospedado](../resources/teamworkhostedcontent.md) no ícone de [um aplicativo.](../resources/teamsappicon.md)</span><span class="sxs-lookup"><span data-stu-id="d9f73-105">Retrieve the [hosted content](../resources/teamworkhostedcontent.md) in an [app's icon](../resources/teamsappicon.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="d9f73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="d9f73-106">Permissions</span></span>

<span data-ttu-id="d9f73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9f73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-app-icon-in-app-catalog"></a><span data-ttu-id="d9f73-109">Permissões para ícone de aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="d9f73-109">Permissions for app icon in app catalog</span></span>
| <span data-ttu-id="d9f73-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9f73-110">Permission Type</span></span>                        | <span data-ttu-id="d9f73-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d9f73-111">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="d9f73-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9f73-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="d9f73-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="d9f73-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="d9f73-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9f73-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d9f73-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9f73-115">Not supported.</span></span>                                                   |
| <span data-ttu-id="d9f73-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d9f73-116">Application</span></span>                            | <span data-ttu-id="d9f73-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9f73-117">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="d9f73-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9f73-118">HTTP request</span></span>

<span data-ttu-id="d9f73-119">**Obter conteúdo hospedado no ícone do aplicativo no catálogo de aplicativos**</span><span class="sxs-lookup"><span data-stu-id="d9f73-119">**Get hosted content in app icon in app catalog**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d9f73-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d9f73-120">Optional query parameters</span></span>

<span data-ttu-id="d9f73-121">Essa operação dá suporte aos `$select` [parâmetros de consulta OData](/graph/query-parameter) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9f73-121">This operation supports the `$select` [OData query parameters](/graph/query-parameter) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d9f73-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9f73-122">Request headers</span></span>

| <span data-ttu-id="d9f73-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9f73-123">Header</span></span>           | <span data-ttu-id="d9f73-124">Valor</span><span class="sxs-lookup"><span data-stu-id="d9f73-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="d9f73-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9f73-125">Authorization</span></span>    | <span data-ttu-id="d9f73-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9f73-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d9f73-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9f73-128">Request body</span></span>

<span data-ttu-id="d9f73-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d9f73-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d9f73-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9f73-130">Response</span></span>

<span data-ttu-id="d9f73-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [teamworkHostedContent](../resources/teamworkhostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9f73-131">If successful, this method returns a `200 OK` response code and a [teamworkHostedContent](../resources/teamworkhostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d9f73-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="d9f73-132">Examples</span></span>

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="d9f73-133">Exemplo 1: Obter os bytes do conteúdo hospedado do ícone de cor de um aplicativo do Teams no catálogo</span><span class="sxs-lookup"><span data-stu-id="d9f73-133">Example 1: Get the bytes of the hosted content of the color icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="d9f73-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9f73-134">Request</span></span>

<span data-ttu-id="d9f73-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9f73-135">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```


#### <a name="response"></a><span data-ttu-id="d9f73-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9f73-136">Response</span></span>

<span data-ttu-id="d9f73-137">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9f73-137">The following example shows the response.</span></span>

> <span data-ttu-id="d9f73-138">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="d9f73-138">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('5a31d4f7-a11d-4052-96eb-1b40786a2a78')/appDefinitions('NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk')/colorIcon/hostedContent/$entity",
    "id": "aWQ9LHR5cGU9MSx1cmw9aHR0cHM6Ly91cy1hcGkuYXNtLnNreXBlLmNvbS92MS9vYmplY3RzLzAtd3VzLWQ0LWQwOGVkNTQ2MjQ2MTliNTc4OGIwMWUzODNlMWVjYzU3L3ZpZXdzL2ltZ3BzaF9mdWxsc2l6ZQ==",
    "contentBytes": null,
    "contentType": null
}
```

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="d9f73-139">Exemplo 2: Obter os bytes do conteúdo hospedado do ícone de contorno de um aplicativo do Teams no catálogo</span><span class="sxs-lookup"><span data-stu-id="d9f73-139">Example 2: Get the bytes of the hosted content of the outline icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="d9f73-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9f73-140">Request</span></span>

<span data-ttu-id="d9f73-141">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9f73-141">The following is an example of the request.</span></span>

> <span data-ttu-id="d9f73-142">**Observação:** As solicitações para o valor bruto não suportam [parâmetros de](/graph/query-parameters) consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d9f73-142">**Note:** Requests for the raw value does not support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>

<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```

#### <a name="response"></a><span data-ttu-id="d9f73-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9f73-143">Response</span></span>

<span data-ttu-id="d9f73-144">A resposta contém bytes para o conteúdo hospedado no corpo.</span><span class="sxs-lookup"><span data-stu-id="d9f73-144">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="d9f73-145">`content-type` o header especifica o tipo de conteúdo hospedado.</span><span class="sxs-lookup"><span data-stu-id="d9f73-145">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.teamworkHostedContent"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a><span data-ttu-id="d9f73-146">Confira também</span><span class="sxs-lookup"><span data-stu-id="d9f73-146">See also</span></span>

- [<span data-ttu-id="d9f73-147">Obter ícones de um aplicativo do Teams</span><span class="sxs-lookup"><span data-stu-id="d9f73-147">Get icons of a Teams app</span></span>](teamsappicon-get.md)
- [<span data-ttu-id="d9f73-148">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="d9f73-148">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
