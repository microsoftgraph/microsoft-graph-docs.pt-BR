---
title: Listar compartilhados
description: Visão calculada que retorna a lista de arquivos compartilhados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 1d920ea8f03c77b0f04c5e88e2c07de26a2f403a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42446324"
---
# <a name="list-shared"></a><span data-ttu-id="7e119-103">Listar compartilhados</span><span class="sxs-lookup"><span data-stu-id="7e119-103">List shared</span></span>

<span data-ttu-id="7e119-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="7e119-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e119-105">Informações calculadas que incluem a lista de documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="7e119-105">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="7e119-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="7e119-106">Permissions</span></span>
<span data-ttu-id="7e119-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7e119-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e119-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7e119-109">Permission type</span></span>      | <span data-ttu-id="7e119-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7e119-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7e119-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7e119-111">Delegated (work or school account)</span></span> | <span data-ttu-id="7e119-112">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e119-112">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="7e119-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7e119-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7e119-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7e119-114">Not supported.</span></span>    |
|<span data-ttu-id="7e119-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7e119-115">Application</span></span> | <span data-ttu-id="7e119-116">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7e119-116">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7e119-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7e119-117">HTTP request</span></span>
<span data-ttu-id="7e119-118">Obter uma lista de documentos compartilhados com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="7e119-118">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="7e119-119">**Observação**: somente o usuário pode fazer solicitações usando a ID do usuário ou o nome principal.</span><span class="sxs-lookup"><span data-stu-id="7e119-119">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="7e119-120">Expanda o recurso mencionado por uma percepção **compartilhada** :</span><span class="sxs-lookup"><span data-stu-id="7e119-120">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7e119-121">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="7e119-121">Optional query parameters</span></span>
<span data-ttu-id="7e119-122">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="7e119-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="7e119-123">Você pode usar o `$filter` parâmetro de consulta para filtrar itens compartilhados.</span><span class="sxs-lookup"><span data-stu-id="7e119-123">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="7e119-124">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="7e119-124">For example, based on **type**:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="7e119-125">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="7e119-125">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="7e119-126">Você também pode recuperar arquivos compartilhados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="7e119-126">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="7e119-127">Por exemplo, especificando a `lastshared/sharedby/address` Propriedade:</span><span class="sxs-lookup"><span data-stu-id="7e119-127">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="7e119-128">Consulte o tipo complexo [sharingDetail](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="7e119-128">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="7e119-129">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7e119-129">Request headers</span></span>
| <span data-ttu-id="7e119-130">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7e119-130">Header</span></span>       |  <span data-ttu-id="7e119-131">Valor</span><span class="sxs-lookup"><span data-stu-id="7e119-131">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="7e119-132">Autorização</span><span class="sxs-lookup"><span data-stu-id="7e119-132">Authorization</span></span>  | <span data-ttu-id="7e119-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7e119-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="7e119-135">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7e119-135">Accept</span></span>  | <span data-ttu-id="7e119-136">application/json</span><span class="sxs-lookup"><span data-stu-id="7e119-136">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e119-137">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7e119-137">Request body</span></span>
<span data-ttu-id="7e119-138">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7e119-138">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e119-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e119-139">Response</span></span>

<span data-ttu-id="7e119-140">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [compartilhados](../resources/insights-shared.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7e119-140">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7e119-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7e119-141">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7e119-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7e119-142">Request</span></span>

<span data-ttu-id="7e119-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7e119-143">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="7e119-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7e119-144">Response</span></span>

<span data-ttu-id="7e119-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7e119-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
```http
{
    "value": [
        {   
            "id": "id-value",
            "lastShared" : { 
                "sharedDateTime" : "sharedDateTime-value",  
                "sharingSubject" : "sharingSubject-value",
                "sharingType" : "sharingType-value", 
                "sharedBy" : { 
                    "displayName" : "displayName-value", 
                    "id": "id-value" 
                }
                "sharingReference" : { 
                    "webUrl" : "webUrl-value",
                    "type: "type-value", 
                    "id": "id-value"
                } 
            },
            "resourceVisualization": { 
                "title" : "title-value, 
                "type"  : "type-value",
                "mediaType" : "mediaType-value",
                "previewImageUrl" : previewImageUrl-value, 
                "previewText" : "previewText-value", 
                "containerWebUrl" : "containerWebUrl-value", 
                "containerDisplayName" : "containerDisplayName-value", 
                "containerType" : "containerType-value" 
            }, 
            "resourceReference" : { 
                "webUrl" : "webUrl-value", 
                "id": "id-value", 
                "type: "type-value" 
}
```

