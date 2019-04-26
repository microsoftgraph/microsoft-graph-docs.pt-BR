---
title: Listar compartilhados
description: Informações calculadas que retornam a lista de arquivos compartilhados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: fd3f784ca48c408b8616faaa965b327aec48c538
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328529"
---
# <a name="list-shared"></a><span data-ttu-id="1400b-103">Listar compartilhados</span><span class="sxs-lookup"><span data-stu-id="1400b-103">List shared</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1400b-104">Informações calculadas que retornam a lista de arquivos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="1400b-104">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="1400b-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="1400b-105">Permissions</span></span>
<span data-ttu-id="1400b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1400b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1400b-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1400b-108">Permission type</span></span>      | <span data-ttu-id="1400b-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1400b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1400b-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1400b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1400b-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1400b-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="1400b-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1400b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1400b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1400b-113">Not supported.</span></span>    |
|<span data-ttu-id="1400b-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1400b-114">Application</span></span> | <span data-ttu-id="1400b-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1400b-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1400b-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1400b-116">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="1400b-117">A solicitação com uma "ID de usuário" ou "userPrincipalName" só pode ser acessada pelo usuário, e não por outras pessoas:</span><span class="sxs-lookup"><span data-stu-id="1400b-117">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/{id | userPrincipalName}/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1400b-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1400b-118">Optional query parameters</span></span>
<span data-ttu-id="1400b-119">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1400b-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1400b-120">Você pode usar o `$filter` parâmetro de consulta para filtrar itens compartilhados.</span><span class="sxs-lookup"><span data-stu-id="1400b-120">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="1400b-121">Por exemplo, com base no tipo:</span><span class="sxs-lookup"><span data-stu-id="1400b-121">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="1400b-122">ConFira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="1400b-122">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="1400b-123">Você também pode recuperar arquivos compartilhados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="1400b-123">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="1400b-124">Por exemplo, especificando a `lastshared/sharedby/address` Propriedade:</span><span class="sxs-lookup"><span data-stu-id="1400b-124">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="1400b-125">Consulte o tipo complexo [sharingDetail](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="1400b-125">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="1400b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1400b-126">Request headers</span></span>
| <span data-ttu-id="1400b-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1400b-127">Header</span></span>       |  <span data-ttu-id="1400b-128">Valor</span><span class="sxs-lookup"><span data-stu-id="1400b-128">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="1400b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="1400b-129">Authorization</span></span>  | <span data-ttu-id="1400b-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1400b-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1400b-132">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1400b-132">Accept</span></span>  | <span data-ttu-id="1400b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="1400b-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1400b-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1400b-134">Request body</span></span>
<span data-ttu-id="1400b-135">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1400b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1400b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1400b-136">Response</span></span>

<span data-ttu-id="1400b-137">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [compartilhados](../resources/insights-shared.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1400b-137">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1400b-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1400b-138">Example</span></span>

##### <a name="request"></a><span data-ttu-id="1400b-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1400b-139">Request</span></span>

<span data-ttu-id="1400b-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1400b-140">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="1400b-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1400b-141">Response</span></span>

<span data-ttu-id="1400b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1400b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="1400b-145">Expandindo recurso</span><span class="sxs-lookup"><span data-stu-id="1400b-145">Expanding resource</span></span>
<span data-ttu-id="1400b-146">O recurso mencionado por uma percepção compartilhada pode ser expandido.</span><span class="sxs-lookup"><span data-stu-id="1400b-146">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
