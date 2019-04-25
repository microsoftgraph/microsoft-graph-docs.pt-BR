---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ae5140bf6164aedd051f04c2c43c361f16517e7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32572700"
---
# <a name="driveitem-preview"></a><span data-ttu-id="bed14-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="bed14-103">driveItem: preview</span></span>

<span data-ttu-id="bed14-104">Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="bed14-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="bed14-105">Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.</span><span class="sxs-lookup"><span data-stu-id="bed14-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="bed14-106">**Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="bed14-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="bed14-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="bed14-108">Permissions</span></span>

<span data-ttu-id="bed14-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="bed14-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bed14-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="bed14-111">Permission type</span></span>                        | <span data-ttu-id="bed14-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="bed14-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="bed14-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="bed14-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="bed14-114">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bed14-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="bed14-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="bed14-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bed14-116">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="bed14-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="bed14-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="bed14-117">Application</span></span>                            | <span data-ttu-id="bed14-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="bed14-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="bed14-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bed14-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="bed14-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bed14-120">Request body</span></span>

<span data-ttu-id="bed14-121">O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="bed14-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="bed14-122">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="bed14-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="bed14-123">Nome</span><span class="sxs-lookup"><span data-stu-id="bed14-123">Name</span></span>      |  <span data-ttu-id="bed14-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="bed14-124">Type</span></span>         | <span data-ttu-id="bed14-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed14-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="bed14-126">page</span><span class="sxs-lookup"><span data-stu-id="bed14-126">page</span></span>        | <span data-ttu-id="bed14-127">Cadeia de caracteres/número</span><span class="sxs-lookup"><span data-stu-id="bed14-127">string/number</span></span> | <span data-ttu-id="bed14-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bed14-128">Optional.</span></span> <span data-ttu-id="bed14-129">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="bed14-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="bed14-130">Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="bed14-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="bed14-131">zoom</span><span class="sxs-lookup"><span data-stu-id="bed14-131">zoom</span></span>        | <span data-ttu-id="bed14-132">number</span><span class="sxs-lookup"><span data-stu-id="bed14-132">number</span></span>        | <span data-ttu-id="bed14-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="bed14-133">Optional.</span></span> <span data-ttu-id="bed14-134">Nível de zoom para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="bed14-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="bed14-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="bed14-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="bed14-136">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="bed14-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="bed14-137">Nome</span><span class="sxs-lookup"><span data-stu-id="bed14-137">Name</span></span>           | <span data-ttu-id="bed14-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="bed14-138">Type</span></span>   | <span data-ttu-id="bed14-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="bed14-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="bed14-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="bed14-140">getUrl</span></span>         | <span data-ttu-id="bed14-141">string</span><span class="sxs-lookup"><span data-stu-id="bed14-141">string</span></span> | <span data-ttu-id="bed14-142">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="bed14-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="bed14-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="bed14-143">postUrl</span></span>        | <span data-ttu-id="bed14-144">string</span><span class="sxs-lookup"><span data-stu-id="bed14-144">string</span></span> | <span data-ttu-id="bed14-145">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="bed14-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="bed14-146">postparameters</span><span class="sxs-lookup"><span data-stu-id="bed14-146">postParameters</span></span> | <span data-ttu-id="bed14-147">string</span><span class="sxs-lookup"><span data-stu-id="bed14-147">string</span></span> | <span data-ttu-id="bed14-148">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="bed14-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="bed14-149">GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="bed14-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="bed14-150">postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postaGem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="bed14-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="bed14-151">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="bed14-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="bed14-152">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="bed14-152">Page/zoom</span></span>

<span data-ttu-id="bed14-153">As opções de ' página ' e ' Zoom ' podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ele.</span><span class="sxs-lookup"><span data-stu-id="bed14-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
