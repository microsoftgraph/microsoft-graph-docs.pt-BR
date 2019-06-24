---
title: Obter applicationtemplate
description: Recupere as propriedades e os relacionamentos do objeto applicationtemplate.
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 152c09467253cd09d55acf17732b11414063616a
ms.sourcegitcommit: 7c03131291113c343a98bb0234d31bd4535a4050
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/22/2019
ms.locfileid: "35147881"
---
# <a name="get-applicationtemplate"></a><span data-ttu-id="daa19-103">Obter applicationtemplate</span><span class="sxs-lookup"><span data-stu-id="daa19-103">Get applicationTemplate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="daa19-104">Recupere as propriedades de um [](../resources/applicationtemplate.md) objeto applicationtemplate.</span><span class="sxs-lookup"><span data-stu-id="daa19-104">Retrieve the properties of an [applicationTemplate](../resources/applicationtemplate.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="daa19-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="daa19-105">Permissions</span></span>

<span data-ttu-id="daa19-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="daa19-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="daa19-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="daa19-108">Permission type</span></span>                        | <span data-ttu-id="daa19-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="daa19-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="daa19-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="daa19-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="daa19-111">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="daa19-111">None.</span></span> |
| <span data-ttu-id="daa19-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="daa19-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="daa19-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="daa19-113">Not supported.</span></span> |
| <span data-ttu-id="daa19-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="daa19-114">Application</span></span>                            | <span data-ttu-id="daa19-115">Nenhum.</span><span class="sxs-lookup"><span data-stu-id="daa19-115">None.</span></span> |

<span data-ttu-id="daa19-116">Permissões adicionais não são necessárias para chamar esta API, contanto que seu aplicativo tenha um token de acesso válido para chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="daa19-116">Additional permissions are not required to call this API, as long as your application has a valid access token to call Microsoft Graph.</span></span>

## <a name="http-request"></a><span data-ttu-id="daa19-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="daa19-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applicationTemplates/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="daa19-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="daa19-118">Optional query parameters</span></span>

<span data-ttu-id="daa19-119">Você pode usar um `$select` parâmetro de consulta para especificar apenas as propriedades que você precisa para o melhor desempenho.</span><span class="sxs-lookup"><span data-stu-id="daa19-119">You can use a `$select` query parameter to specify only the properties you need for best performance.</span></span> <span data-ttu-id="daa19-120">A propriedade **id** sempre será retornada.</span><span class="sxs-lookup"><span data-stu-id="daa19-120">The **id** property is always returned.</span></span> 

<span data-ttu-id="daa19-121">Para obter informações gerais, confira [parâmetros de consulta OData](/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="daa19-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="daa19-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="daa19-122">Request headers</span></span>

| <span data-ttu-id="daa19-123">Nome</span><span class="sxs-lookup"><span data-stu-id="daa19-123">Name</span></span>      |<span data-ttu-id="daa19-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="daa19-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="daa19-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="daa19-125">Authorization</span></span> | <span data-ttu-id="daa19-126">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="daa19-126">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="daa19-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="daa19-127">Request body</span></span>

<span data-ttu-id="daa19-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="daa19-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="daa19-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="daa19-129">Response</span></span>

<span data-ttu-id="daa19-130">Se tiver êxito, este método retornará `200 OK` um código de resposta e o objeto [applicationtemplate](../resources/applicationtemplate.md) solicitado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="daa19-130">If successful, this method returns a `200 OK` response code and the requested [applicationTemplate](../resources/applicationtemplate.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="daa19-131">Exemplos</span><span class="sxs-lookup"><span data-stu-id="daa19-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="daa19-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="daa19-132">Request</span></span>

<span data-ttu-id="daa19-133">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="daa19-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_applicationtemplate"
}-->

```http
GET https://graph.microsoft.com/beta/applicationTemplates/{id}
```

### <a name="response"></a><span data-ttu-id="daa19-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="daa19-134">Response</span></span>

<span data-ttu-id="daa19-135">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="daa19-135">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="daa19-136">O objeto de resposta mostrado aqui pode ser reduzido para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="daa19-136">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="daa19-137">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="daa19-137">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.applicationTemplate"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id" : "id-value",
    "displayName" : "displayName-value",
    "homePageUrl" : "homePageUrl-value",
    "supportedSingleSignOnModes" : ["supportedSingleSignOnModes-value"],
    "logoUrl" : "logoUrl-value",
    "categories" : ["categories-value"],
    "publisher" : "publisher-value",
    "description" : "description-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get applicationTemplate",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
