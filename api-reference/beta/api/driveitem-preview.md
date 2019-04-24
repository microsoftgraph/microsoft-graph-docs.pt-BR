---
title: 'driveItem: visualização'
description: Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32454367"
---
# <a name="driveitem-preview"></a><span data-ttu-id="c3efb-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="c3efb-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3efb-104">Esta ação permite que você obtenha URLs que podem ser inseridas de curta duração em um item para renderizar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="c3efb-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="c3efb-105">Se você quiser obter links incorporáveis de longa duração, use a API [CreateLink][] em vez disso.</span><span class="sxs-lookup"><span data-stu-id="c3efb-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="c3efb-106">**Observação:** No momento, a ação de **Visualização** só está disponível no SharePoint e no onedrive for Business.</span><span class="sxs-lookup"><span data-stu-id="c3efb-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="c3efb-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="c3efb-108">Permissions</span></span>

<span data-ttu-id="c3efb-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3efb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c3efb-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c3efb-111">Permission type</span></span>                        | <span data-ttu-id="c3efb-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c3efb-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="c3efb-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c3efb-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c3efb-114">Files. Read, files. ReadWrite, files. ReadWrite. All, sites. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3efb-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="c3efb-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c3efb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3efb-116">Files. Read, files. ReadWrite, files. ReadWrite. All</span><span class="sxs-lookup"><span data-stu-id="c3efb-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="c3efb-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c3efb-117">Application</span></span>                            | <span data-ttu-id="c3efb-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c3efb-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="c3efb-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c3efb-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="c3efb-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c3efb-120">Request body</span></span>

<span data-ttu-id="c3efb-121">O corpo da solicitação define as propriedades da URL incorporável que seu aplicativo está solicitando.</span><span class="sxs-lookup"><span data-stu-id="c3efb-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="c3efb-122">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="c3efb-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="c3efb-123">Name</span><span class="sxs-lookup"><span data-stu-id="c3efb-123">Name</span></span>      |  <span data-ttu-id="c3efb-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3efb-124">Type</span></span>         | <span data-ttu-id="c3efb-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3efb-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="c3efb-126">visor</span><span class="sxs-lookup"><span data-stu-id="c3efb-126">viewer</span></span>      | <span data-ttu-id="c3efb-127">string</span><span class="sxs-lookup"><span data-stu-id="c3efb-127">string</span></span>        | <span data-ttu-id="c3efb-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3efb-128">Optional.</span></span> <span data-ttu-id="c3efb-129">Aplicativo de visualização a ser usado.</span><span class="sxs-lookup"><span data-stu-id="c3efb-129">Preview app to use.</span></span> <span data-ttu-id="c3efb-130">`onedrive` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="c3efb-130">`onedrive` or `office`.</span></span> <span data-ttu-id="c3efb-131">Se for NULL, um visualizador adequado será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="c3efb-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="c3efb-132">Não Chrome</span><span class="sxs-lookup"><span data-stu-id="c3efb-132">chromeless</span></span>  | <span data-ttu-id="c3efb-133">booliano</span><span class="sxs-lookup"><span data-stu-id="c3efb-133">boolean</span></span>       | <span data-ttu-id="c3efb-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3efb-134">Optional.</span></span> <span data-ttu-id="c3efb-135">Se `true` (padrão), o modo de exibição incorporado não incluirá nenhum controle.</span><span class="sxs-lookup"><span data-stu-id="c3efb-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="c3efb-136">allowEdit</span><span class="sxs-lookup"><span data-stu-id="c3efb-136">allowEdit</span></span>   | <span data-ttu-id="c3efb-137">booliano</span><span class="sxs-lookup"><span data-stu-id="c3efb-137">boolean</span></span>       | <span data-ttu-id="c3efb-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3efb-138">Optional.</span></span> <span data-ttu-id="c3efb-139">Se `true`, o arquivo pode ser editado a partir da interface do usuário incorporada.</span><span class="sxs-lookup"><span data-stu-id="c3efb-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="c3efb-140">page</span><span class="sxs-lookup"><span data-stu-id="c3efb-140">page</span></span>        | <span data-ttu-id="c3efb-141">Cadeia de caracteres/número</span><span class="sxs-lookup"><span data-stu-id="c3efb-141">string/number</span></span> | <span data-ttu-id="c3efb-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3efb-142">Optional.</span></span> <span data-ttu-id="c3efb-143">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="c3efb-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="c3efb-144">Especificado como cadeia de caracteres para casos de uso futuros em relação a tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="c3efb-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="c3efb-145">zoom</span><span class="sxs-lookup"><span data-stu-id="c3efb-145">zoom</span></span>        | <span data-ttu-id="c3efb-146">number</span><span class="sxs-lookup"><span data-stu-id="c3efb-146">number</span></span>        | <span data-ttu-id="c3efb-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c3efb-147">Optional.</span></span> <span data-ttu-id="c3efb-148">Nível de zoom para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="c3efb-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="c3efb-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c3efb-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="c3efb-150">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="c3efb-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="c3efb-151">Name</span><span class="sxs-lookup"><span data-stu-id="c3efb-151">Name</span></span>           | <span data-ttu-id="c3efb-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3efb-152">Type</span></span>   | <span data-ttu-id="c3efb-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3efb-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="c3efb-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="c3efb-154">getUrl</span></span>         | <span data-ttu-id="c3efb-155">string</span><span class="sxs-lookup"><span data-stu-id="c3efb-155">string</span></span> | <span data-ttu-id="c3efb-156">URL adequada para incorporação usando HTTP GET (IFrames, etc.)</span><span class="sxs-lookup"><span data-stu-id="c3efb-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="c3efb-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="c3efb-157">postUrl</span></span>        | <span data-ttu-id="c3efb-158">string</span><span class="sxs-lookup"><span data-stu-id="c3efb-158">string</span></span> | <span data-ttu-id="c3efb-159">URL adequada para incorporação usando HTTP POST (Form Post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="c3efb-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="c3efb-160">postparameters</span><span class="sxs-lookup"><span data-stu-id="c3efb-160">postParameters</span></span> | <span data-ttu-id="c3efb-161">string</span><span class="sxs-lookup"><span data-stu-id="c3efb-161">string</span></span> | <span data-ttu-id="c3efb-162">LANÇAR parâmetros para incluir se estiver usando postUrl</span><span class="sxs-lookup"><span data-stu-id="c3efb-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="c3efb-163">GetUrl, postUrl ou ambos podem ser retornados, dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="c3efb-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="c3efb-164">postparameters é uma cadeia de caracteres `application/x-www-form-urlencoded`formatada como e, se estiver executando uma postaGem no postUrl, o tipo de conteúdo deve ser definido de acordo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="c3efb-165">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="c3efb-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="c3efb-166">Visualizadores</span><span class="sxs-lookup"><span data-stu-id="c3efb-166">Viewers</span></span>

