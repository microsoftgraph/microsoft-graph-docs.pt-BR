---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
author: JeremyKelley
ms.openlocfilehash: f56f62fdd0244a5bc3a014cae4ad4bc9151181c7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47981881"
---
# <a name="driveitem-preview"></a><span data-ttu-id="30cba-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="30cba-103">driveItem: preview</span></span>

<span data-ttu-id="30cba-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30cba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="30cba-105">Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="30cba-105">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="30cba-106">Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.</span><span class="sxs-lookup"><span data-stu-id="30cba-106">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="30cba-107">**Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="30cba-107">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="30cba-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="30cba-109">Permissions</span></span>

<span data-ttu-id="30cba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="30cba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="30cba-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="30cba-112">Permission type</span></span>                        | <span data-ttu-id="30cba-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="30cba-113">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="30cba-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="30cba-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="30cba-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30cba-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="30cba-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="30cba-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="30cba-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="30cba-117">Not supported.</span></span>
| <span data-ttu-id="30cba-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="30cba-118">Application</span></span>                            | <span data-ttu-id="30cba-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="30cba-119">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>

## <a name="http-request"></a><span data-ttu-id="30cba-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="30cba-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="30cba-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="30cba-121">Request body</span></span>

<span data-ttu-id="30cba-122">O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="30cba-122">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="30cba-123">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="30cba-123">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="30cba-124">Nome</span><span class="sxs-lookup"><span data-stu-id="30cba-124">Name</span></span>      |  <span data-ttu-id="30cba-125">Tipo</span><span class="sxs-lookup"><span data-stu-id="30cba-125">Type</span></span>         | <span data-ttu-id="30cba-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="30cba-126">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="30cba-127">visor</span><span class="sxs-lookup"><span data-stu-id="30cba-127">viewer</span></span>      | <span data-ttu-id="30cba-128">string</span><span class="sxs-lookup"><span data-stu-id="30cba-128">string</span></span>        | <span data-ttu-id="30cba-129">Opcional.</span><span class="sxs-lookup"><span data-stu-id="30cba-129">Optional.</span></span> <span data-ttu-id="30cba-130">Aplicativo de visualização a ser usado.</span><span class="sxs-lookup"><span data-stu-id="30cba-130">Preview app to use.</span></span> <span data-ttu-id="30cba-131">`onedrive` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="30cba-131">`onedrive` or `office`.</span></span> <span data-ttu-id="30cba-132">Se for NULL, um visualizador adequado será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="30cba-132">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="30cba-133">Não Chrome</span><span class="sxs-lookup"><span data-stu-id="30cba-133">chromeless</span></span>  | <span data-ttu-id="30cba-134">booliano</span><span class="sxs-lookup"><span data-stu-id="30cba-134">boolean</span></span>       | <span data-ttu-id="30cba-135">Opcional.</span><span class="sxs-lookup"><span data-stu-id="30cba-135">Optional.</span></span> <span data-ttu-id="30cba-136">Se `true` (padrão), o modo de exibição incorporado não incluirá nenhum controle.</span><span class="sxs-lookup"><span data-stu-id="30cba-136">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="30cba-137">allowEdit</span><span class="sxs-lookup"><span data-stu-id="30cba-137">allowEdit</span></span>   | <span data-ttu-id="30cba-138">booliano</span><span class="sxs-lookup"><span data-stu-id="30cba-138">boolean</span></span>       | <span data-ttu-id="30cba-139">Opcional.</span><span class="sxs-lookup"><span data-stu-id="30cba-139">Optional.</span></span> <span data-ttu-id="30cba-140">Se `true` , o arquivo pode ser editado a partir da interface do usuário incorporada.</span><span class="sxs-lookup"><span data-stu-id="30cba-140">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="30cba-141">page</span><span class="sxs-lookup"><span data-stu-id="30cba-141">page</span></span>        | <span data-ttu-id="30cba-142">Cadeia de caracteres/número</span><span class="sxs-lookup"><span data-stu-id="30cba-142">string/number</span></span> | <span data-ttu-id="30cba-143">Opcional.</span><span class="sxs-lookup"><span data-stu-id="30cba-143">Optional.</span></span> <span data-ttu-id="30cba-144">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="30cba-144">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="30cba-145">Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="30cba-145">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="30cba-146">zoom</span><span class="sxs-lookup"><span data-stu-id="30cba-146">zoom</span></span>        | <span data-ttu-id="30cba-147">number</span><span class="sxs-lookup"><span data-stu-id="30cba-147">number</span></span>        | <span data-ttu-id="30cba-148">Opcional.</span><span class="sxs-lookup"><span data-stu-id="30cba-148">Optional.</span></span> <span data-ttu-id="30cba-149">Nível de zoom para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="30cba-149">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="30cba-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="30cba-150">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="30cba-151">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="30cba-151">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="30cba-152">Nome</span><span class="sxs-lookup"><span data-stu-id="30cba-152">Name</span></span>           | <span data-ttu-id="30cba-153">Tipo</span><span class="sxs-lookup"><span data-stu-id="30cba-153">Type</span></span>   | <span data-ttu-id="30cba-154">Descrição</span><span class="sxs-lookup"><span data-stu-id="30cba-154">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="30cba-155">getUrl</span><span class="sxs-lookup"><span data-stu-id="30cba-155">getUrl</span></span>         | <span data-ttu-id="30cba-156">string</span><span class="sxs-lookup"><span data-stu-id="30cba-156">string</span></span> | <span data-ttu-id="30cba-157">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="30cba-157">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="30cba-158">postUrl</span><span class="sxs-lookup"><span data-stu-id="30cba-158">postUrl</span></span>        | <span data-ttu-id="30cba-159">string</span><span class="sxs-lookup"><span data-stu-id="30cba-159">string</span></span> | <span data-ttu-id="30cba-160">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="30cba-160">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="30cba-161">postparameters</span><span class="sxs-lookup"><span data-stu-id="30cba-161">postParameters</span></span> | <span data-ttu-id="30cba-162">string</span><span class="sxs-lookup"><span data-stu-id="30cba-162">string</span></span> | <span data-ttu-id="30cba-163">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="30cba-163">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="30cba-164">GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="30cba-164">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="30cba-165">postparameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded` e, se estiver executando uma postagem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="30cba-165">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="30cba-166">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="30cba-166">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="30cba-167">Visualizadores</span><span class="sxs-lookup"><span data-stu-id="30cba-167">Viewers</span></span>

><span data-ttu-id="30cba-168">**Observação:** Esse parâmetro é preterido e não será disponibilizado no ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="30cba-168">**Note:** This parameter is deprecated and will not be made available on the v1.0 endpoint.</span></span>

<span data-ttu-id="30cba-169">Os valores a seguir são permitidos para o parâmetro **Viewer** .</span><span class="sxs-lookup"><span data-stu-id="30cba-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="30cba-170">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="30cba-170">Type value</span></span> | <span data-ttu-id="30cba-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="30cba-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="30cba-172">vazio</span><span class="sxs-lookup"><span data-stu-id="30cba-172">(null)</span></span>     | <span data-ttu-id="30cba-173">Escolhe um aplicativo apropriado para renderizar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="30cba-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="30cba-174">Na maioria dos casos, isso usará o `onedrive` Visualizador, mas pode variar de acordo com o tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="30cba-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="30cba-175">Use o aplicativo de visualização do OneDrive para renderizar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="30cba-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="30cba-176">Use a versão da Web do Office para renderizar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="30cba-176">Use the web version of Office to render the file.</span></span> <span data-ttu-id="30cba-177">Só é válido para documentos do Office.</span><span class="sxs-lookup"><span data-stu-id="30cba-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="30cba-178">Cromado vs não monocromático</span><span class="sxs-lookup"><span data-stu-id="30cba-178">Chrome vs chromeless</span></span>
><span data-ttu-id="30cba-179">**Observação:** Esse parâmetro é preterido e não será disponibilizado no ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="30cba-179">**Note:** This parameter is deprecated and will not be made available on the v1.0 endpoint.</span></span>

<span data-ttu-id="30cba-180">Se `chromeless` for true, a visualização será uma renderização Bare do arquivo.</span><span class="sxs-lookup"><span data-stu-id="30cba-180">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="30cba-181">Caso contrário, poderão existir barras de ferramentas/botões adicionais exibidos para interagir com o documento/modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="30cba-181">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="30cba-182">Exibir/editar</span><span class="sxs-lookup"><span data-stu-id="30cba-182">View/edit</span></span>
><span data-ttu-id="30cba-183">**Observação:** Esse parâmetro é preterido e não será disponibilizado no ponto de extremidade v 1.0.</span><span class="sxs-lookup"><span data-stu-id="30cba-183">**Note:** This parameter is deprecated and will not be made available on the v1.0 endpoint.</span></span>

<span data-ttu-id="30cba-184">Se `allowEdit` for true, o documento poderá ser modificado pela interação do usuário com a visualização incorporada.</span><span class="sxs-lookup"><span data-stu-id="30cba-184">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="30cba-185">Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="30cba-185">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="30cba-186">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="30cba-186">Page/zoom</span></span>

<span data-ttu-id="30cba-187">As `page` `zoom` Opções e podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ela.</span><span class="sxs-lookup"><span data-stu-id="30cba-187">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>


