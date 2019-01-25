---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a49a05e1e01616bc9bbbb713fd05805d9af3070
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29508535"
---
# <a name="driveitem-preview"></a><span data-ttu-id="96bf8-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="96bf8-103">driveItem: preview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96bf8-104">Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="96bf8-104">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="96bf8-105">Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="96bf8-105">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="96bf8-106">**Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="96bf8-106">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="96bf8-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="96bf8-108">Permissions</span></span>

<span data-ttu-id="96bf8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="96bf8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="96bf8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="96bf8-111">Permission type</span></span>                        | <span data-ttu-id="96bf8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="96bf8-112">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="96bf8-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="96bf8-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="96bf8-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96bf8-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="96bf8-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="96bf8-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="96bf8-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96bf8-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="96bf8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="96bf8-117">Application</span></span>                            | <span data-ttu-id="96bf8-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="96bf8-118">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="96bf8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="96bf8-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="96bf8-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="96bf8-120">Request body</span></span>

<span data-ttu-id="96bf8-121">O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96bf8-121">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="96bf8-122">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="96bf8-122">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="96bf8-123">Nome</span><span class="sxs-lookup"><span data-stu-id="96bf8-123">Name</span></span>      |  <span data-ttu-id="96bf8-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bf8-124">Type</span></span>         | <span data-ttu-id="96bf8-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bf8-125">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="96bf8-126">Visualizador</span><span class="sxs-lookup"><span data-stu-id="96bf8-126">viewer</span></span>      | <span data-ttu-id="96bf8-127">string</span><span class="sxs-lookup"><span data-stu-id="96bf8-127">string</span></span>        | <span data-ttu-id="96bf8-128">Opcional.</span><span class="sxs-lookup"><span data-stu-id="96bf8-128">Optional.</span></span> <span data-ttu-id="96bf8-129">Aplicativo de visualização para usar.</span><span class="sxs-lookup"><span data-stu-id="96bf8-129">Preview app to use.</span></span> <span data-ttu-id="96bf8-130">`onedrive` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="96bf8-130">`onedrive` or `office`.</span></span> <span data-ttu-id="96bf8-131">Se for null, um visualizador adequado será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="96bf8-131">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="96bf8-132">sem cromo</span><span class="sxs-lookup"><span data-stu-id="96bf8-132">chromeless</span></span>  | <span data-ttu-id="96bf8-133">booliano</span><span class="sxs-lookup"><span data-stu-id="96bf8-133">boolean</span></span>       | <span data-ttu-id="96bf8-134">Opcional.</span><span class="sxs-lookup"><span data-stu-id="96bf8-134">Optional.</span></span> <span data-ttu-id="96bf8-135">Se `true` (padrão), o modo de exibição incorporado não incluirá todos os controles.</span><span class="sxs-lookup"><span data-stu-id="96bf8-135">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="96bf8-136">AllowEdit</span><span class="sxs-lookup"><span data-stu-id="96bf8-136">allowEdit</span></span>   | <span data-ttu-id="96bf8-137">booliano</span><span class="sxs-lookup"><span data-stu-id="96bf8-137">boolean</span></span>       | <span data-ttu-id="96bf8-138">Opcional.</span><span class="sxs-lookup"><span data-stu-id="96bf8-138">Optional.</span></span> <span data-ttu-id="96bf8-139">Se `true`, o arquivo pode ser editado da interface do usuário incorporado.</span><span class="sxs-lookup"><span data-stu-id="96bf8-139">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="96bf8-140">página</span><span class="sxs-lookup"><span data-stu-id="96bf8-140">page</span></span>        | <span data-ttu-id="96bf8-141">número de sequência de caracteres /</span><span class="sxs-lookup"><span data-stu-id="96bf8-141">string/number</span></span> | <span data-ttu-id="96bf8-142">Opcional.</span><span class="sxs-lookup"><span data-stu-id="96bf8-142">Optional.</span></span> <span data-ttu-id="96bf8-143">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="96bf8-143">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="96bf8-144">Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="96bf8-144">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="96bf8-145">zoom</span><span class="sxs-lookup"><span data-stu-id="96bf8-145">zoom</span></span>        | <span data-ttu-id="96bf8-146">number</span><span class="sxs-lookup"><span data-stu-id="96bf8-146">number</span></span>        | <span data-ttu-id="96bf8-147">Opcional.</span><span class="sxs-lookup"><span data-stu-id="96bf8-147">Optional.</span></span> <span data-ttu-id="96bf8-148">Amplie o nível para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="96bf8-148">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="96bf8-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="96bf8-149">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="96bf8-150">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="96bf8-150">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="96bf8-151">Nome</span><span class="sxs-lookup"><span data-stu-id="96bf8-151">Name</span></span>           | <span data-ttu-id="96bf8-152">Tipo</span><span class="sxs-lookup"><span data-stu-id="96bf8-152">Type</span></span>   | <span data-ttu-id="96bf8-153">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bf8-153">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="96bf8-154">getUrl</span><span class="sxs-lookup"><span data-stu-id="96bf8-154">getUrl</span></span>         | <span data-ttu-id="96bf8-155">string</span><span class="sxs-lookup"><span data-stu-id="96bf8-155">string</span></span> | <span data-ttu-id="96bf8-156">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="96bf8-156">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="96bf8-157">postUrl</span><span class="sxs-lookup"><span data-stu-id="96bf8-157">postUrl</span></span>        | <span data-ttu-id="96bf8-158">string</span><span class="sxs-lookup"><span data-stu-id="96bf8-158">string</span></span> | <span data-ttu-id="96bf8-159">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="96bf8-159">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="96bf8-160">postParameters</span><span class="sxs-lookup"><span data-stu-id="96bf8-160">postParameters</span></span> | <span data-ttu-id="96bf8-161">string</span><span class="sxs-lookup"><span data-stu-id="96bf8-161">string</span></span> | <span data-ttu-id="96bf8-162">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="96bf8-162">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="96bf8-163">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="96bf8-163">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="96bf8-164">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="96bf8-164">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="96bf8-165">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="96bf8-165">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="96bf8-166">Visualizadores</span><span class="sxs-lookup"><span data-stu-id="96bf8-166">Viewers</span></span>

