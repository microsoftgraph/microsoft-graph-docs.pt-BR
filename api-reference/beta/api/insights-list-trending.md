---
title: Listar tendências
description: Insights calculados que retornam a lista de itens de tendências do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 5a790c23a0e3cee09079beb5b51151610f309dad
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52040242"
---
# <a name="list-trending"></a><span data-ttu-id="e1665-103">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="e1665-103">List trending</span></span>

<span data-ttu-id="e1665-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e1665-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1665-105">Insights calculados que incluem uma lista de documentos que são tendências ao redor do usuário.</span><span class="sxs-lookup"><span data-stu-id="e1665-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="e1665-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="e1665-106">Permissions</span></span>
<span data-ttu-id="e1665-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e1665-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="e1665-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1665-109">Permission type</span></span>      | <span data-ttu-id="e1665-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e1665-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1665-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1665-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1665-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1665-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="e1665-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1665-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1665-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1665-114">Not supported.</span></span>    |
|<span data-ttu-id="e1665-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1665-115">Application</span></span> | <span data-ttu-id="e1665-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1665-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1665-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1665-117">HTTP request</span></span>
<span data-ttu-id="e1665-118">Obter uma lista de documentos que são tendências em torno do usuário ou usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="e1665-118">Get a list of documents trending around the signed-in user or specified user:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="e1665-119">Expanda o recurso referenciado por **uma visão de tendência:**</span><span class="sxs-lookup"><span data-stu-id="e1665-119">Expand the resource referenced by a **trending** insight:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e1665-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="e1665-120">Optional query parameters</span></span>
<span data-ttu-id="e1665-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="e1665-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="e1665-122">Você pode usar o `$filter` parâmetro de consulta para filtrar itens de tendência.</span><span class="sxs-lookup"><span data-stu-id="e1665-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="e1665-123">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="e1665-123">For example, based on **type**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="e1665-124">Ou com base em **containerType**:</span><span class="sxs-lookup"><span data-stu-id="e1665-124">Or based on **containerType**:</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="e1665-125">Consulte os tipos e tipos de contêiner disponíveis que você pode filtrar em [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="e1665-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="e1665-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1665-126">Request headers</span></span>
| <span data-ttu-id="e1665-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1665-127">Header</span></span>       |  <span data-ttu-id="e1665-128">Valor</span><span class="sxs-lookup"><span data-stu-id="e1665-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="e1665-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1665-129">Authorization</span></span>  | <span data-ttu-id="e1665-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1665-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="e1665-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1665-132">Accept</span></span>  | <span data-ttu-id="e1665-133">application/json</span><span class="sxs-lookup"><span data-stu-id="e1665-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1665-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1665-134">Request body</span></span>
<span data-ttu-id="e1665-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1665-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1665-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1665-136">Response</span></span>

<span data-ttu-id="e1665-137">Se tiver êxito, este método retornará um código de resposta e uma lista de itens `200 OK` [de](../resources/insights-trending.md) tendência no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1665-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="e1665-138">Cada item contém propriedades de visualização para exibir o item em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="e1665-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

<span data-ttu-id="e1665-139">Se as percepções de item do usuário direcionado foram desabilitadas, este método `403 Forbidden` retornará e o seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="e1665-139">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
<!-- { "blockType": "ignored" } -->

```
{
  "error": {
    "code": "ItemInsightsDisabled",
    "message": " The access to the requested resource is denied because item insights are disabled.",
    "innerError": {
      "requestId": "request-id",
      "date": "date-time"
    }
  }
}
```
<span data-ttu-id="e1665-140">Para obter mais detalhes, confira [personalizar política de informações](/graph/insights-customize-item-insights-privacy.md).</span><span class="sxs-lookup"><span data-stu-id="e1665-140">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span>

## <a name="example"></a><span data-ttu-id="e1665-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1665-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="e1665-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1665-142">Request</span></span>
<span data-ttu-id="e1665-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1665-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="e1665-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="e1665-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_trending"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/trending
```
# <a name="c"></a>[<span data-ttu-id="e1665-145">C#</span><span class="sxs-lookup"><span data-stu-id="e1665-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-trending-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e1665-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e1665-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-trending-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e1665-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e1665-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-trending-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e1665-148">Java</span><span class="sxs-lookup"><span data-stu-id="e1665-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-me-trending-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="e1665-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1665-149">Response</span></span>
<span data-ttu-id="e1665-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e1665-150">Here is an example of the response.</span></span> <span data-ttu-id="e1665-151">Observação: o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="e1665-151">Note: The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="e1665-152">Consulte um exemplo de resposta não truncada na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="e1665-152">See an example un-truncated response at the bottom of the page.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending",
  "name": "get_me_trending"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "AWMiSOpKHlJCpP_ZoVJQXi9ees4wFhDQQqF55Pm5DlaMzvtd2zra4UWSTEvpTldvb6EhQ289G4BAsxnrajQyjW1jIkjqSh5SQqT_2aFSUF4vBQ",
      "weight": "0.1583399742569597",
      "resourceVisualization": {
        "title": "LiveCaptions",
        "type": "Image",
        "mediaType": "application/octet-stream",
        "previewImageUrl": "https://contoso.sharepoint.com/_api/v2.0/drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN/thumbnails/0/small/thumbnailContent",
        "previewText": "",
        "containerWebUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared Documents/Go to Market Plan",
        "containerDisplayName": "Mark 8 Project Team",
        "containerType": "Site"
      },
      "resourceReference": {
        "webUrl": "https://contoso.sharepoint.com/sites/Mark8ProjectTeam/Shared%20Documents/Go%20to%20Market%20Plan/LiveCaptions.gif",
        "id": "drives/b!YyJI6koeUkKk_9mhUlBeL156zjAWENBCoXnk-bkOVozO-13bOtrhRZJMS-lOV29v/items/01H273TR5BEFBW6PI3QBALGGPLNI2DFDLN",
        "type": "microsoft.graph.driveItem"
      }
    }
  ]
}
```
