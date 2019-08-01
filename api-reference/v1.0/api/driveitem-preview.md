---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: apiPageType
ms.openlocfilehash: 1de53b8183f4277c0241a08822ef539613b83a45
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36015338"
---
# <a name="driveitem-preview"></a><span data-ttu-id="1cd0d-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="1cd0d-103">driveItem: preview</span></span>

<span data-ttu-id="1cd0d-104">Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="1cd0d-105">Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="1cd0d-106">**Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="1cd0d-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="1cd0d-108">Permissions</span></span>

<span data-ttu-id="1cd0d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1cd0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="1cd0d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1cd0d-111">Permission type</span></span>                        | <span data-ttu-id="1cd0d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1cd0d-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="1cd0d-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1cd0d-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="1cd0d-114">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1cd0d-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="1cd0d-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1cd0d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1cd0d-116">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="1cd0d-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="1cd0d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1cd0d-117">Application</span></span>                            | <span data-ttu-id="1cd0d-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="1cd0d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1cd0d-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="1cd0d-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1cd0d-120">Request body</span></span>

<span data-ttu-id="1cd0d-121">O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="1cd0d-122">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="1cd0d-123">Nome</span><span class="sxs-lookup"><span data-stu-id="1cd0d-123">Name</span></span>      |  <span data-ttu-id="1cd0d-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd0d-124">Type</span></span>         | <span data-ttu-id="1cd0d-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd0d-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="1cd0d-126">page</span><span class="sxs-lookup"><span data-stu-id="1cd0d-126">page</span></span>        | <span data-ttu-id="1cd0d-127">Cadeia de caracteres/número</span><span class="sxs-lookup"><span data-stu-id="1cd0d-127">string/number</span></span> | <span data-ttu-id="1cd0d-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-128">Optional.</span></span> <span data-ttu-id="1cd0d-129">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="1cd0d-130">Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="1cd0d-131">zoom</span><span class="sxs-lookup"><span data-stu-id="1cd0d-131">zoom</span></span>        | <span data-ttu-id="1cd0d-132">number</span><span class="sxs-lookup"><span data-stu-id="1cd0d-132">number</span></span>        | <span data-ttu-id="1cd0d-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-133">Optional.</span></span> <span data-ttu-id="1cd0d-134">Nível de zoom para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="1cd0d-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="1cd0d-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="1cd0d-136">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="1cd0d-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="1cd0d-137">Nome</span><span class="sxs-lookup"><span data-stu-id="1cd0d-137">Name</span></span>           | <span data-ttu-id="1cd0d-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="1cd0d-138">Type</span></span>   | <span data-ttu-id="1cd0d-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="1cd0d-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="1cd0d-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="1cd0d-140">getUrl</span></span>         | <span data-ttu-id="1cd0d-141">string</span><span class="sxs-lookup"><span data-stu-id="1cd0d-141">string</span></span> | <span data-ttu-id="1cd0d-142">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="1cd0d-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="1cd0d-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="1cd0d-143">postUrl</span></span>        | <span data-ttu-id="1cd0d-144">string</span><span class="sxs-lookup"><span data-stu-id="1cd0d-144">string</span></span> | <span data-ttu-id="1cd0d-145">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="1cd0d-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="1cd0d-146">postparameters</span><span class="sxs-lookup"><span data-stu-id="1cd0d-146">postParameters</span></span> | <span data-ttu-id="1cd0d-147">string</span><span class="sxs-lookup"><span data-stu-id="1cd0d-147">string</span></span> | <span data-ttu-id="1cd0d-148">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="1cd0d-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="1cd0d-149">GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="1cd0d-150">postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="1cd0d-151">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="1cd0d-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="1cd0d-152">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="1cd0d-152">Page/zoom</span></span>

<span data-ttu-id="1cd0d-153">As opções de ' página ' e ' Zoom ' podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="1cd0d-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
