---
title: Trabalhando com o Excel no Microsoft Graph
description: 'É possível usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive for Business, site do SharePoint ou unidade do Grupo. O recurso `Workbook` (ou arquivo do Excel) contém todos os outros recursos do Excel por meio de relações. É possível acessar uma pasta de trabalho por meio da API Drive identificando a localização do arquivo na URL. Por exemplo:'
localization_priority: Priority
author: lumine2008
ms.prod: excel
ms.openlocfilehash: 0010a7244d9ba6e629849f55dfc793bf6b875b38
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27917682"
---
# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="991e5-106">Trabalhando com o Excel no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="991e5-106">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="991e5-p102">É possível usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive for Business, site do SharePoint ou unidade do Grupo. O recurso `Workbook` (ou arquivo do Excel) contém todos os outros recursos do Excel por meio de relações. É possível acessar uma pasta de trabalho por meio da [API Drive](drive.md) identificando a localização do arquivo na URL. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="991e5-p102">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive for Business, SharePoint site or Group drive. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="991e5-p103">Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho. Por exemplo, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span><span class="sxs-lookup"><span data-stu-id="991e5-p103">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="991e5-113">retorna uma coleção de todos os objetos da planilha que fazem parte da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="991e5-113">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="991e5-p104">A API REST do Excel só oferece suporte para pastas de trabalho formatadas pelo arquivo do Office Open XML. Não há suporte para pastas de trabalho de extensão de `.xls`.</span><span class="sxs-lookup"><span data-stu-id="991e5-p104">The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

<span data-ttu-id="991e5-116">**Observação**: o suporte para pastas de trabalho armazenadas na plataforma de Consumidor do OneDrive ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="991e5-116">**Note**: Support for workbooks stored in OneDrive Consumer platform is still not available.</span></span> <span data-ttu-id="991e5-117">Neste momento, somente os arquivos armazenados em plataformas comerciais têm suporte das APIs REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="991e5-117">At this time, only the files stored in business platform is supported by Excel REST APIs.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="991e5-118">Autorização e escopos</span><span class="sxs-lookup"><span data-stu-id="991e5-118">Authorization and scopes</span></span>

<span data-ttu-id="991e5-119">Você pode usar o [ponto de extremidade do Azure AD v.2](https://developer.microsoft.com/graph/docs/authorization/converged_auth) para autenticar APIs do Excel.</span><span class="sxs-lookup"><span data-stu-id="991e5-119">You can use the [Azure AD v.2 endpoint](https://developer.microsoft.com/graph/docs/authorization/converged_auth) to authenticate Excel APIs.</span></span> <span data-ttu-id="991e5-120">Todas as APIs exigem o cabeçalho HTTP `Authorization: Bearer {access-token}`.</span><span class="sxs-lookup"><span data-stu-id="991e5-120">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="991e5-121">Um dos seguintes [escopos de permissão](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é obrigatório para usar o recurso do Excel:</span><span class="sxs-lookup"><span data-stu-id="991e5-121">One of the following [permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="991e5-122">Files.Read (para ações de leitura)</span><span class="sxs-lookup"><span data-stu-id="991e5-122">Files.Read (for read actions)</span></span>
* <span data-ttu-id="991e5-123">Files.ReadWrite (para ações de leitura e gravação)</span><span class="sxs-lookup"><span data-stu-id="991e5-123">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="991e5-124">Sessões e persistência</span><span class="sxs-lookup"><span data-stu-id="991e5-124">Sessions and persistence</span></span>

<span data-ttu-id="991e5-125">As APIs do Excel podem ser chamadas em um destes três modos:</span><span class="sxs-lookup"><span data-stu-id="991e5-125">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="991e5-126">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas).</span><span class="sxs-lookup"><span data-stu-id="991e5-126">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="991e5-127">Esse é o modo de operação mais eficiente e com desempenho mais elevado.</span><span class="sxs-lookup"><span data-stu-id="991e5-127">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="991e5-p108">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="991e5-p108">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="991e5-132">Sem sessão ‒ a chamada à API é feita sem informações sobre a sessão.</span><span class="sxs-lookup"><span data-stu-id="991e5-132">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="991e5-133">Os servidores do Excel têm que localizar a cópia do servidor de pasta de trabalho sempre que executam a operação. Portanto, essa não é uma maneira eficiente de chamar APIs do Excel.</span><span class="sxs-lookup"><span data-stu-id="991e5-133">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="991e5-134">Ele é adequado para fazer solicitações únicas.</span><span class="sxs-lookup"><span data-stu-id="991e5-134">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="991e5-135">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="991e5-135">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="991e5-p110">**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="991e5-p110">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="991e5-139">Chamada à API para obter uma sessão</span><span class="sxs-lookup"><span data-stu-id="991e5-139">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="991e5-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-140">Request</span></span> 

