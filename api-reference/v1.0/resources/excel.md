# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="9bc1e-101">Trabalhando com o Excel no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="9bc1e-101">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="9bc1e-p101">É possível usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive for Business, site do SharePoint ou unidade do Grupo. O recurso `Workbook` (ou arquivo do Excel) contém todos os outros recursos do Excel por meio de relações. É possível acessar uma pasta de trabalho por meio da [API Drive](drive.md) identificando a localização do arquivo na URL. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p101">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive for Business, SharePoint site or Group drive. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="9bc1e-p102">Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho. Por exemplo, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p102">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="9bc1e-108">retorna uma coleção de todos os objetos da planilha que fazem parte da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-108">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="9bc1e-p103">A API REST do Excel só oferece suporte para pastas de trabalho formatadas pelo arquivo do Office Open XML. Não há suporte para pastas de trabalho de extensão de `.xls`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p103">The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

<span data-ttu-id="9bc1e-111">**Observação**: o suporte para pastas de trabalho armazenadas na plataforma de Consumidor do OneDrive ainda não está disponível.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-111">**Note**: Support for workbooks stored in OneDrive Consumer platform is still not available.</span></span> <span data-ttu-id="9bc1e-112">Neste momento, somente os arquivos armazenados em plataformas comerciais têm suporte das APIs REST do Excel.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-112">At this time, only the files stored in business platform is supported by Excel REST APIs.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="9bc1e-113">Autorização e escopos</span><span class="sxs-lookup"><span data-stu-id="9bc1e-113">Authorization and scopes</span></span>

<span data-ttu-id="9bc1e-114">Você pode usar o [ponto de extremidade do Azure AD v.2](https://developer.microsoft.com/graph/docs/authorization/converged_auth) para autenticar APIs do Excel.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-114">You can use the [Azure AD v.2 endpoint](https://developer.microsoft.com/graph/docs/authorization/converged_auth) to authenticate Excel APIs.</span></span> <span data-ttu-id="9bc1e-115">Todas as APIs exigem o cabeçalho HTTP `Authorization: Bearer {access-token}`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-115">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="9bc1e-116">Um dos seguintes [escopos de permissão](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) é obrigatório para usar o recurso do Excel:</span><span class="sxs-lookup"><span data-stu-id="9bc1e-116">One of the following [permission scopes](https://developer.microsoft.com/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="9bc1e-117">Files.Read (para ações de leitura)</span><span class="sxs-lookup"><span data-stu-id="9bc1e-117">Files.Read (for read actions)</span></span>
* <span data-ttu-id="9bc1e-118">Files.ReadWrite (para ações de leitura e gravação)</span><span class="sxs-lookup"><span data-stu-id="9bc1e-118">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="9bc1e-119">Sessões e persistência</span><span class="sxs-lookup"><span data-stu-id="9bc1e-119">Sessions and persistence</span></span>

<span data-ttu-id="9bc1e-120">As APIs do Excel podem ser chamadas em um destes três modos:</span><span class="sxs-lookup"><span data-stu-id="9bc1e-120">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="9bc1e-121">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas).</span><span class="sxs-lookup"><span data-stu-id="9bc1e-121">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="9bc1e-122">Esse é o modo de operação mais eficiente e com desempenho mais elevado.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-122">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="9bc1e-p107">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p107">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="9bc1e-127">Sem sessão ‒ a chamada à API é feita sem informações sobre a sessão.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-127">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="9bc1e-128">Os servidores do Excel têm que localizar a cópia do servidor de pasta de trabalho sempre que executam a operação. Portanto, essa não é uma maneira eficiente de chamar APIs do Excel.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-128">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="9bc1e-129">Ele é adequado para fazer solicitações únicas.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-129">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="9bc1e-130">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-130">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="9bc1e-p109">**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p109">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="9bc1e-134">Chamada à API para obter uma sessão</span><span class="sxs-lookup"><span data-stu-id="9bc1e-134">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="9bc1e-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-135">Request</span></span> 

