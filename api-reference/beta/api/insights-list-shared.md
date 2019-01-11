---
title: Lista compartilhada
description: Percepção calculada que retorna a lista de arquivos compartilhados com um usuário.
author: simonhult
localization_priority: Normal
ms.openlocfilehash: eb9d0165d61559d5f31af486b96e1127c9c7c43c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843264"
---
# <a name="list-shared"></a><span data-ttu-id="ab051-103">Lista compartilhada</span><span class="sxs-lookup"><span data-stu-id="ab051-103">List shared</span></span>

> <span data-ttu-id="ab051-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ab051-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab051-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ab051-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ab051-106">Percepção calculada que retorna a lista de arquivos compartilhados com um usuário.</span><span class="sxs-lookup"><span data-stu-id="ab051-106">Calculated insight that returns the list of files shared with a user.</span></span>

## <a name="permissions"></a><span data-ttu-id="ab051-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="ab051-107">Permissions</span></span>
<span data-ttu-id="ab051-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ab051-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab051-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ab051-110">Permission type</span></span>      | <span data-ttu-id="ab051-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ab051-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ab051-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ab051-112">Delegated (work or school account)</span></span> | <span data-ttu-id="ab051-113">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab051-113">Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="ab051-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ab051-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ab051-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ab051-115">Not supported.</span></span>    |
|<span data-ttu-id="ab051-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ab051-116">Application</span></span> | <span data-ttu-id="ab051-117">Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab051-117">Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ab051-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ab051-118">HTTP request</span></span>
```http
GET /me/insights/shared
```
<span data-ttu-id="ab051-119">Solicitar com uma id de usuário' ' ou 'userPrincipalName' só está acessível pelo usuário, e não por qualquer pessoa:</span><span class="sxs-lookup"><span data-stu-id="ab051-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user, not by anyone else:</span></span>
```http
GET /users/<id | userPrincipalName>/insights/shared
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ab051-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ab051-120">Optional query parameters</span></span>
<span data-ttu-id="ab051-121">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ab051-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="ab051-122">Você pode usar o `$filter` consulta parâmetro para filtrar itens compartilhados.</span><span class="sxs-lookup"><span data-stu-id="ab051-122">You can use the `$filter` query parameter to filter shared items.</span></span> <span data-ttu-id="ab051-123">Por exemplo, com base no tipo:</span><span class="sxs-lookup"><span data-stu-id="ab051-123">For example, based on Type:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=ResourceVisualization/Type eq 'PowerPoint'`

<span data-ttu-id="ab051-124">Consulte os tipos de contêiner e os tipos que você pode filtrar por em [resourceVisualization](../resources/insights-resourcevisualization.md)a disponíveis.</span><span class="sxs-lookup"><span data-stu-id="ab051-124">See the available Container Types and Types you can filter by in [resourceVisualization](../resources/insights-resourcevisualization.md).</span></span>

<span data-ttu-id="ab051-125">Também é possível recuperar arquivos compartilhados por um usuário específico.</span><span class="sxs-lookup"><span data-stu-id="ab051-125">You can also retrieve files shared by a specific user.</span></span> <span data-ttu-id="ab051-126">Por exemplo, especificando o `lastshared/sharedby/address` propriedade:</span><span class="sxs-lookup"><span data-stu-id="ab051-126">For example, by specifying the `lastshared/sharedby/address` property:</span></span>

`https://graph.microsoft.com/beta/me/insights/shared?$filter=lastshared/sharedby/address eq 'kellygraham@contoso.com'`

<span data-ttu-id="ab051-127">Consulte o tipo de [sharingDetail](../resources/insights-sharingdetail.md) complexo.</span><span class="sxs-lookup"><span data-stu-id="ab051-127">See the [sharingDetail](../resources/insights-sharingdetail.md) complex type.</span></span>


## <a name="request-headers"></a><span data-ttu-id="ab051-128">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ab051-128">Request headers</span></span>
| <span data-ttu-id="ab051-129">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ab051-129">Header</span></span>       |  <span data-ttu-id="ab051-130">Valor</span><span class="sxs-lookup"><span data-stu-id="ab051-130">Value</span></span>|
|:-------------|:------|
| <span data-ttu-id="ab051-131">Autorização</span><span class="sxs-lookup"><span data-stu-id="ab051-131">Authorization</span></span>  | <span data-ttu-id="ab051-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ab051-p105">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="ab051-134">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ab051-134">Accept</span></span>  | <span data-ttu-id="ab051-135">application/json</span><span class="sxs-lookup"><span data-stu-id="ab051-135">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab051-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ab051-136">Request body</span></span>
<span data-ttu-id="ab051-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ab051-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ab051-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab051-138">Response</span></span>

<span data-ttu-id="ab051-139">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma lista de itens [compartilhados](../resources/insights-shared.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ab051-139">If successful, this method returns a `200 OK` response code and a list of [shared](../resources/insights-shared.md) items in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ab051-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ab051-140">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ab051-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ab051-141">Request</span></span>

<span data-ttu-id="ab051-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ab051-142">Here is an example of the request.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared
```

##### <a name="response"></a><span data-ttu-id="ab051-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ab051-143">Response</span></span>

<span data-ttu-id="ab051-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ab051-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

### <a name="expanding-resource"></a><span data-ttu-id="ab051-147">A expansão de recurso</span><span class="sxs-lookup"><span data-stu-id="ab051-147">Expanding resource</span></span>
<span data-ttu-id="ab051-148">O recurso referenciado por um insight compartilhado pode ser expandido.</span><span class="sxs-lookup"><span data-stu-id="ab051-148">The resource referenced by a shared insight can be expanded.</span></span>
```http
GET https://graph.microsoft.com/beta/me/insights/shared/{id}/resource
```
