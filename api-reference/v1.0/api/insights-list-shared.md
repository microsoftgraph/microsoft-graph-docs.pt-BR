---
title: Listar compartilhados
description: Visão calculada que retorna a lista de arquivos compartilhados com um usuário.
author: simonhult
localization_priority: Normal
ms.prod: insights
doc_type: apiPageType
ms.openlocfilehash: 8aa3267de5373e0f75f73851c4d995cbb29cd8bf
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39844327"
---
# <a name="list-shared"></a><span data-ttu-id="d35f5-103">Listar compartilhados</span><span class="sxs-lookup"><span data-stu-id="d35f5-103">List shared</span></span>

<span data-ttu-id="d35f5-104">Informações calculadas que incluem a lista de documentos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="d35f5-104">Calculated insight that includes the list of documents shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="d35f5-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="d35f5-105">Permissions</span></span>
<span data-ttu-id="d35f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d35f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d35f5-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d35f5-108">Permission type</span></span>      | <span data-ttu-id="d35f5-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d35f5-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d35f5-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d35f5-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d35f5-111">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d35f5-111">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="d35f5-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d35f5-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d35f5-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d35f5-113">Not supported.</span></span>    |
|<span data-ttu-id="d35f5-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d35f5-114">Application</span></span> | <span data-ttu-id="d35f5-115">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d35f5-115">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d35f5-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d35f5-116">HTTP request</span></span>
<span data-ttu-id="d35f5-117">Obter uma lista de documentos compartilhados com o usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="d35f5-117">Get a list of documents shared with the signed-in user.</span></span>

><span data-ttu-id="d35f5-118">**Observação**: somente o usuário pode fazer solicitações usando a ID do usuário ou o nome principal.</span><span class="sxs-lookup"><span data-stu-id="d35f5-118">**Note**: Only the user can make requests using the user's id or principal name.</span></span>

```http
GET /me/insights/shared
GET /users/{id | userPrincipalName}/insights/shared
```

<span data-ttu-id="d35f5-119">Expanda o recurso mencionado por uma percepção **compartilhada** :</span><span class="sxs-lookup"><span data-stu-id="d35f5-119">Expand the resource referenced by a **shared** insight:</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared/{id}/resource
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d35f5-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="d35f5-120">Optional query parameters</span></span>
<span data-ttu-id="d35f5-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="d35f5-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="d35f5-122">Você pode usar o `$filter` parâmetro de consulta para filtrar itens compartilhados.</span><span class="sxs-lookup"><span data-stu-id="d35f5-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="d35f5-123">Por exemplo, com base no **tipo**:</span><span class="sxs-lookup"><span data-stu-id="d35f5-123">For example, based on **type**:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="d35f5-124">Confira os tipos e tipos de contêiner disponíveis que você pode filtrar no [resourceVisualization](../resources/insights-resourcevisualization.md).</span><span class="sxs-lookup"><span data-stu-id="d35f5-124">See the available container types and types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="d35f5-125">Você também pode recuperar arquivos compartilhados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="d35f5-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="d35f5-126">Por exemplo, especificando a `lastshared/sharedby/address` Propriedade:</span><span class="sxs-lookup"><span data-stu-id="d35f5-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/v1.0/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="d35f5-127">Consulte o tipo complexo [sharingDetail](../resources/insights-sharingdetail.md) .</span><span class="sxs-lookup"><span data-stu-id="d35f5-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="d35f5-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d35f5-128">Request headers</span></span>
| <span data-ttu-id="d35f5-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d35f5-129">Header</span></span>       |  <span data-ttu-id="d35f5-130">Valor</span><span class="sxs-lookup"><span data-stu-id="d35f5-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="d35f5-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="d35f5-131">Authorization</span></span>  | <span data-ttu-id="d35f5-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d35f5-p104">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="d35f5-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d35f5-134">Accept</span></span>  | <span data-ttu-id="d35f5-135">application/json</span><span class="sxs-lookup"><span data-stu-id="d35f5-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d35f5-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d35f5-136">Request body</span></span>
<span data-ttu-id="d35f5-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d35f5-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d35f5-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="d35f5-138">Response</span></span>

<span data-ttu-id="d35f5-139">Se tiver êxito, este método retornará `200 OK` um código de resposta e uma lista de itens [compartilhados](../resources/insights-shared.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d35f5-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d35f5-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d35f5-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="d35f5-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d35f5-141">Request</span></span>

<span data-ttu-id="d35f5-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d35f5-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/v1.0/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="d35f5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="d35f5-143">Response</span></span>

<span data-ttu-id="d35f5-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d35f5-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