<span data-ttu-id="9bc1e-136">Passe um objeto JSON definindo o valor de `persistchanges` como `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-136">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="9bc1e-137">Quando o valor de `persistChanges` está definido como `false`, uma id de sessão não persistente é retornada.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-137">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="9bc1e-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-138">Response</span></span>

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

#### <a name="usage"></a><span data-ttu-id="9bc1e-139">Uso</span><span class="sxs-lookup"><span data-stu-id="9bc1e-139">Usage</span></span> 

<span data-ttu-id="9bc1e-140">A ID de sessão retornada da chamada anterior é transmitida como um cabeçalho em solicitações de API subsequentes no</span><span class="sxs-lookup"><span data-stu-id="9bc1e-140">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="9bc1e-141">cabeçalho HTTP `workbook-session-id`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-141">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="9bc1e-142">Observação: se a id da sessão tiver expirado, um código de erro HTTP `404` será retornado na sessão.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-142">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="9bc1e-143">Nesse cenário, você pode optar por criar uma nova sessão e continuar.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-143">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="9bc1e-144">Outra abordagem seria atualizar a sessão periodicamente para manter a sessão ativa.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-144">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="9bc1e-145">Normalmente, a sessão persistente expira após cerca de sete minutos de inatividade.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-145">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="9bc1e-146">A sessão não persistente expira após cerca de cinco minutos de inatividade.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-146">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="9bc1e-147">Cenários comuns do Excel</span><span class="sxs-lookup"><span data-stu-id="9bc1e-147">Common Excel scenarios</span></span>

<span data-ttu-id="9bc1e-148">Esta seção fornece exemplos das operações comuns que você pode usar em objetos do Excel.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-148">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="9bc1e-149">Operações de planilha</span><span class="sxs-lookup"><span data-stu-id="9bc1e-149">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="9bc1e-150">Listar a parte de planilhas da pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="9bc1e-150">List worksheets part of the workbook</span></span> 
<span data-ttu-id="9bc1e-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-151">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-152">Response</span></span>

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
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="9bc1e-153">Adicionar uma nova planilha</span><span class="sxs-lookup"><span data-stu-id="9bc1e-153">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="9bc1e-154">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-154">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="9bc1e-155">Obter uma nova planilha</span><span class="sxs-lookup"><span data-stu-id="9bc1e-155">Get a new worksheet</span></span> 

<span data-ttu-id="9bc1e-156">Obter uma planilha com base no nome.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-156">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-157">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-157">Response <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="9bc1e-p111">\*\* Observação: as planilhas também podem ser recuperadas usando a ID. No entanto, atualmente, a ID contém os caracteres `{` e '}' que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter uma planilha com a ID de `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, a URL codifica a ID no caminho como `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p111">\*\* Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="9bc1e-161">Excluir uma planilha</span><span class="sxs-lookup"><span data-stu-id="9bc1e-161">Delete a worksheet</span></span>

<span data-ttu-id="9bc1e-162">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-162">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-163">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-163">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="9bc1e-164">Atualizar as propriedades da planilha</span><span class="sxs-lookup"><span data-stu-id="9bc1e-164">Update worksheet properties</span></span>

<span data-ttu-id="9bc1e-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-165">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="9bc1e-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-166">Response</span></span>

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

### <a name="chart-operations"></a><span data-ttu-id="9bc1e-167">Operações de gráfico</span><span class="sxs-lookup"><span data-stu-id="9bc1e-167">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="9bc1e-168">Listar gráficos que fazem parte da planilha</span><span class="sxs-lookup"><span data-stu-id="9bc1e-168">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="9bc1e-169">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-169">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="9bc1e-170">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-170">Response <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="9bc1e-p112">\*\* Observação: a ID contém os caracteres `{` e `}` (exemplo: `{00000000-0008-0000-0100-000003000000}`) que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter um objeto gráfico, a URL codifica a ID no caminho como `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p112">\*\* Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="9bc1e-173">Obter imagem do gráfico</span><span class="sxs-lookup"><span data-stu-id="9bc1e-173">Get chart image</span></span>

<span data-ttu-id="9bc1e-174">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-174">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="9bc1e-175">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-175">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="9bc1e-176">Adicionar um gráfico</span><span class="sxs-lookup"><span data-stu-id="9bc1e-176">Add a chart</span></span>  

<span data-ttu-id="9bc1e-177">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-177">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="9bc1e-178">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-178">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="update-a-chart"></a><span data-ttu-id="9bc1e-179">Atualizar um gráfico</span><span class="sxs-lookup"><span data-stu-id="9bc1e-179">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="9bc1e-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-180">Response</span></span> 

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

#### <a name="update-chart-source-data"></a><span data-ttu-id="9bc1e-181">Atualizar dados de origem do gráfico</span><span class="sxs-lookup"><span data-stu-id="9bc1e-181">Update chart source data</span></span> 

<span data-ttu-id="9bc1e-182">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-182">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="9bc1e-183">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-183">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="9bc1e-184">Operações de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-184">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="9bc1e-185">Obter lista de tabelas</span><span class="sxs-lookup"><span data-stu-id="9bc1e-185">Get list of tables</span></span> 

<span data-ttu-id="9bc1e-186">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-186">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-187">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-187">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="9bc1e-188">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-188">Create table</span></span>

<span data-ttu-id="9bc1e-189">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-189">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/{table-id}/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="9bc1e-190">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-190">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="update-table"></a><span data-ttu-id="9bc1e-191">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-191">Update table</span></span>

<span data-ttu-id="9bc1e-192">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-192">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="9bc1e-193">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-193">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="9bc1e-194">Obter lista de linhas de tabelas</span><span class="sxs-lookup"><span data-stu-id="9bc1e-194">Get list of table rows</span></span>
<span data-ttu-id="9bc1e-195">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-195">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-196">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-196">Response</span></span>

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

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="9bc1e-197">Obter lista de colunas de tabelas</span><span class="sxs-lookup"><span data-stu-id="9bc1e-197">Get list of table columns</span></span>

<span data-ttu-id="9bc1e-198">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-198">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-199">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-199">Response</span></span> 

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


#### <a name="add-a-table-row"></a><span data-ttu-id="9bc1e-200">Adicionar uma linha de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-200">Add a table row</span></span>

<span data-ttu-id="9bc1e-201">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-201">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="9bc1e-202">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-202">Response <!-- { "blockType": "ignored" } --></span></span>
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

#### <a name="add-a-table-column"></a><span data-ttu-id="9bc1e-203">Adicionar uma coluna de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-203">Add a table column</span></span> 

<span data-ttu-id="9bc1e-204">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-204">Request <!-- { "blockType": "ignored" } --></span></span>
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="9bc1e-205">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-205">Response</span></span> 

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

#### <a name="delete-table-row"></a><span data-ttu-id="9bc1e-206">Excluir linha de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-206">Delete table row</span></span>

<span data-ttu-id="9bc1e-207">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-207">Request <!-- { "blockType": "ignored" } --></span></span>
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows/$/itemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-208">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-208">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="9bc1e-209">Excluir coluna de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-209">Delete table column</span></span> 
<span data-ttu-id="9bc1e-210">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-210">Request <!-- { "blockType": "ignored" } --></span></span>
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-211">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-211">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="9bc1e-212">Converter tabela em intervalo</span><span class="sxs-lookup"><span data-stu-id="9bc1e-212">Convert table to range</span></span> 
<span data-ttu-id="9bc1e-213">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-213">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-214">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-214">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="9bc1e-215">Classificação de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-215">Table sort</span></span>
<span data-ttu-id="9bc1e-216">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-216">Request <!-- { "blockType": "ignored" } --></span></span>
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


<span data-ttu-id="9bc1e-217">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-217">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="9bc1e-218">Filtro de tabela</span><span class="sxs-lookup"><span data-stu-id="9bc1e-218">Table filter</span></span>
<span data-ttu-id="9bc1e-219">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-219">Request <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="9bc1e-220">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-220">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="9bc1e-221">Limpar filtro</span><span class="sxs-lookup"><span data-stu-id="9bc1e-221">Clear filter</span></span>
<span data-ttu-id="9bc1e-222">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-222">Request <!-- { "blockType": "ignored" } --></span></span>
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-223">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-223">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="9bc1e-224">Operações de intervalo</span><span class="sxs-lookup"><span data-stu-id="9bc1e-224">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="9bc1e-225">Obter intervalo</span><span class="sxs-lookup"><span data-stu-id="9bc1e-225">Get Range</span></span> 

<span data-ttu-id="9bc1e-226">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-226">Request <!-- { "blockType": "ignored" } --></span></span>
```http
GET /{version}/me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-227">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-227">Response</span></span> 

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

#### <a name="range-update"></a><span data-ttu-id="9bc1e-228">Atualização de intervalo</span><span class="sxs-lookup"><span data-stu-id="9bc1e-228">Range update</span></span> 

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

#### <a name="range-sort"></a><span data-ttu-id="9bc1e-229">Classificação de intervalo</span><span class="sxs-lookup"><span data-stu-id="9bc1e-229">Range sort</span></span>
<span data-ttu-id="9bc1e-230">Solicitação<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-230">Request <!-- { "blockType": "ignored" } --></span></span>
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

<span data-ttu-id="9bc1e-231">Resposta<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="9bc1e-231">Response <!-- { "blockType": "ignored" } --></span></span>
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="9bc1e-232">Itens nomeados</span><span class="sxs-lookup"><span data-stu-id="9bc1e-232">Named items</span></span>
<span data-ttu-id="9bc1e-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-233">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="9bc1e-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-234">Response</span></span> 

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

### <a name="work-with-nulls"></a><span data-ttu-id="9bc1e-235">Trabalhar com nulos</span><span class="sxs-lookup"><span data-stu-id="9bc1e-235">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="9bc1e-236">entrada nula em uma matriz 2D</span><span class="sxs-lookup"><span data-stu-id="9bc1e-236">null input in 2-D array</span></span>

<span data-ttu-id="9bc1e-p113">A entrada `null` em uma matriz bidimensional (para valores, formato de número ou fórmula) é ignorada nos recursos Range e Table. Nenhuma atualização será realizada no destino pretendido (célula) quando a entrada `null` for enviada em valores, formato de número ou grade de fórmula de valores.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p113">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="9bc1e-239">Por exemplo, para atualizar somente partes específicas de Range, como o formato de número de uma célula, e para manter o formato de número existente em outras partes de Range, defina o formato de número onde for obrigatório e envie `null` para as outras células.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-239">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="9bc1e-240">Na solicitação de definição a seguir, somente algumas partes do formato de número de Range são definidas, enquanto o formato de número existente na parte restante é mantido (por meio da transmissão de nulos).</span><span class="sxs-lookup"><span data-stu-id="9bc1e-240">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="9bc1e-241">entrada nula para uma propriedade</span><span class="sxs-lookup"><span data-stu-id="9bc1e-241">null input for a property</span></span>

<span data-ttu-id="9bc1e-p114">`null` não é uma entrada válida única para toda a propriedade. Por exemplo, o modelo a seguir não é válido, uma vez que os valores inteiros não podem ser ignorados ou definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p114">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="9bc1e-244">O exemplo a seguir também não é válido, porque nulo não é um valor de cor válido.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-244">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="9bc1e-245">Resposta nula</span><span class="sxs-lookup"><span data-stu-id="9bc1e-245">Null-Response</span></span>

<span data-ttu-id="9bc1e-246">Representação de propriedades de formatação que consiste em valores não uniformes que resultam no retorno de um valor nulo na resposta.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-246">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="9bc1e-p115">Por exemplo, um intervalo pode consistir em uma ou mais células. Nos casos em que as células individuais incluídas no intervalo especificado não apresentam valores de formatação uniformes, a representação de nível do intervalo será indefinida.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p115">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="9bc1e-249">Entrada e saída em branco</span><span class="sxs-lookup"><span data-stu-id="9bc1e-249">Blank input and output</span></span>

<span data-ttu-id="9bc1e-p116">Valores em branco em solicitações de atualização são tratados como uma instrução para limpar ou redefinir a respectiva propriedade. Um valor em branco é representado por aspas duplas sem espaço entre elas: `""`</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p116">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="9bc1e-252">Exemplos:</span><span class="sxs-lookup"><span data-stu-id="9bc1e-252">Examples:</span></span>

* <span data-ttu-id="9bc1e-253">Para `values`, o valor do intervalo é removido. Isso equivale a limpar o conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-253">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="9bc1e-254">Para `numberFormat`, o formato de número é definido como `General`.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-254">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="9bc1e-255">Para `formula` e `formulaLocale`, os valores de fórmula são excluídos.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-255">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="9bc1e-p117">Para operações de leitura, espera-se receber valores em branco caso o conteúdo das células esteja em branco. Quando a célula não inclui dados ou valores, a API retorna um valor em branco. O valor em branco é representado por aspas duplas sem espaço entre elas: `""`</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p117">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

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


### <a name="unbounded-range"></a><span data-ttu-id="9bc1e-259">Intervalo não associado</span><span class="sxs-lookup"><span data-stu-id="9bc1e-259">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="9bc1e-260">Leitura</span><span class="sxs-lookup"><span data-stu-id="9bc1e-260">Read</span></span>

<span data-ttu-id="9bc1e-261">Um endereço de intervalo não associado contém apenas os identificadores de coluna ou de linha e identificador não especificado de linha ou de coluna, respectivamente, como:</span><span class="sxs-lookup"><span data-stu-id="9bc1e-261">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="9bc1e-262">`C:C`, `A:F`, `A:XFD` (inclui linhas não especificadas)</span><span class="sxs-lookup"><span data-stu-id="9bc1e-262">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="9bc1e-263">`2:2`, `1:4`, `1:1048546` (inclui colunas não especificadas)</span><span class="sxs-lookup"><span data-stu-id="9bc1e-263">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="9bc1e-p118">Quando a API faz uma solicitação para recuperar um intervalo não associado (`getRange('C:C')`), a resposta retornada contém `null` para as propriedades em nível de célula, como `values`, `text`, `numberFormat` ou `formula`. Outras propriedades de Range, como `address` ou `cellCount`, refletirão o intervalo não associado.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p118">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="9bc1e-266">Gravação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-266">Write</span></span>

<span data-ttu-id="9bc1e-267">O sistema **não permite** a definição de propriedades de nível da célula (como values, numberFormat, etc.) em um intervalo não associado, pois a solicitação de entrada pode ser muito extensa para ser manipulada.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-267">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="9bc1e-268">O exemplo a seguir não é uma solicitação de atualização válida, pois o intervalo solicitado não está associado.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-268">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id}/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="9bc1e-269">Quando uma operação de atualização é tentada nesse intervalo, a API retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-269">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="9bc1e-270">Intervalo longo</span><span class="sxs-lookup"><span data-stu-id="9bc1e-270">Large Range</span></span>

<span data-ttu-id="9bc1e-p119">Um intervalo longo significa um intervalo cujo tamanho é muito grande para uma única chamada à API. Muitos fatores, como o número de células, os valores, os formatos de número e as fórmulas incluídas no intervalo, podem fazer com que a resposta seja tão extensa a ponto de se tornar inadequada para interação com a API. A API faz a melhor tentativa para retornar ou gravar os dados solicitados. No entanto, o tamanho extenso envolvido pode resultar em uma condição de erro da API devido à intensa utilização de recursos.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p119">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="9bc1e-275">Para evitar isso, convém fazer leituras ou gravações para um intervalo longo em vários tamanhos de intervalo menores.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-275">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="9bc1e-276">Cópia de entrada única</span><span class="sxs-lookup"><span data-stu-id="9bc1e-276">Single input copy</span></span>

<span data-ttu-id="9bc1e-p120">Para dar suporte a atualização de um intervalo com os formatos de número ou valores idênticos, ou para a aplicação de uma mesma fórmula em um intervalo, você deve usar a seguinte convenção na API de configuração. No Excel, esse comportamento é semelhante a inserir valores ou fórmulas em um intervalo no modo Ctrl+Enter.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p120">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="9bc1e-279">A API vai procurar um *valor de célula única*, no entanto, se a dimensão do intervalo de destino não corresponder à dimensão do intervalo de entrada, ela aplicará a atualização ao intervalo inteiro no modo Ctrl+Enter com o valor ou fórmula fornecida na solicitação.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-279">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="9bc1e-280">Exemplos</span><span class="sxs-lookup"><span data-stu-id="9bc1e-280">Examples</span></span>

<span data-ttu-id="9bc1e-p121">A solicitação a seguir atualiza o intervalo selecionado com "Texto de amostra". Observe que o intervalo tem 200 células, ao passo que a entrada fornecida tem apenas 1 valor de célula.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p121">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id}/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="9bc1e-283">Funções de pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="9bc1e-283">Workbook functions</span></span> 
<span data-ttu-id="9bc1e-284">Você pode acessar as funções de pasta de trabalho por meio de uma coleção de funções incluídas no recurso /Functions.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-284">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="9bc1e-285">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9bc1e-285">Request</span></span>
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


##### <a name="response"></a><span data-ttu-id="9bc1e-286">Resposta</span><span class="sxs-lookup"><span data-stu-id="9bc1e-286">Response</span></span> 

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

## <a name="error-information"></a><span data-ttu-id="9bc1e-287">Informações do erro</span><span class="sxs-lookup"><span data-stu-id="9bc1e-287">Error information</span></span> 

<span data-ttu-id="9bc1e-p122">Erros são retornados com um código de erro HTTP e um objeto de erro. Um `code` de erro e uma `message` explicam o motivo do erro.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-p122">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="9bc1e-290">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="9bc1e-290">The following is an example.</span></span>

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