<span data-ttu-id="c3efb-167">Os valores a seguir são permitidos para o parâmetro **Viewer** .</span><span class="sxs-lookup"><span data-stu-id="c3efb-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="c3efb-168">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="c3efb-168">Type value</span></span> | <span data-ttu-id="c3efb-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3efb-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="c3efb-170">vazio</span><span class="sxs-lookup"><span data-stu-id="c3efb-170">(null)</span></span>     | <span data-ttu-id="c3efb-171">Escolhe um aplicativo apropriado para renderizar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="c3efb-172">Na maioria dos casos, isso usará o visualizador, mas pode variar de acordo com o tipo de `onedrive` arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="c3efb-173">Use o aplicativo de visualização do OneDrive para renderizar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="c3efb-174">Use o WAC (Office Online) para renderizar o arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="c3efb-175">Só é válido para documentos do Office.</span><span class="sxs-lookup"><span data-stu-id="c3efb-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="c3efb-176">Cromado vs não monocromático</span><span class="sxs-lookup"><span data-stu-id="c3efb-176">Chrome vs chromeless</span></span>

<span data-ttu-id="c3efb-177">Se `chromeless` for true, a visualização será uma renderização Bare do arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="c3efb-178">Caso contrário, poderão existir barras de ferramentas/botões adicionais exibidos para interagir com o documento/modo de exibição.</span><span class="sxs-lookup"><span data-stu-id="c3efb-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="c3efb-179">Exibir/editar</span><span class="sxs-lookup"><span data-stu-id="c3efb-179">View/edit</span></span>

<span data-ttu-id="c3efb-180">Se `allowEdit` for true, o documento poderá ser modificado pela interação do usuário com a visualização incorporada.</span><span class="sxs-lookup"><span data-stu-id="c3efb-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="c3efb-181">Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="c3efb-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="c3efb-182">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="c3efb-182">Page/zoom</span></span>

<span data-ttu-id="c3efb-183">As `page` opções `zoom` e podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização oferecer suporte a ela.</span><span class="sxs-lookup"><span data-stu-id="c3efb-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
