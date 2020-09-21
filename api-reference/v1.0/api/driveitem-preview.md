---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
author: JeremyKelley
doc_type: apiPageType
ms.openlocfilehash: 5fea16ce14e2df4b87ddc2b3f9246dfe758ec5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48073261"
---
# <a name="driveitem-preview"></a><span data-ttu-id="a1497-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="a1497-103">driveItem: preview</span></span>

<span data-ttu-id="a1497-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1497-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a1497-105">Esta ação permite que você obtenha uma URL incorporável de curta duração para um item a fim de renderizar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="a1497-105">This action allows you to obtain a short-lived embeddable URL for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="a1497-106">Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.</span><span class="sxs-lookup"><span data-stu-id="a1497-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="a1497-107">**Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="a1497-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="a1497-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1497-109">Permissions</span></span>

<span data-ttu-id="a1497-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a1497-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a1497-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1497-112">Permission type</span></span>                        | <span data-ttu-id="a1497-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1497-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="a1497-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1497-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="a1497-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1497-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="a1497-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1497-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1497-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1497-117">Not supported.</span></span>
| <span data-ttu-id="a1497-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1497-118">Application</span></span>                            | <span data-ttu-id="a1497-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1497-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a1497-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1497-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="a1497-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1497-121">Request body</span></span>

<span data-ttu-id="a1497-122">O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="a1497-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="a1497-123">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="a1497-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="a1497-124">Nome</span><span class="sxs-lookup"><span data-stu-id="a1497-124">Name</span></span>      |  <span data-ttu-id="a1497-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1497-125">Type</span></span>         | <span data-ttu-id="a1497-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1497-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="a1497-127">page</span><span class="sxs-lookup"><span data-stu-id="a1497-127">page</span></span>        | <span data-ttu-id="a1497-128">Cadeia de caracteres/número</span><span class="sxs-lookup"><span data-stu-id="a1497-128">string/number</span></span> | <span data-ttu-id="a1497-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a1497-129">Optional.</span></span> <span data-ttu-id="a1497-130">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="a1497-130">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="a1497-131">Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="a1497-131">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="a1497-132">zoom</span><span class="sxs-lookup"><span data-stu-id="a1497-132">zoom</span></span>        | <span data-ttu-id="a1497-133">number</span><span class="sxs-lookup"><span data-stu-id="a1497-133">number</span></span>        | <span data-ttu-id="a1497-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="a1497-134">Optional.</span></span> <span data-ttu-id="a1497-135">Nível de zoom para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="a1497-135">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="a1497-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1497-136">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="a1497-137">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="a1497-137">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="a1497-138">Nome</span><span class="sxs-lookup"><span data-stu-id="a1497-138">Name</span></span>           | <span data-ttu-id="a1497-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1497-139">Type</span></span>   | <span data-ttu-id="a1497-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1497-140">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="a1497-141">getUrl</span><span class="sxs-lookup"><span data-stu-id="a1497-141">getUrl</span></span>         | <span data-ttu-id="a1497-142">string</span><span class="sxs-lookup"><span data-stu-id="a1497-142">string</span></span> | <span data-ttu-id="a1497-143">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="a1497-143">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="a1497-144">postUrl</span><span class="sxs-lookup"><span data-stu-id="a1497-144">postUrl</span></span>        | <span data-ttu-id="a1497-145">string</span><span class="sxs-lookup"><span data-stu-id="a1497-145">string</span></span> | <span data-ttu-id="a1497-146">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="a1497-146">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="a1497-147">postparameters</span><span class="sxs-lookup"><span data-stu-id="a1497-147">postParameters</span></span> | <span data-ttu-id="a1497-148">string</span><span class="sxs-lookup"><span data-stu-id="a1497-148">string</span></span> | <span data-ttu-id="a1497-149">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="a1497-149">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="a1497-150">GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="a1497-150">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="a1497-151">postparameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded` e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="a1497-151">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="a1497-152">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="a1497-152">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="a1497-153">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="a1497-153">Page/zoom</span></span>

<span data-ttu-id="a1497-154">As opções de ' página ' e ' Zoom ' podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="a1497-154">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>

