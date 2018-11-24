# <a name="driveitem-preview"></a><span data-ttu-id="9f462-101">driveItem: visualização</span><span class="sxs-lookup"><span data-stu-id="9f462-101">driveItem: preview</span></span>

<span data-ttu-id="9f462-102">Essa ação permite que você obtenha URLs incorporáveis temporários e para um item para processar uma visualização temporária.</span><span class="sxs-lookup"><span data-stu-id="9f462-102">This action allows you to obtain short-lived embeddable URLs for an item in order to render a temporary preview.</span></span>

<span data-ttu-id="9f462-103">Se você quiser obter links incorporável vida útil longa, use o [createLink][] API.</span><span class="sxs-lookup"><span data-stu-id="9f462-103">If you want to obtain long-lived embeddable links, use the [createLink][] API instead.</span></span>

> <span data-ttu-id="9f462-104">**Observação:** Atualmente, a ação de **visualização** só está disponível no SharePoint e o OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="9f462-104">**Note:** The **preview** action is currently only available on SharePoint and OneDrive for Business.</span></span>

[createLink]: driveItem_createLink.md

## <a name="permissions"></a><span data-ttu-id="9f462-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9f462-106">Permissions</span></span>

<span data-ttu-id="9f462-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="9f462-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="9f462-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9f462-109">Permission type</span></span>                        | <span data-ttu-id="9f462-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="9f462-110">Permissions (from least to most privileged)</span></span>
|:---------------------------------------|:-------------------------------------------
| <span data-ttu-id="9f462-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9f462-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="9f462-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f462-112">Files.Read, Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All</span></span>
| <span data-ttu-id="9f462-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9f462-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9f462-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f462-114">Files.Read, Files.ReadWrite, Files.ReadWrite.All</span></span>
| <span data-ttu-id="9f462-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9f462-115">Application</span></span>                            | <span data-ttu-id="9f462-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9f462-116">Not supported.</span></span>

