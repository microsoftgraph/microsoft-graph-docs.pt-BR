---
title: 'driveItem: visualização'
description: Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.
ms.openlocfilehash: 51432e53d6986e680dda8508ef0069c7713b3a9d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034596"
---
# <a name="driveitem-preview"></a><span data-ttu-id="63922-103">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="63922-103">driveItem: preview</span></span>

> <span data-ttu-id="63922-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="63922-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63922-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="63922-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="63922-106">Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="63922-106">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="63922-107">Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="63922-107">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="63922-108">**Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="63922-108">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveitem-createlink.md

## <a name="permissions"></a><span data-ttu-id="63922-110">Permissions</span><span class="sxs-lookup"><span data-stu-id="63922-110">Permissions</span></span>

<span data-ttu-id="63922-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="63922-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="63922-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="63922-113">Permission type</span></span>                        | <span data-ttu-id="63922-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="63922-114">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="63922-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="63922-115">Delegated (work or school account)</span></span>     | <span data-ttu-id="63922-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63922-116">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="63922-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="63922-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63922-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63922-118">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="63922-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="63922-119">Application</span></span>                            | <span data-ttu-id="63922-120">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="63922-120">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="63922-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="63922-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="63922-122">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="63922-122">Request body</span></span>

<span data-ttu-id="63922-123">O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="63922-123">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="63922-124">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="63922-124">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="63922-125">Nome</span><span class="sxs-lookup"><span data-stu-id="63922-125">Name</span></span>      |  <span data-ttu-id="63922-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="63922-126">Type</span></span>         | <span data-ttu-id="63922-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="63922-127">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="63922-128">Visualizador</span><span class="sxs-lookup"><span data-stu-id="63922-128">viewer</span></span>      | <span data-ttu-id="63922-129">string</span><span class="sxs-lookup"><span data-stu-id="63922-129">string</span></span>        | <span data-ttu-id="63922-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63922-130">Optional.</span></span> <span data-ttu-id="63922-131">Aplicativo de visualização para usar.</span><span class="sxs-lookup"><span data-stu-id="63922-131">Preview app to use.</span></span> <span data-ttu-id="63922-132">`onedrive` ou `office`.</span><span class="sxs-lookup"><span data-stu-id="63922-132">`onedrive` or `office`.</span></span> <span data-ttu-id="63922-133">Se for null, um visualizador adequado será escolhido automaticamente.</span><span class="sxs-lookup"><span data-stu-id="63922-133">If null, a suitable viewer will be chosen automatically.</span></span>
| <span data-ttu-id="63922-134">sem cromo</span><span class="sxs-lookup"><span data-stu-id="63922-134">chromeless</span></span>  | <span data-ttu-id="63922-135">booliano</span><span class="sxs-lookup"><span data-stu-id="63922-135">boolean</span></span>       | <span data-ttu-id="63922-136">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63922-136">Optional.</span></span> <span data-ttu-id="63922-137">Se `true` (padrão), o modo de exibição incorporado não incluirá todos os controles.</span><span class="sxs-lookup"><span data-stu-id="63922-137">If `true` (default), the embedded view will not include any controls.</span></span>
| <span data-ttu-id="63922-138">allowEdit</span><span class="sxs-lookup"><span data-stu-id="63922-138">allowEdit</span></span>   | <span data-ttu-id="63922-139">booliano</span><span class="sxs-lookup"><span data-stu-id="63922-139">boolean</span></span>       | <span data-ttu-id="63922-140">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63922-140">Optional.</span></span> <span data-ttu-id="63922-141">Se `true`, o arquivo pode ser editado da interface do usuário incorporado.</span><span class="sxs-lookup"><span data-stu-id="63922-141">If `true`, the file can be edited from the embedded UI.</span></span>
| <span data-ttu-id="63922-142">página</span><span class="sxs-lookup"><span data-stu-id="63922-142">page</span></span>        | <span data-ttu-id="63922-143">número de sequência de caracteres /</span><span class="sxs-lookup"><span data-stu-id="63922-143">string/number</span></span> | <span data-ttu-id="63922-144">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63922-144">Optional.</span></span> <span data-ttu-id="63922-145">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="63922-145">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="63922-146">Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="63922-146">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="63922-147">zoom</span><span class="sxs-lookup"><span data-stu-id="63922-147">zoom</span></span>        | <span data-ttu-id="63922-148">número</span><span class="sxs-lookup"><span data-stu-id="63922-148">number</span></span>        | <span data-ttu-id="63922-149">Opcional.</span><span class="sxs-lookup"><span data-stu-id="63922-149">Optional.</span></span> <span data-ttu-id="63922-150">Amplie o nível para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="63922-150">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="63922-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="63922-151">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="63922-152">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="63922-152">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="63922-153">Nome</span><span class="sxs-lookup"><span data-stu-id="63922-153">Name</span></span>           | <span data-ttu-id="63922-154">Tipo</span><span class="sxs-lookup"><span data-stu-id="63922-154">Type</span></span>   | <span data-ttu-id="63922-155">Descrição</span><span class="sxs-lookup"><span data-stu-id="63922-155">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="63922-156">getUrl</span><span class="sxs-lookup"><span data-stu-id="63922-156">getUrl</span></span>         | <span data-ttu-id="63922-157">string</span><span class="sxs-lookup"><span data-stu-id="63922-157">string</span></span> | <span data-ttu-id="63922-158">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="63922-158">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="63922-159">postUrl</span><span class="sxs-lookup"><span data-stu-id="63922-159">postUrl</span></span>        | <span data-ttu-id="63922-160">string</span><span class="sxs-lookup"><span data-stu-id="63922-160">string</span></span> | <span data-ttu-id="63922-161">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="63922-161">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="63922-162">postParameters</span><span class="sxs-lookup"><span data-stu-id="63922-162">postParameters</span></span> | <span data-ttu-id="63922-163">string</span><span class="sxs-lookup"><span data-stu-id="63922-163">string</span></span> | <span data-ttu-id="63922-164">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="63922-164">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="63922-165">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="63922-165">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="63922-166">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="63922-166">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="63922-167">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="63922-167">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="viewers"></a><span data-ttu-id="63922-168">Visualizadores</span><span class="sxs-lookup"><span data-stu-id="63922-168">Viewers</span></span>