<span data-ttu-id="96bf8-167">Os seguintes valores são permitidos para o parâmetro do **Visualizador** .</span><span class="sxs-lookup"><span data-stu-id="96bf8-167">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="96bf8-168">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="96bf8-168">Type value</span></span> | <span data-ttu-id="96bf8-169">Descrição</span><span class="sxs-lookup"><span data-stu-id="96bf8-169">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="96bf8-170">Null
</span><span class="sxs-lookup"><span data-stu-id="96bf8-170">(null)</span></span>     | <span data-ttu-id="96bf8-171">Escolhe um aplicativo apropriado para o arquivo de renderização.</span><span class="sxs-lookup"><span data-stu-id="96bf8-171">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="96bf8-172">Na maioria dos casos isso usará o `onedrive` visualizador, mas pode variar por tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="96bf8-172">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="96bf8-173">Use o aplicativo de pré-visualização OneDrive para processá-lo.</span><span class="sxs-lookup"><span data-stu-id="96bf8-173">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="96bf8-174">Use o WAC (Office online) para processá-lo.</span><span class="sxs-lookup"><span data-stu-id="96bf8-174">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="96bf8-175">Só é válido para documentos do Office.</span><span class="sxs-lookup"><span data-stu-id="96bf8-175">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="96bf8-176">Chrome versus sem cromo</span><span class="sxs-lookup"><span data-stu-id="96bf8-176">Chrome vs chromeless</span></span>

<span data-ttu-id="96bf8-177">Se `chromeless` for true, a visualização será um processamento bare do arquivo.</span><span class="sxs-lookup"><span data-stu-id="96bf8-177">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="96bf8-178">Caso contrário, pode haver adicionais barras de ferramentas/botões exibidos para interagir com a exibição de documentos.</span><span class="sxs-lookup"><span data-stu-id="96bf8-178">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="96bf8-179">Exibir/editar</span><span class="sxs-lookup"><span data-stu-id="96bf8-179">View/edit</span></span>

<span data-ttu-id="96bf8-180">Se `allowEdit` for true, o documento pode ser modificado pelo interação do usuário com a visualização incorporada.</span><span class="sxs-lookup"><span data-stu-id="96bf8-180">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="96bf8-181">Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="96bf8-181">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="96bf8-182">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="96bf8-182">Page/zoom</span></span>

<span data-ttu-id="96bf8-183">O `page` e `zoom` opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.</span><span class="sxs-lookup"><span data-stu-id="96bf8-183">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/driveitem-preview.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
