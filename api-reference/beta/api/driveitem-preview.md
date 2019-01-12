---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: be96a0cd451bb3f1c75c32f235d7669ce0bd7509
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980871"
---
# <a name="driveitem-preview"></a><span data-ttu-id="861d2-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="861d2-103">driveItem: preview</span></span>

> <span data-ttu-id="861d2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="861d2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="861d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="861d2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="861d2-106">Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="861d2-106">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="861d2-107">Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="861d2-107">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="861d2-108">**Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="861d2-108">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="861d2-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="861d2-110">Permissions</span></span>

<span data-ttu-id="861d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="861d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="861d2-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="861d2-113">Permission type</span></span>                        | <span data-ttu-id="861d2-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="861d2-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="861d2-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="861d2-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="861d2-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861d2-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="861d2-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="861d2-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="861d2-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861d2-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="861d2-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="861d2-119">Application</span></span>                            | <span data-ttu-id="861d2-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="861d2-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="861d2-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="861d2-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="861d2-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="861d2-122">Request body</span></span>

<span data-ttu-id="861d2-123">O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="861d2-123">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="861d2-124">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="861d2-124">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="861d2-125">Nome</span><span class="sxs-lookup"><span data-stu-id="861d2-125">Name</span></span>      |  <span data-ttu-id="861d2-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="861d2-126">Type</span></span>         | <span data-ttu-id="861d2-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="861d2-127">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="861d2-128">Visualizador</span><span class="sxs-lookup"><span data-stu-id="861d2-128">viewer</span></span>      | <span data-ttu-id="861d2-129">string</span><span class="sxs-lookup"><span data-stu-id="861d2-129">string</span></span>        | <span data-ttu-id="861d2-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="861d2-130">Optional.</span></span> <span data-ttu-id="861d2-131">Aplicativo de visualização para usar.</span><span class="sxs-lookup"><span data-stu-id="861d2-131">Preview app to use.</span></span> <span data-ttu-id="861d2-132">`onedrive` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="861d2-132">`onedrive` or `office`.</span></span> <span data-ttu-id="861d2-133">Se for null, um visualizador adequado será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="861d2-133">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="861d2-134">sem cromo</span><span class="sxs-lookup"><span data-stu-id="861d2-134">chromeless</span></span>  | <span data-ttu-id="861d2-135">booliano</span><span class="sxs-lookup"><span data-stu-id="861d2-135">boolean</span></span>       | <span data-ttu-id="861d2-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="861d2-136">Optional.</span></span> <span data-ttu-id="861d2-137">Se `true` (padrão), o modo de exibição incorporado não incluirá todos os controles.</span><span class="sxs-lookup"><span data-stu-id="861d2-137">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="861d2-138">allowEdit</span><span class="sxs-lookup"><span data-stu-id="861d2-138">allowEdit</span></span>   | <span data-ttu-id="861d2-139">booliano</span><span class="sxs-lookup"><span data-stu-id="861d2-139">boolean</span></span>       | <span data-ttu-id="861d2-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="861d2-140">Optional.</span></span> <span data-ttu-id="861d2-141">Se `true`, o arquivo pode ser editado da interface do usuário incorporado.</span><span class="sxs-lookup"><span data-stu-id="861d2-141">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="861d2-142">página</span><span class="sxs-lookup"><span data-stu-id="861d2-142">page</span></span>        | <span data-ttu-id="861d2-143">número de sequência de caracteres /</span><span class="sxs-lookup"><span data-stu-id="861d2-143">string/number</span></span> | <span data-ttu-id="861d2-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="861d2-144">Optional.</span></span> <span data-ttu-id="861d2-145">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="861d2-145">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="861d2-146">Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="861d2-146">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="861d2-147">zoom</span><span class="sxs-lookup"><span data-stu-id="861d2-147">zoom</span></span>        | <span data-ttu-id="861d2-148">number</span><span class="sxs-lookup"><span data-stu-id="861d2-148">number</span></span>        | <span data-ttu-id="861d2-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="861d2-149">Optional.</span></span> <span data-ttu-id="861d2-150">Amplie o nível para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="861d2-150">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="861d2-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="861d2-151">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="861d2-152">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="861d2-152">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="861d2-153">Nome</span><span class="sxs-lookup"><span data-stu-id="861d2-153">Name</span></span>           | <span data-ttu-id="861d2-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="861d2-154">Type</span></span>   | <span data-ttu-id="861d2-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="861d2-155">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="861d2-156">getUrl</span><span class="sxs-lookup"><span data-stu-id="861d2-156">getUrl</span></span>         | <span data-ttu-id="861d2-157">string</span><span class="sxs-lookup"><span data-stu-id="861d2-157">string</span></span> | <span data-ttu-id="861d2-158">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="861d2-158">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="861d2-159">postUrl</span><span class="sxs-lookup"><span data-stu-id="861d2-159">postUrl</span></span>        | <span data-ttu-id="861d2-160">string</span><span class="sxs-lookup"><span data-stu-id="861d2-160">string</span></span> | <span data-ttu-id="861d2-161">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="861d2-161">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="861d2-162">postParameters</span><span class="sxs-lookup"><span data-stu-id="861d2-162">postParameters</span></span> | <span data-ttu-id="861d2-163">string</span><span class="sxs-lookup"><span data-stu-id="861d2-163">string</span></span> | <span data-ttu-id="861d2-164">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="861d2-164">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="861d2-165">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="861d2-165">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="861d2-166">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="861d2-166">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="861d2-167">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="861d2-167">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="861d2-168">Visualizadores</span><span class="sxs-lookup"><span data-stu-id="861d2-168">Viewers</span></span>