## <a name="http-request"></a><span data-ttu-id="9f462-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9f462-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /drives/{driveId}/items/{itemId}/preview
POST /groups/{groupId}/drive/items/{itemId}/preview
POST /me/drive/items/{itemId}/preview
POST /sites/{siteId}/drive/items/{itemId}/preview
POST /users/{userId}/drive/items/{itemId}/preview
POST /shares/{shareId}/driveItem/preview
```

## <a name="request-body"></a><span data-ttu-id="9f462-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9f462-118">Request body</span></span>

<span data-ttu-id="9f462-119">O corpo da solicitação define as propriedades da URL incorporável está solicitando o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9f462-119">The body of the request defines properties of the embeddable URL your application is requesting.</span></span>
<span data-ttu-id="9f462-120">A solicitação deve ser um objeto JSON com as seguintes propriedades.</span><span class="sxs-lookup"><span data-stu-id="9f462-120">The request should be a JSON object with the following properties.</span></span>

|   <span data-ttu-id="9f462-121">Nome</span><span class="sxs-lookup"><span data-stu-id="9f462-121">Name</span></span>      |  <span data-ttu-id="9f462-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f462-122">Type</span></span>         | <span data-ttu-id="9f462-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f462-123">Description</span></span>
|:------------|:--------------|:-----------------------------------------------
| <span data-ttu-id="9f462-124">página</span><span class="sxs-lookup"><span data-stu-id="9f462-124">page</span></span>        | <span data-ttu-id="9f462-125">número de sequência de caracteres /</span><span class="sxs-lookup"><span data-stu-id="9f462-125">string/number</span></span> | <span data-ttu-id="9f462-126">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f462-126">Optional.</span></span> <span data-ttu-id="9f462-127">Número de página do documento para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="9f462-127">Page number of document to start at, if applicable.</span></span> <span data-ttu-id="9f462-128">Especificado como cadeia de caracteres para uso futuro casos em torno de tipos de arquivo como ZIP.</span><span class="sxs-lookup"><span data-stu-id="9f462-128">Specified as string for future use cases around file types such as ZIP.</span></span>
| <span data-ttu-id="9f462-129">zoom</span><span class="sxs-lookup"><span data-stu-id="9f462-129">zoom</span></span>        | <span data-ttu-id="9f462-130">número</span><span class="sxs-lookup"><span data-stu-id="9f462-130">number</span></span>        | <span data-ttu-id="9f462-131">Opcional.</span><span class="sxs-lookup"><span data-stu-id="9f462-131">Optional.</span></span> <span data-ttu-id="9f462-132">Amplie o nível para iniciar em, se aplicável.</span><span class="sxs-lookup"><span data-stu-id="9f462-132">Zoom level to start at, if applicable.</span></span>

## <a name="response"></a><span data-ttu-id="9f462-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9f462-133">Response</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

<span data-ttu-id="9f462-134">A resposta será um objeto JSON que contém as seguintes propriedades:</span><span class="sxs-lookup"><span data-stu-id="9f462-134">The response will be a JSON object containing the following properties:</span></span>

| <span data-ttu-id="9f462-135">Nome</span><span class="sxs-lookup"><span data-stu-id="9f462-135">Name</span></span>           | <span data-ttu-id="9f462-136">Tipo</span><span class="sxs-lookup"><span data-stu-id="9f462-136">Type</span></span>   | <span data-ttu-id="9f462-137">Descrição</span><span class="sxs-lookup"><span data-stu-id="9f462-137">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="9f462-138">getUrl</span><span class="sxs-lookup"><span data-stu-id="9f462-138">getUrl</span></span>         | <span data-ttu-id="9f462-139">string</span><span class="sxs-lookup"><span data-stu-id="9f462-139">string</span></span> | <span data-ttu-id="9f462-140">URL adequada para incorporação usando HTTP GET (iframes, etc.)</span><span class="sxs-lookup"><span data-stu-id="9f462-140">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="9f462-141">postUrl</span><span class="sxs-lookup"><span data-stu-id="9f462-141">postUrl</span></span>        | <span data-ttu-id="9f462-142">string</span><span class="sxs-lookup"><span data-stu-id="9f462-142">string</span></span> | <span data-ttu-id="9f462-143">URL adequada para incorporação usando POST HTTP (formulário post, JS, etc.)</span><span class="sxs-lookup"><span data-stu-id="9f462-143">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="9f462-144">postParameters</span><span class="sxs-lookup"><span data-stu-id="9f462-144">postParameters</span></span> | <span data-ttu-id="9f462-145">string</span><span class="sxs-lookup"><span data-stu-id="9f462-145">string</span></span> | <span data-ttu-id="9f462-146">Parâmetros de POSTAGEM para incluir se usando postUrl</span><span class="sxs-lookup"><span data-stu-id="9f462-146">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="9f462-147">GetUrl, postUrl ou ambos podem ser retornados dependendo do estado atual do suporte de embed para as opções especificadas.</span><span class="sxs-lookup"><span data-stu-id="9f462-147">Either getUrl, postUrl, or both might be returned depending on the current state of embed support for the specified options.</span></span>

<span data-ttu-id="9f462-148">postParameters é uma cadeia de caracteres formatada como `application/x-www-form-urlencoded`, e se realizar uma POSTAGEM para o postUrl o tipo de conteúdo deve ser definida adequadamente.</span><span class="sxs-lookup"><span data-stu-id="9f462-148">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="9f462-149">Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9f462-149">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

### <a name="pagezoom"></a><span data-ttu-id="9f462-150">Página/zoom</span><span class="sxs-lookup"><span data-stu-id="9f462-150">Page/zoom</span></span>

<span data-ttu-id="9f462-151">O 'página' e 'zoom' Opções podem não estar disponíveis para todos os aplicativos de visualização, mas serão aplicadas se o aplicativo de visualização lhe fornecer apoio.</span><span class="sxs-lookup"><span data-stu-id="9f462-151">The 'page' and 'zoom' options may not be available for all preview apps, but will be applied if the preview app supports it.</span></span>