<span data-ttu-id="63922-169">Os seguintes valores são permitidos para o parâmetro do **Visualizador** .</span><span class="sxs-lookup"><span data-stu-id="63922-169">The following values are allowed for the **viewer** parameter.</span></span>

| <span data-ttu-id="63922-170">Valor do tipo</span><span class="sxs-lookup"><span data-stu-id="63922-170">Type value</span></span> | <span data-ttu-id="63922-171">Descrição</span><span class="sxs-lookup"><span data-stu-id="63922-171">Description</span></span>
|:-----------|:----------------------------------------------------------------
| <span data-ttu-id="63922-172">(nulo)</span><span class="sxs-lookup"><span data-stu-id="63922-172">(null)</span></span>     | <span data-ttu-id="63922-173">Escolhe um aplicativo apropriado para o arquivo de renderização.</span><span class="sxs-lookup"><span data-stu-id="63922-173">Chooses an appropriate app for rendering the file.</span></span> <span data-ttu-id="63922-174">Na maioria dos casos isso usará o `onedrive` visualizador, mas pode variar por tipo de arquivo.</span><span class="sxs-lookup"><span data-stu-id="63922-174">In most cases this will use the `onedrive` previewer, but may vary by file type.</span></span>
| `onedrive` | <span data-ttu-id="63922-175">Use o aplicativo de pré-visualização OneDrive para processá-lo.</span><span class="sxs-lookup"><span data-stu-id="63922-175">Use the OneDrive previewer app to render the file.</span></span>
| `office`   | <span data-ttu-id="63922-176">Use o WAC (Office online) para processá-lo.</span><span class="sxs-lookup"><span data-stu-id="63922-176">Use the WAC (Office online) to render the file.</span></span> <span data-ttu-id="63922-177">Só é válido para documentos do Office.</span><span class="sxs-lookup"><span data-stu-id="63922-177">Only valid for Office documents.</span></span>

### <a name="chrome-vs-chromeless"></a><span data-ttu-id="63922-178">Chrome versus sem cromo</span><span class="sxs-lookup"><span data-stu-id="63922-178">Chrome vs chromeless</span></span>

<span data-ttu-id="63922-179">Se `chromeless` for true, a visualização será um processamento bare do arquivo.</span><span class="sxs-lookup"><span data-stu-id="63922-179">If `chromeless` is true, the preview will be a bare rendering of the file.</span></span>
<span data-ttu-id="63922-180">Caso contrário, pode haver adicionais barras de ferramentas/botões exibidos para interagir com a exibição de documentos.</span><span class="sxs-lookup"><span data-stu-id="63922-180">Otherwise, there may be additional toolbars/buttons displayed for interacting with the document/view.</span></span>

### <a name="viewedit"></a><span data-ttu-id="63922-181">Exibir/editar</span><span class="sxs-lookup"><span data-stu-id="63922-181">View/edit</span></span>

<span data-ttu-id="63922-182">Se `allowEdit` for true, o documento pode ser modificado pelo interação do usuário com a visualização incorporada.</span><span class="sxs-lookup"><span data-stu-id="63922-182">If `allowEdit` is true, the document can be modified by user interaction with the embedded preview.</span></span>
<span data-ttu-id="63922-183">Esse recurso pode não estar disponível para todos os aplicativos de visualização ou tipos de arquivo.</span><span class="sxs-lookup"><span data-stu-id="63922-183">This capability may not be available for all preview apps or file types.</span></span>

### <a name="pagezoom"></a><span data-ttu-id="63922-184">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="63922-184">Page/zoom</span></span>

<span data-ttu-id="63922-185">O `page` e `zoom` opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.</span><span class="sxs-lookup"><span data-stu-id="63922-185">The `page` and `zoom` options might not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
