---
title: Obter o trabalho em equipeHostedContent
description: Recupere o conteúdo hospedado em um teamsAppIcon.
localization_priority: Normal
author: jecha
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6317cac369ad8d7bb29ed83c7e2c5ce9a0ca5f5f
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/06/2021
ms.locfileid: "52788000"
---
# <a name="get-teamworkhostedcontent"></a><span data-ttu-id="214aa-103">Obter o trabalho em equipeHostedContent</span><span class="sxs-lookup"><span data-stu-id="214aa-103">Get teamworkHostedContent</span></span>

<span data-ttu-id="214aa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="214aa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="214aa-105">Recupere o [conteúdo hospedado](../resources/teamworkhostedcontent.md) no ícone de [um aplicativo.](../resources/teamsappicon.md)</span><span class="sxs-lookup"><span data-stu-id="214aa-105">Retrieve the [hosted content](../resources/teamworkhostedcontent.md) in an [app's icon](../resources/teamsappicon.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="214aa-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="214aa-106">Permissions</span></span>

<span data-ttu-id="214aa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="214aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

### <a name="permissions-for-app-icon-in-app-catalog"></a><span data-ttu-id="214aa-109">Permissões para ícone de aplicativo no catálogo de aplicativos</span><span class="sxs-lookup"><span data-stu-id="214aa-109">Permissions for app icon in app catalog</span></span>
| <span data-ttu-id="214aa-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="214aa-110">Permission Type</span></span>                        | <span data-ttu-id="214aa-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="214aa-111">Permissions (from least to most privileged)</span></span>                      |
| :------------------------------------- | :--------------------------------------------------------------- |
| <span data-ttu-id="214aa-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="214aa-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="214aa-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="214aa-113">AppCatalog.Read.All, AppCatalog.ReadWrite.All, AppCatalog.Submit</span></span> |
| <span data-ttu-id="214aa-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="214aa-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="214aa-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="214aa-115">Not supported.</span></span>                                                   |
| <span data-ttu-id="214aa-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="214aa-116">Application</span></span>                            | <span data-ttu-id="214aa-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="214aa-117">Not supported.</span></span>                                                   |

## <a name="http-request"></a><span data-ttu-id="214aa-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="214aa-118">HTTP request</span></span>

<span data-ttu-id="214aa-119">**Obter conteúdo hospedado no ícone do aplicativo no catálogo de aplicativos**</span><span class="sxs-lookup"><span data-stu-id="214aa-119">**Get hosted content in app icon in app catalog**</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/colorIcon/hostedContent/$value
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/
GET /appCatalogs/teamsApps/{teams-app-id}/appDefinitions/{app-definition-id}/outlineIcon/hostedContent/$value
```

## <a name="optional-query-parameters"></a><span data-ttu-id="214aa-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="214aa-120">Optional query parameters</span></span>

<span data-ttu-id="214aa-121">Essa operação dá suporte aos `$select` [parâmetros de consulta OData](/graph/query-parameter) para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="214aa-121">This operation supports the `$select` [OData query parameters](/graph/query-parameter) to customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="214aa-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="214aa-122">Request headers</span></span>

| <span data-ttu-id="214aa-123">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="214aa-123">Header</span></span>           | <span data-ttu-id="214aa-124">Valor</span><span class="sxs-lookup"><span data-stu-id="214aa-124">Value</span></span>                      |
| :--------------- | :------------------------- |
| <span data-ttu-id="214aa-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="214aa-125">Authorization</span></span>    | <span data-ttu-id="214aa-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="214aa-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="214aa-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="214aa-128">Request body</span></span>

<span data-ttu-id="214aa-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="214aa-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="214aa-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="214aa-130">Response</span></span>

<span data-ttu-id="214aa-131">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [teamworkHostedContent](../resources/teamworkhostedcontent.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="214aa-131">If successful, this method returns a `200 OK` response code and a [teamworkHostedContent](../resources/teamworkhostedcontent.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="214aa-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="214aa-132">Examples</span></span>

### <a name="example-1-get-the-bytes-of-the-hosted-content-of-the-color-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="214aa-133">Exemplo 1: Obter os bytes do conteúdo hospedado do ícone de cor de um Teams no catálogo</span><span class="sxs-lookup"><span data-stu-id="214aa-133">Example 1: Get the bytes of the hosted content of the color icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="214aa-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="214aa-134">Request</span></span>

<span data-ttu-id="214aa-135">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="214aa-135">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="214aa-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="214aa-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontent_coloricon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/colorIcon/hostedContent/
```
# <a name="c"></a>[<span data-ttu-id="214aa-137">C#</span><span class="sxs-lookup"><span data-stu-id="214aa-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamsappicon-get-hostedcontent-coloricon-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="214aa-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="214aa-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamsappicon-get-hostedcontent-coloricon-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="214aa-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="214aa-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/teamsappicon-get-hostedcontent-coloricon-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="214aa-140">Java</span><span class="sxs-lookup"><span data-stu-id="214aa-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamsappicon-get-hostedcontent-coloricon-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



#### <a name="response"></a><span data-ttu-id="214aa-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="214aa-141">Response</span></span>

<span data-ttu-id="214aa-142">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="214aa-142">The following example shows the response.</span></span>

> <span data-ttu-id="214aa-143">**Observação:** `contentBytes` e `contentType` são sempre definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="214aa-143">**Note:** `contentBytes` and `contentType` are always set to null.</span></span>
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

### <a name="example-2-get-the-bytes-of-the-hosted-content-of-the-outline-icon-of-a-teams-app-in-the-catalog"></a><span data-ttu-id="214aa-144">Exemplo 2: Obter os bytes do conteúdo hospedado do ícone de Teams de um aplicativo de Teams no catálogo</span><span class="sxs-lookup"><span data-stu-id="214aa-144">Example 2: Get the bytes of the hosted content of the outline icon of a Teams app in the catalog</span></span>

#### <a name="request"></a><span data-ttu-id="214aa-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="214aa-145">Request</span></span>

<span data-ttu-id="214aa-146">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="214aa-146">The following is an example of the request.</span></span>

> <span data-ttu-id="214aa-147">**Observação:** As solicitações para o valor bruto não suportam [parâmetros de](/graph/query-parameters) consulta OData para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="214aa-147">**Note:** Requests for the raw value does not support [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


# <a name="http"></a>[<span data-ttu-id="214aa-148">HTTP</span><span class="sxs-lookup"><span data-stu-id="214aa-148">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "teamsappicon_get_hostedcontentbytes_outlineicon_value"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps/5a31d4f7-a11d-4052-96eb-1b40786a2a78/appDefinitions/NWEzMWQ0ZjctYTExZC00MDUyLTk2ZWItMWI0MDc4NmEyYTc4IyM2LjAuNSMjUHVibGlzaGVk/outlineIcon/hostedContent/$value
```
# <a name="c"></a>[<span data-ttu-id="214aa-149">C#</span><span class="sxs-lookup"><span data-stu-id="214aa-149">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/teamsappicon-get-hostedcontentbytes-outlineicon-value-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="214aa-150">JavaScript</span><span class="sxs-lookup"><span data-stu-id="214aa-150">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/teamsappicon-get-hostedcontentbytes-outlineicon-value-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="214aa-151">Objective-C</span><span class="sxs-lookup"><span data-stu-id="214aa-151">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/teamsappicon-get-hostedcontentbytes-outlineicon-value-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="214aa-152">Java</span><span class="sxs-lookup"><span data-stu-id="214aa-152">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/teamsappicon-get-hostedcontentbytes-outlineicon-value-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="214aa-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="214aa-153">Response</span></span>

<span data-ttu-id="214aa-154">A resposta contém bytes para o conteúdo hospedado no corpo.</span><span class="sxs-lookup"><span data-stu-id="214aa-154">Response contains bytes for the hosted content in the body.</span></span> <span data-ttu-id="214aa-155">`content-type` o header especifica o tipo de conteúdo hospedado.</span><span class="sxs-lookup"><span data-stu-id="214aa-155">`content-type` header specifies the kind of hosted content.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: image/png
```

## <a name="see-also"></a><span data-ttu-id="214aa-156">Confira também</span><span class="sxs-lookup"><span data-stu-id="214aa-156">See also</span></span>

- [<span data-ttu-id="214aa-157">Obter ícones de um Teams aplicativo</span><span class="sxs-lookup"><span data-stu-id="214aa-157">Get icons of a Teams app</span></span>](teamsappicon-get.md)
- [<span data-ttu-id="214aa-158">Listar aplicativos no catálogo</span><span class="sxs-lookup"><span data-stu-id="214aa-158">List apps in catalog</span></span>](appcatalogs-list-teamsapps.md)
