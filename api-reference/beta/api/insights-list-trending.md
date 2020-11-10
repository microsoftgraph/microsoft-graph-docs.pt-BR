---
title: Listar tendências
description: Insights calculados que retornam a lista de itens de tendências do usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 83accede4b6af1f1bbc255f94e9e54fb4de4b90f
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48964631"
---
# <a name="list-trending"></a><span data-ttu-id="fca67-103">Listar tendências</span><span class="sxs-lookup"><span data-stu-id="fca67-103">List trending</span></span>

<span data-ttu-id="fca67-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fca67-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fca67-105">Informação calculada que inclui uma lista de documentos que envolvem a tendência do usuário.</span><span class="sxs-lookup"><span data-stu-id="fca67-105">Calculated insight that includes a list of documents trending around the user.</span></span>

## <a name="permissions"></a><span data-ttu-id="fca67-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="fca67-106">Permissions</span></span>
<span data-ttu-id="fca67-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="fca67-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fca67-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fca67-109">Permission type</span></span>      | <span data-ttu-id="fca67-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="fca67-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fca67-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fca67-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fca67-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca67-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fca67-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fca67-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fca67-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fca67-114">Not supported.</span></span>    |
|<span data-ttu-id="fca67-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fca67-115">Application</span></span> | <span data-ttu-id="fca67-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fca67-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fca67-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fca67-117">HTTP request</span></span>
<span data-ttu-id="fca67-118">Obter uma lista de documentos de tendências em torno do usuário conectado ou do usuário especificado:</span><span class="sxs-lookup"><span data-stu-id="fca67-118">Get a list of documents trending around the signed-in user or specified user:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending
GET /users/{id | userPrincipalName}/insights/trending
```

<span data-ttu-id="fca67-119">Expanda o recurso mencionado por uma visão de **tendências** :</span><span class="sxs-lookup"><span data-stu-id="fca67-119">Expand the resource referenced by a **trending** insight:</span></span>
<!-- { "blockType": "ignored" } -->

```http
GET /me/insights/trending/{id}/resource
GET /users/{id | userPrincipalName}/insights/trending/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fca67-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="fca67-120">Optional query parameters</span></span>
<span data-ttu-id="fca67-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="fca67-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="fca67-122">Você pode usar o `$filter` parâmetro de consulta para filtrar itens de tendência.</span><span class="sxs-lookup"><span data-stu-id="fca67-122">You can use the `$filter` query parameter to filter trending items.</span></span> <span data-ttu-id="fca67-123">Por exemplo, com base no **tipo** :</span><span class="sxs-lookup"><span data-stu-id="fca67-123">For example, based on **type** :</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/type eq 'PowerPoint'`

<span data-ttu-id="fca67-124">Ou com base no **ContainerType** :</span><span class="sxs-lookup"><span data-stu-id="fca67-124">Or based on **containerType** :</span></span>
<!-- { "blockType": "ignored" } -->

`https://graph.microsoft.com/v1.0/me/insights/trending?$filter=ResourceVisualization/containerType eq 'OneDriveBusiness'`

<span data-ttu-id="fca67-125">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="fca67-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>


## <a name="request-headers"></a><span data-ttu-id="fca67-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fca67-126">Request headers</span></span>
| <span data-ttu-id="fca67-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fca67-127">Header</span></span>       |  <span data-ttu-id="fca67-128">Valor</span><span class="sxs-lookup"><span data-stu-id="fca67-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="fca67-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="fca67-129">Authorization</span></span>  | <span data-ttu-id="fca67-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fca67-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="fca67-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fca67-132">Accept</span></span>  | <span data-ttu-id="fca67-133">application/json</span><span class="sxs-lookup"><span data-stu-id="fca67-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fca67-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fca67-134">Request body</span></span>
<span data-ttu-id="fca67-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="fca67-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fca67-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca67-136">Response</span></span>

<span data-ttu-id="fca67-137">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de itens de [tendência](../resources/insights-trending.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fca67-137">If successful, this method returns a `200 OK` response code and a list of [trending](../resources/insights-trending.md) items in the response body.</span></span> <span data-ttu-id="fca67-138">Cada item contém propriedades de visualização para exibir o item em sua experiência.</span><span class="sxs-lookup"><span data-stu-id="fca67-138">Each item contains visualization properties for displaying the item in your experience.</span></span>

<span data-ttu-id="fca67-139">Se as ideias de item do usuário de destino tiverem sido desabilitadas, este método retornará `403 Forbidden` e o seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="fca67-139">If item insights of targeted user have been disabled, this method returns `403 Forbidden` and the following error:</span></span>
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
<span data-ttu-id="fca67-140">Para obter mais detalhes, confira [personalizar política de informações](/graph/insights-customize-item-insights-privacy.md).</span><span class="sxs-lookup"><span data-stu-id="fca67-140">For more details, see [customize insights privacy](/graph/insights-customize-item-insights-privacy.md).</span></span>

## <a name="example"></a><span data-ttu-id="fca67-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fca67-141">Example</span></span>
#### <a name="request"></a><span data-ttu-id="fca67-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fca67-142">Request</span></span>
<span data-ttu-id="fca67-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fca67-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fca67-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="fca67-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_me_trending"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/me/insights/trending
```
# <a name="c"></a>[<span data-ttu-id="fca67-145">C#</span><span class="sxs-lookup"><span data-stu-id="fca67-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-me-trending-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fca67-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fca67-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-me-trending-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fca67-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fca67-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-me-trending-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fca67-148">Java</span><span class="sxs-lookup"><span data-stu-id="fca67-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-me-trending-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="fca67-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="fca67-149">Response</span></span>
<span data-ttu-id="fca67-150">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fca67-150">Here is an example of the response.</span></span> <span data-ttu-id="fca67-151">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="fca67-151">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="fca67-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fca67-152">All of the properties will be returned from an actual call.</span></span> <span data-ttu-id="fca67-153">Veja um exemplo de resposta un truncada na parte inferior da página.</span><span class="sxs-lookup"><span data-stu-id="fca67-153">See an example un-truncated response at the bottom of the page.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trending",
  "name": "get_me_trending"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 801

{
    "value": [
        {
            "id": "id-value",
            "weight": "weight-value",
            "resourceVisualization": {
                "title": "title-value",
                "type": "type-value",
                "mediaType": "mediaType-value",
                "previewImageUrl": "previewImageUrl-value",
                "previewText": "previewText-value",
                "containerWebUrl": "containerWebUrl-value",
                "containerDisplayName": "containerDisplayName-value",
                "containerType": "containerType-value"
            },
            "resourceReference": {
                "webUrl": "webUrl-value",
                "id": "id-value",
                "type": "type-value"
            }
        }
    ]
}
```