<span data-ttu-id="991e5-141">Passe um objeto JSON definindo o valor de `persistchanges` como `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="991e5-141">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="991e5-142">Quando o valor de `persistChanges` está definido como `false`, uma id de sessão não persistente é retornada.</span><span class="sxs-lookup"><span data-stu-id="991e5-142">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="991e5-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-143">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a><span data-ttu-id="991e5-144">Uso</span><span class="sxs-lookup"><span data-stu-id="991e5-144">Usage</span></span> 

<span data-ttu-id="991e5-145">A ID de sessão retornada da chamada anterior é transmitida como um cabeçalho em solicitações de API subsequentes no</span><span class="sxs-lookup"><span data-stu-id="991e5-145">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="991e5-146">cabeçalho HTTP `workbook-session-id`.</span><span class="sxs-lookup"><span data-stu-id="991e5-146">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="991e5-147">Observação: se a id da sessão tiver expirado, um código de erro HTTP `404` será retornado na sessão.</span><span class="sxs-lookup"><span data-stu-id="991e5-147">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="991e5-148">Nesse cenário, você pode optar por criar uma nova sessão e continuar.</span><span class="sxs-lookup"><span data-stu-id="991e5-148">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="991e5-149">Outra abordagem seria atualizar a sessão periodicamente para manter a sessão ativa.</span><span class="sxs-lookup"><span data-stu-id="991e5-149">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="991e5-150">Normalmente, a sessão persistente expira após cerca de sete minutos de inatividade.</span><span class="sxs-lookup"><span data-stu-id="991e5-150">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="991e5-151">A sessão não persistente expira após cerca de cinco minutos de inatividade.</span><span class="sxs-lookup"><span data-stu-id="991e5-151">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="991e5-152">Cenários comuns do Excel</span><span class="sxs-lookup"><span data-stu-id="991e5-152">Common Excel scenarios</span></span>

<span data-ttu-id="991e5-153">Esta seção fornece exemplos das operações comuns que você pode usar em objetos do Excel.</span><span class="sxs-lookup"><span data-stu-id="991e5-153">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="991e5-154">Operações de planilha</span><span class="sxs-lookup"><span data-stu-id="991e5-154">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="991e5-155">Listar a parte de planilhas da pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="991e5-155">List worksheets part of the workbook</span></span> 
<span data-ttu-id="991e5-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-156">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-157">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="991e5-158">Adicionar uma nova planilha</span><span class="sxs-lookup"><span data-stu-id="991e5-158">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="991e5-159">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-159">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="991e5-160">Obter uma nova planilha</span><span class="sxs-lookup"><span data-stu-id="991e5-160">Get a new worksheet</span></span> 

<span data-ttu-id="991e5-161">Obter uma planilha com base no nome.</span><span class="sxs-lookup"><span data-stu-id="991e5-161">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-162">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-162">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

<span data-ttu-id="991e5-p112">\*\* Observação: as planilhas também podem ser recuperadas usando a ID. No entanto, atualmente, a ID contém os caracteres `{` e '}' que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter uma planilha com a ID de `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, a URL codifica a ID no caminho como `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span><span class="sxs-lookup"><span data-stu-id="991e5-p112">\*\* Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="991e5-166">Excluir uma planilha</span><span class="sxs-lookup"><span data-stu-id="991e5-166">Delete a worksheet</span></span>

<span data-ttu-id="991e5-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-167">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-168">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-168">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="991e5-169">Atualizar as propriedades da planilha</span><span class="sxs-lookup"><span data-stu-id="991e5-169">Update worksheet properties</span></span>

<span data-ttu-id="991e5-170">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-170">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="991e5-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-171">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a><span data-ttu-id="991e5-172">Operações de gráfico</span><span class="sxs-lookup"><span data-stu-id="991e5-172">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="991e5-173">Listar gráficos que fazem parte da planilha</span><span class="sxs-lookup"><span data-stu-id="991e5-173">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="991e5-174">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-174">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="991e5-175">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-175">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

<span data-ttu-id="991e5-p113">\*\* Observação: a ID contém os caracteres `{` e `}` (exemplo: `{00000000-0008-0000-0100-000003000000}`) que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter um objeto gráfico, a URL codifica a ID no caminho como `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span><span class="sxs-lookup"><span data-stu-id="991e5-p113">\*\* Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="991e5-178">Obter imagem do gráfico</span><span class="sxs-lookup"><span data-stu-id="991e5-178">Get chart image</span></span>

<span data-ttu-id="991e5-179">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-179">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="991e5-180">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-180">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="991e5-181">Adicionar um gráfico</span><span class="sxs-lookup"><span data-stu-id="991e5-181">Add a chart</span></span>  

<span data-ttu-id="991e5-182">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-182">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="991e5-183">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-183">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#chart",
  "@odata.type": "#microsoft.graph.workbookChart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="991e5-184">Atualizar um gráfico</span><span class="sxs-lookup"><span data-stu-id="991e5-184">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="991e5-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-185">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a><span data-ttu-id="991e5-186">Atualizar dados de origem do gráfico</span><span class="sxs-lookup"><span data-stu-id="991e5-186">Update chart source data</span></span> 

<span data-ttu-id="991e5-187">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-187">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="991e5-188">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-188">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="991e5-189">Operações de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-189">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="991e5-190">Obter lista de tabelas</span><span class="sxs-lookup"><span data-stu-id="991e5-190">Get list of tables</span></span> 

<span data-ttu-id="991e5-191">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-191">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-192">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-192">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="991e5-193">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-193">Create table</span></span>

<span data-ttu-id="991e5-194">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-194">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/{table-id}/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="991e5-195">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-195">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="update-table"></a><span data-ttu-id="991e5-196">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-196">Update table</span></span>

<span data-ttu-id="991e5-197">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-197">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="991e5-198">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-198">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="991e5-199">Obter lista de linhas de tabelas</span><span class="sxs-lookup"><span data-stu-id="991e5-199">Get list of table rows</span></span>
<span data-ttu-id="991e5-200">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-200">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-201">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-201">Response</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="991e5-202">Obter lista de colunas de tabelas</span><span class="sxs-lookup"><span data-stu-id="991e5-202">Get list of table columns</span></span>

<span data-ttu-id="991e5-203">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-203">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-204">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-204">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a><span data-ttu-id="991e5-205">Adicionar uma linha de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-205">Add a table row</span></span>

<span data-ttu-id="991e5-206">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-206">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="991e5-207">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-207">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a><span data-ttu-id="991e5-208">Adicionar uma coluna de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-208">Add a table column</span></span> 

<span data-ttu-id="991e5-209">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-209">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="991e5-210">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-210">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a><span data-ttu-id="991e5-211">Excluir linha de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-211">Delete table row</span></span>

<span data-ttu-id="991e5-212">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-212">Request <!-- { "blockType": "ignored" } --></span></span>
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows/$/itemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-213">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-213">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="991e5-214">Excluir coluna de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-214">Delete table column</span></span> 
<span data-ttu-id="991e5-215">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-215">Request <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-216">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-216">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="991e5-217">Converter tabela em intervalo</span><span class="sxs-lookup"><span data-stu-id="991e5-217">Convert table to range</span></span> 
<span data-ttu-id="991e5-218">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-218">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-219">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-219">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="991e5-220">Classificação de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-220">Table sort</span></span>
<span data-ttu-id="991e5-221">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-221">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


<span data-ttu-id="991e5-222">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-222">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="991e5-223">Filtro de tabela</span><span class="sxs-lookup"><span data-stu-id="991e5-223">Table filter</span></span>
<span data-ttu-id="991e5-224">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-224">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

<span data-ttu-id="991e5-225">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-225">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="991e5-226">Limpar filtro</span><span class="sxs-lookup"><span data-stu-id="991e5-226">Clear filter</span></span>
<span data-ttu-id="991e5-227">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-227">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-228">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-228">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="991e5-229">Operações de intervalo</span><span class="sxs-lookup"><span data-stu-id="991e5-229">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="991e5-230">Obter intervalo</span><span class="sxs-lookup"><span data-stu-id="991e5-230">Get Range</span></span> 

<span data-ttu-id="991e5-231">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-231">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-232">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a><span data-ttu-id="991e5-233">Atualização de intervalo</span><span class="sxs-lookup"><span data-stu-id="991e5-233">Range update</span></span> 

<!-- { "blockType": "ignored" } -->
```http
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a><span data-ttu-id="991e5-234">Classificação de intervalo</span><span class="sxs-lookup"><span data-stu-id="991e5-234">Range sort</span></span>
<span data-ttu-id="991e5-235">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-235">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

<span data-ttu-id="991e5-236">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="991e5-236">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="991e5-237">Itens nomeados</span><span class="sxs-lookup"><span data-stu-id="991e5-237">Named items</span></span>
<span data-ttu-id="991e5-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-238">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="991e5-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-239">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a><span data-ttu-id="991e5-240">Trabalhar com nulos</span><span class="sxs-lookup"><span data-stu-id="991e5-240">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="991e5-241">entrada nula em uma matriz 2D</span><span class="sxs-lookup"><span data-stu-id="991e5-241">null input in 2-D array</span></span>

<span data-ttu-id="991e5-p114">A entrada `null` em uma matriz bidimensional (para valores, formato de número ou fórmula) é ignorada nos recursos Range e Table. Nenhuma atualização será realizada no destino pretendido (célula) quando a entrada `null` for enviada em valores, formato de número ou grade de fórmula de valores.</span><span class="sxs-lookup"><span data-stu-id="991e5-p114">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="991e5-244">Por exemplo, para atualizar somente partes específicas de Range, como o formato de número de uma célula, e para manter o formato de número existente em outras partes de Range, defina o formato de número onde for obrigatório e envie `null` para as outras células.</span><span class="sxs-lookup"><span data-stu-id="991e5-244">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="991e5-245">Na solicitação de definição a seguir, somente algumas partes do formato de número de Range são definidas, enquanto o formato de número existente na parte restante é mantido (por meio da transmissão de nulos).</span><span class="sxs-lookup"><span data-stu-id="991e5-245">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="991e5-246">entrada nula para uma propriedade</span><span class="sxs-lookup"><span data-stu-id="991e5-246">null input for a property</span></span>

<span data-ttu-id="991e5-p115">`null` não é uma entrada válida única para toda a propriedade. Por exemplo, o modelo a seguir não é válido, uma vez que os valores inteiros não podem ser ignorados ou definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="991e5-p115">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="991e5-249">O exemplo a seguir também não é válido, porque nulo não é um valor de cor válido.</span><span class="sxs-lookup"><span data-stu-id="991e5-249">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="991e5-250">Resposta nula</span><span class="sxs-lookup"><span data-stu-id="991e5-250">Null-Response</span></span>

<span data-ttu-id="991e5-251">Representação de propriedades de formatação que consiste em valores não uniformes que resultam no retorno de um valor nulo na resposta.</span><span class="sxs-lookup"><span data-stu-id="991e5-251">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="991e5-p116">Por exemplo, um intervalo pode consistir em uma ou mais células. Nos casos em que as células individuais incluídas no intervalo especificado não apresentam valores de formatação uniformes, a representação de nível do intervalo será indefinida.</span><span class="sxs-lookup"><span data-stu-id="991e5-p116">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="991e5-254">Entrada e saída em branco</span><span class="sxs-lookup"><span data-stu-id="991e5-254">Blank input and output</span></span>

<span data-ttu-id="991e5-p117">Valores em branco em solicitações de atualização são tratados como uma instrução para limpar ou redefinir a respectiva propriedade. Um valor em branco é representado por aspas duplas sem espaço entre elas: `""`</span><span class="sxs-lookup"><span data-stu-id="991e5-p117">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="991e5-257">Exemplos:</span><span class="sxs-lookup"><span data-stu-id="991e5-257">Examples:</span></span>

* <span data-ttu-id="991e5-258">Para `values`, o valor do intervalo é removido. Isso equivale a limpar o conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="991e5-258">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="991e5-259">Para `numberFormat`, o formato de número é definido como `General`.</span><span class="sxs-lookup"><span data-stu-id="991e5-259">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="991e5-260">Para `formula` e `formulaLocale`, os valores de fórmula são excluídos.</span><span class="sxs-lookup"><span data-stu-id="991e5-260">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="991e5-p118">Para operações de leitura, espera-se receber valores em branco caso o conteúdo das células esteja em branco. Quando a célula não inclui dados ou valores, a API retorna um valor em branco. O valor em branco é representado por aspas duplas sem espaço entre elas: `""`</span><span class="sxs-lookup"><span data-stu-id="991e5-p118">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a><span data-ttu-id="991e5-264">Intervalo não associado</span><span class="sxs-lookup"><span data-stu-id="991e5-264">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="991e5-265">Leitura</span><span class="sxs-lookup"><span data-stu-id="991e5-265">Read</span></span>

<span data-ttu-id="991e5-266">Um endereço de intervalo não associado contém apenas os identificadores de coluna ou de linha e identificador não especificado de linha ou de coluna, respectivamente, como:</span><span class="sxs-lookup"><span data-stu-id="991e5-266">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="991e5-267">`C:C`, `A:F`, `A:XFD` (inclui linhas não especificadas)</span><span class="sxs-lookup"><span data-stu-id="991e5-267">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="991e5-268">`2:2`, `1:4`, `1:1048546` (inclui colunas não especificadas)</span><span class="sxs-lookup"><span data-stu-id="991e5-268">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="991e5-p119">Quando a API faz uma solicitação para recuperar um intervalo não associado (`getRange('C:C')`), a resposta retornada contém `null` para as propriedades em nível de célula, como `values`, `text`, `numberFormat` ou `formula`. Outras propriedades de Range, como `address` ou `cellCount`, refletirão o intervalo não associado.</span><span class="sxs-lookup"><span data-stu-id="991e5-p119">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="991e5-271">Gravação</span><span class="sxs-lookup"><span data-stu-id="991e5-271">Write</span></span>

<span data-ttu-id="991e5-272">O sistema **não permite** a definição de propriedades de nível da célula (como values, numberFormat, etc.) em um intervalo não associado, pois a solicitação de entrada pode ser muito extensa para ser manipulada.</span><span class="sxs-lookup"><span data-stu-id="991e5-272">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="991e5-273">O exemplo a seguir não é uma solicitação de atualização válida, pois o intervalo solicitado não está associado.</span><span class="sxs-lookup"><span data-stu-id="991e5-273">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id}/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="991e5-274">Quando uma operação de atualização é tentada nesse intervalo, a API retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="991e5-274">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="991e5-275">Intervalo longo</span><span class="sxs-lookup"><span data-stu-id="991e5-275">Large Range</span></span>

<span data-ttu-id="991e5-p120">Um intervalo longo significa um intervalo cujo tamanho é muito grande para uma única chamada à API. Muitos fatores, como o número de células, os valores, os formatos de número e as fórmulas incluídas no intervalo, podem fazer com que a resposta seja tão extensa a ponto de se tornar inadequada para interação com a API. A API faz a melhor tentativa para retornar ou gravar os dados solicitados. No entanto, o tamanho extenso envolvido pode resultar em uma condição de erro da API devido à intensa utilização de recursos.</span><span class="sxs-lookup"><span data-stu-id="991e5-p120">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="991e5-280">Para evitar isso, convém fazer leituras ou gravações para um intervalo longo em vários tamanhos de intervalo menores.</span><span class="sxs-lookup"><span data-stu-id="991e5-280">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="991e5-281">Cópia de entrada única</span><span class="sxs-lookup"><span data-stu-id="991e5-281">Single input copy</span></span>

<span data-ttu-id="991e5-p121">Para dar suporte a atualização de um intervalo com os formatos de número ou valores idênticos, ou para a aplicação de uma mesma fórmula em um intervalo, você deve usar a seguinte convenção na API de configuração. No Excel, esse comportamento é semelhante a inserir valores ou fórmulas em um intervalo no modo Ctrl+Enter.</span><span class="sxs-lookup"><span data-stu-id="991e5-p121">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="991e5-284">A API vai procurar um *valor de célula única*, no entanto, se a dimensão do intervalo de destino não corresponder à dimensão do intervalo de entrada, ela aplicará a atualização ao intervalo inteiro no modo Ctrl+Enter com o valor ou fórmula fornecida na solicitação.</span><span class="sxs-lookup"><span data-stu-id="991e5-284">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="991e5-285">Exemplos</span><span class="sxs-lookup"><span data-stu-id="991e5-285">Examples</span></span>

<span data-ttu-id="991e5-p122">A solicitação a seguir atualiza o intervalo selecionado com "Texto de amostra". Observe que o intervalo tem 200 células, ao passo que a entrada fornecida tem apenas 1 valor de célula.</span><span class="sxs-lookup"><span data-stu-id="991e5-p122">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id}/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="991e5-288">Funções de pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="991e5-288">Workbook functions</span></span> 
<span data-ttu-id="991e5-289">Você pode acessar as funções de pasta de trabalho por meio de uma coleção de funções incluídas no recurso /Functions.</span><span class="sxs-lookup"><span data-stu-id="991e5-289">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="991e5-290">Solicitação</span><span class="sxs-lookup"><span data-stu-id="991e5-290">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a><span data-ttu-id="991e5-291">Resposta</span><span class="sxs-lookup"><span data-stu-id="991e5-291">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a><span data-ttu-id="991e5-292">Informações do erro</span><span class="sxs-lookup"><span data-stu-id="991e5-292">Error information</span></span> 

<span data-ttu-id="991e5-p123">Erros são retornados com um código de erro HTTP e um objeto de erro. Um `code` de erro e uma `message` explicam o motivo do erro.</span><span class="sxs-lookup"><span data-stu-id="991e5-p123">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="991e5-295">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="991e5-295">The following is an example.</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