<span data-ttu-id="861d2-169">Os seguintes valores são permitidos para o parâmetro do **Visualizador** .</span><span class="sxs-lookup"><span data-stu-id="861d2-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="861d2-170">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="861d2-170">Type value</span></span> | <span data-ttu-id="861d2-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="861d2-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="861d2-172">(nulo)</span><span class="sxs-lookup"><span data-stu-id="861d2-172">(null)</span></span>     | <span data-ttu-id="861d2-173">Escolhe um aplicativo apropriado para o arquivo de renderização.</span><span class="sxs-lookup"><span data-stu-id="861d2-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="861d2-174">Na maioria dos casos isso usará o `onedrive` visualizador, mas pode variar por tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="861d2-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="861d2-175">Use o aplicativo de pré-visualização OneDrive para processá-lo.</span><span class="sxs-lookup"><span data-stu-id="861d2-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="861d2-176">Use o WAC (Office online) para processá-lo.</span><span class="sxs-lookup"><span data-stu-id="861d2-176">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="861d2-177">Só é válido para documentos do Office.</span><span class="sxs-lookup"><span data-stu-id="861d2-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="861d2-178">Chrome versus sem cromo</span><span class="sxs-lookup"><span data-stu-id="861d2-178">Chrome vs chromeless</span></span>

<span data-ttu-id="861d2-179">Se `chromeless` for true, a visualização será um processamento bare do arquivo.</span><span class="sxs-lookup"><span data-stu-id="861d2-179">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="861d2-180">Caso contrário, pode haver adicionais barras de ferramentas/botões exibidos para interagir com a exibição de documentos.</span><span class="sxs-lookup"><span data-stu-id="861d2-180">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="861d2-181">Exibir/editar</span><span class="sxs-lookup"><span data-stu-id="861d2-181">View/edit</span></span>

<span data-ttu-id="861d2-182">Se `allowEdit` for true, o documento pode ser modificado pelo interação do usuário com a visualização incorporada.</span><span class="sxs-lookup"><span data-stu-id="861d2-182">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="861d2-183">Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="861d2-183">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="861d2-184">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="861d2-184">Page/zoom</span></span>

<span data-ttu-id="861d2-185">O `page` e `zoom` opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.</span><span class="sxs-lookup"><span data-stu-id="861d2-185">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
