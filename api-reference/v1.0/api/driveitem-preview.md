---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.
ms.openlocfilehash: 741e449c972ad372aae30d9921cdb3b7fa1fc40d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006331"
---
# <a name="driveitem-preview"></a><span data-ttu-id="6c268-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="6c268-103">driveItem: preview</span></span>

<span data-ttu-id="6c268-104">Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="6c268-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="6c268-105">Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="6c268-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="6c268-106">**Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="6c268-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="6c268-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="6c268-108">Permissions</span></span>

<span data-ttu-id="6c268-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6c268-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c268-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6c268-111">Permission type</span></span>                        | <span data-ttu-id="6c268-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6c268-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="6c268-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6c268-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="6c268-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c268-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="6c268-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6c268-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c268-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c268-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="6c268-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6c268-117">Application</span></span>                            | <span data-ttu-id="6c268-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6c268-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="6c268-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6c268-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="6c268-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6c268-120">Request body</span></span>

<span data-ttu-id="6c268-121">O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="6c268-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="6c268-122">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="6c268-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="6c268-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6c268-123">Name</span></span>      |  <span data-ttu-id="6c268-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c268-124">Type</span></span>         | <span data-ttu-id="6c268-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c268-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="6c268-126">página</span><span class="sxs-lookup"><span data-stu-id="6c268-126">page</span></span>        | <span data-ttu-id="6c268-127">número de sequência de caracteres /</span><span class="sxs-lookup"><span data-stu-id="6c268-127">string/number</span></span> | <span data-ttu-id="6c268-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c268-128">Optional.</span></span> <span data-ttu-id="6c268-129">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="6c268-129">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="6c268-130">Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="6c268-130">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="6c268-131">zoom</span><span class="sxs-lookup"><span data-stu-id="6c268-131">zoom</span></span>        | <span data-ttu-id="6c268-132">número</span><span class="sxs-lookup"><span data-stu-id="6c268-132">number</span></span>        | <span data-ttu-id="6c268-133">Opcional.</span><span class="sxs-lookup"><span data-stu-id="6c268-133">Optional.</span></span> <span data-ttu-id="6c268-134">Amplie o nível para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="6c268-134">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="6c268-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="6c268-135">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="6c268-136">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="6c268-136">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="6c268-137">Nome</span><span class="sxs-lookup"><span data-stu-id="6c268-137">Name</span></span>           | <span data-ttu-id="6c268-138">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c268-138">Type</span></span>   | <span data-ttu-id="6c268-139">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c268-139">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="6c268-140">getUrl</span><span class="sxs-lookup"><span data-stu-id="6c268-140">getUrl</span></span>         | <span data-ttu-id="6c268-141">string</span><span class="sxs-lookup"><span data-stu-id="6c268-141">string</span></span> | <span data-ttu-id="6c268-142">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="6c268-142">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="6c268-143">postUrl</span><span class="sxs-lookup"><span data-stu-id="6c268-143">postUrl</span></span>        | <span data-ttu-id="6c268-144">string</span><span class="sxs-lookup"><span data-stu-id="6c268-144">string</span></span> | <span data-ttu-id="6c268-145">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="6c268-145">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="6c268-146">postParameters</span><span class="sxs-lookup"><span data-stu-id="6c268-146">postParameters</span></span> | <span data-ttu-id="6c268-147">string</span><span class="sxs-lookup"><span data-stu-id="6c268-147">string</span></span> | <span data-ttu-id="6c268-148">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="6c268-148">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="6c268-149">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="6c268-149">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="6c268-150">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="6c268-150">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="6c268-151">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="6c268-151">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="6c268-152">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="6c268-152">Page/zoom</span></span>

<span data-ttu-id="6c268-153">O 'página' e 'zoom' Opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.</span><span class="sxs-lookup"><span data-stu-id="6c268-153">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
