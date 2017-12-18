# <a name="working-with-excel-in-microsoft-graph"></a><span data-ttu-id="e2688-101">Trabalhando com o Excel no Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="e2688-101">Working with Excel in Microsoft Graph</span></span>

<span data-ttu-id="e2688-p101">Você pode usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive, no SharePoint ou em outras plataformas de armazenamento com suporte. O recurso `Workbook` (ou arquivo do Excel) contém todos os outros recursos do Excel por meio de relações. Você pode acessar uma pasta de trabalho por meio da [API Drive](drive.md) identificando a localização do arquivo na URL. Por exemplo:</span><span class="sxs-lookup"><span data-stu-id="e2688-p101">You can use Microsoft Graph to allow web and mobile applications to read and modify Excel workbooks stored in OneDrive, SharePoint, or other supported storage platforms. The `Workbook` (or Excel file) resource contains all the other Excel resources through relationships. You can access a workbook through the [Drive API](drive.md) by identifying the location of the file in the URL. For example:</span></span>

`https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/{version}/me/drive/root:/{item-path}:/workbook/`  

<span data-ttu-id="e2688-p102">Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho. Por exemplo, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span><span class="sxs-lookup"><span data-stu-id="e2688-p102">You can access a set of Excel objects (such as Table, Range, or Chart) by using standard REST APIs to perform  create, read, update, and delete (CRUD) operations on the workbook. For example, `GET https://graph.microsoft.com/{version}/me/drive/items/{id}/workbook/worksheets`</span></span>  
<span data-ttu-id="e2688-108">retorna uma coleção de todos os objetos da planilha que fazem parte da pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e2688-108">returns a collection of worksheet objects that are part of the workbook.</span></span>    


<span data-ttu-id="e2688-p103">**Observação:** a API REST do Excel só oferece suporte para pastas de trabalho formatadas pelo arquivo do Office Open XML. Não há suporte para pastas de trabalho de extensão de `.xls`.</span><span class="sxs-lookup"><span data-stu-id="e2688-p103">**Note:** The Excel REST API supports only Office Open XML file formatted workbooks. The `.xls` extension workbooks are not supported.</span></span> 

## <a name="authorization-and-scopes"></a><span data-ttu-id="e2688-111">Autorização e escopos</span><span class="sxs-lookup"><span data-stu-id="e2688-111">Authorization and scopes</span></span>

<span data-ttu-id="e2688-112">Você pode usar o [ponto de extremidade do Azure AD v.2](https://developer.microsoft.com/pt-BR/graph/docs/authorization/converged_auth) para autenticar APIs do Excel.</span><span class="sxs-lookup"><span data-stu-id="e2688-112">You can use the [Azure AD v.2 endpoint](https://developer.microsoft.com/pt-BR/graph/docs/authorization/converged_auth) to authenticate Excel APIs.</span></span> <span data-ttu-id="e2688-113">Todas as APIs exigem o cabeçalho HTTP `Authorization: Bearer {access-token}`.</span><span class="sxs-lookup"><span data-stu-id="e2688-113">All APIs require the `Authorization: Bearer {access-token}` HTTP header.</span></span>   
  
<span data-ttu-id="e2688-114">Um dos seguintes [escopos de permissão](https://developer.microsoft.com/pt-BR/graph/docs/authorization/permission_scopes) é obrigatório para usar o recurso do Excel:</span><span class="sxs-lookup"><span data-stu-id="e2688-114">One of the following [permission scopes](https://developer.microsoft.com/pt-BR/graph/docs/authorization/permission_scopes) is required to use the Excel resource:</span></span>

* <span data-ttu-id="e2688-115">Files.Read (para ações de leitura)</span><span class="sxs-lookup"><span data-stu-id="e2688-115">Files.Read (for read actions)</span></span>
* <span data-ttu-id="e2688-116">Files.ReadWrite (para ações de leitura e gravação)</span><span class="sxs-lookup"><span data-stu-id="e2688-116">Files.ReadWrite (for read and write actions)</span></span>


## <a name="sessions-and-persistence"></a><span data-ttu-id="e2688-117">Sessões e persistência</span><span class="sxs-lookup"><span data-stu-id="e2688-117">Sessions and persistence</span></span>

<span data-ttu-id="e2688-118">As APIs do Excel podem ser chamadas em um destes três modos:</span><span class="sxs-lookup"><span data-stu-id="e2688-118">Excel APIs can be called in one of three modes:</span></span> 

1. <span data-ttu-id="e2688-119">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas).</span><span class="sxs-lookup"><span data-stu-id="e2688-119">Persistent session - All changes made to the workbook are persisted (saved).</span></span> <span data-ttu-id="e2688-120">Esse é o modo de operação mais eficiente e com desempenho mais elevado.</span><span class="sxs-lookup"><span data-stu-id="e2688-120">This is the most efficient and performant mode of operation.</span></span> 
2. <span data-ttu-id="e2688-p106">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="e2688-p106">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span> 
3. <span data-ttu-id="e2688-125">Sem sessão ‒ a chamada à API é feita sem informações sobre a sessão.</span><span class="sxs-lookup"><span data-stu-id="e2688-125">Sessionless - The API call is made without session information.</span></span> <span data-ttu-id="e2688-126">Os servidores do Excel têm que localizar a cópia do servidor de pasta de trabalho sempre que executam a operação. Portanto, essa não é uma maneira eficiente de chamar APIs do Excel.</span><span class="sxs-lookup"><span data-stu-id="e2688-126">Excel servers have to locate the server's copy of the workbook each time to perform the operation and hence this is not an efficient way for call Excel APIs.</span></span> <span data-ttu-id="e2688-127">Ele é adequado para fazer solicitações únicas.</span><span class="sxs-lookup"><span data-stu-id="e2688-127">It is suitable for making one off requests.</span></span> 

<span data-ttu-id="e2688-128">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="e2688-128">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="e2688-p108">**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="e2688-p108">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

### <a name="api-call-to-get-a-session"></a><span data-ttu-id="e2688-132">Chamada à API para obter uma sessão</span><span class="sxs-lookup"><span data-stu-id="e2688-132">API call to get a session</span></span> 

#### <a name="request"></a><span data-ttu-id="e2688-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-133">Request</span></span> 

<span data-ttu-id="e2688-134">Passe um objeto JSON definindo o valor de `persistchanges` como `true` ou `false`.</span><span class="sxs-lookup"><span data-stu-id="e2688-134">Pass a JSON object by setting the `persistchanges` value to `true` or `false`.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

<span data-ttu-id="e2688-135">Quando o valor de `persistChanges` está definido como `false`, uma id de sessão não persistente é retornada.</span><span class="sxs-lookup"><span data-stu-id="e2688-135">When the value of `persistChanges` is set to `false`, a non-persistent session id is returned.</span></span>  


#### <a name="response"></a><span data-ttu-id="e2688-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-136">Response</span></span>

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

#### <a name="usage"></a><span data-ttu-id="e2688-137">Uso</span><span class="sxs-lookup"><span data-stu-id="e2688-137">Usage</span></span> 

<span data-ttu-id="e2688-138">A ID de sessão retornada da chamada anterior é transmitida como um cabeçalho em solicitações de API subsequentes no</span><span class="sxs-lookup"><span data-stu-id="e2688-138">The session ID returned from the previous call is passed as a header on subsequent API requests in</span></span>  
<span data-ttu-id="e2688-139">cabeçalho HTTP `workbook-session-id`.</span><span class="sxs-lookup"><span data-stu-id="e2688-139">`workbook-session-id` HTTP header.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

><span data-ttu-id="e2688-140">Observação: se a id da sessão tiver expirado, um código de erro HTTP `404` será retornado na sessão.</span><span class="sxs-lookup"><span data-stu-id="e2688-140">Note: If the session id has expired, a `404` HTTP error code is returned on the session.</span></span> <span data-ttu-id="e2688-141">Nesse cenário, você pode optar por criar uma nova sessão e continuar.</span><span class="sxs-lookup"><span data-stu-id="e2688-141">In such a scenarion, you can choose to create a new session and continue.</span></span> <span data-ttu-id="e2688-142">Outra abordagem seria atualizar a sessão periodicamente para manter a sessão ativa.</span><span class="sxs-lookup"><span data-stu-id="e2688-142">Another approach would be to refresh the session periodically to keep the session alive.</span></span> <span data-ttu-id="e2688-143">Normalmente, a sessão persistente expira após cerca de sete minutos de inatividade.</span><span class="sxs-lookup"><span data-stu-id="e2688-143">Typically the persistent session expires after about 7 minutes of inactivity.</span></span> <span data-ttu-id="e2688-144">A sessão não persistente expira após cerca de cinco minutos de inatividade.</span><span class="sxs-lookup"><span data-stu-id="e2688-144">Non persistent session expires after about 5 minutes of inactivity.</span></span> 

## <a name="common-excel-scenarios"></a><span data-ttu-id="e2688-145">Cenários comuns do Excel</span><span class="sxs-lookup"><span data-stu-id="e2688-145">Common Excel scenarios</span></span>

<span data-ttu-id="e2688-146">Esta seção fornece exemplos das operações comuns que você pode usar em objetos do Excel.</span><span class="sxs-lookup"><span data-stu-id="e2688-146">This section provides examples of the common operations you can use on Excel objects.</span></span>

### <a name="worksheet-operations"></a><span data-ttu-id="e2688-147">Operações de planilha</span><span class="sxs-lookup"><span data-stu-id="e2688-147">Worksheet operations</span></span>

#### <a name="list-worksheets-part-of-the-workbook"></a><span data-ttu-id="e2688-148">Listar a parte de planilhas da pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="e2688-148">List worksheets part of the workbook</span></span> 
<span data-ttu-id="e2688-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-149">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-150">Response</span></span>

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
#### <a name="add-a-new-worksheet"></a><span data-ttu-id="e2688-151">Adicionar uma nova planilha</span><span class="sxs-lookup"><span data-stu-id="e2688-151">Add a new worksheet</span></span> 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

<span data-ttu-id="e2688-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-152">Response</span></span> 
<!-- { "blockType": "ignored" } -->
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

#### <a name="get-a-new-worksheet"></a><span data-ttu-id="e2688-153">Obter uma nova planilha</span><span class="sxs-lookup"><span data-stu-id="e2688-153">Get a new worksheet</span></span> 

<span data-ttu-id="e2688-154">Obter uma planilha com base no nome.</span><span class="sxs-lookup"><span data-stu-id="e2688-154">Get a worksheet based on the name.</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-155">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-155">Response</span></span> 
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="e2688-p110">** Observação: as planilhas também podem ser recuperadas usando a ID. No entanto, atualmente, a ID contém os caracteres `{` e '}' que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter uma planilha com a ID de `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, a URL codifica a ID no caminho como `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span><span class="sxs-lookup"><span data-stu-id="e2688-p110">** Note: Worksheets can also be retrieved using the ID. However, currently the ID contains `{` and '}' characters, which needs to be URL encoded for the API to work. Example: In order to get a worksheet with ID of `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, URL encode the ID in the path as `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`.</span></span> 

#### <a name="delete-a-worksheet"></a><span data-ttu-id="e2688-159">Excluir uma planilha</span><span class="sxs-lookup"><span data-stu-id="e2688-159">Delete a worksheet</span></span>

<span data-ttu-id="e2688-160">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-160">Request</span></span>
```
DELETE /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-161">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a><span data-ttu-id="e2688-162">Atualizar as propriedades da planilha</span><span class="sxs-lookup"><span data-stu-id="e2688-162">Update worksheet properties</span></span>

<span data-ttu-id="e2688-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-163">Request</span></span> 

```
PATCH /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

<span data-ttu-id="e2688-164">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-164">Response</span></span>

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

### <a name="chart-operations"></a><span data-ttu-id="e2688-165">Operações de gráfico</span><span class="sxs-lookup"><span data-stu-id="e2688-165">Chart operations</span></span>

#### <a name="list-charts-that-are-part-of-the-worksheet"></a><span data-ttu-id="e2688-166">Listar gráficos que fazem parte da planilha</span><span class="sxs-lookup"><span data-stu-id="e2688-166">List charts that are part of the worksheet</span></span> 

<span data-ttu-id="e2688-167">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-167">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="e2688-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-168">Response</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="e2688-p111">** Observação: a ID contém os caracteres `{` e `}` (exemplo: `{00000000-0008-0000-0100-000003000000}`) que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter um objeto gráfico, a URL codifica a ID no caminho como `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span><span class="sxs-lookup"><span data-stu-id="e2688-p111">** Note: Chart ID contains `{` and `}` characters (example: `{00000000-0008-0000-0100-000003000000}`), which needs to be URL encoded for the API to work. Example: In order to get a chart object, URL encode the ID in the path as `/charts/%7B00000000-0008-0000-0100-000003000000%7D`.</span></span> 

#### <a name="get-chart-image"></a><span data-ttu-id="e2688-171">Obter imagem do gráfico</span><span class="sxs-lookup"><span data-stu-id="e2688-171">Get chart image</span></span>

<span data-ttu-id="e2688-172">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-172">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

<span data-ttu-id="e2688-173">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-173">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a><span data-ttu-id="e2688-174">Adicionar um gráfico</span><span class="sxs-lookup"><span data-stu-id="e2688-174">Add a chart</span></span>  

<span data-ttu-id="e2688-175">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-175">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

<span data-ttu-id="e2688-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-176">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#chart",
  "@odata.type": "#microsoft.graph.chart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a><span data-ttu-id="e2688-177">Atualizar um gráfico</span><span class="sxs-lookup"><span data-stu-id="e2688-177">Update a chart</span></span>

<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
<span data-ttu-id="e2688-178">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-178">Response</span></span> 

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

#### <a name="update-chart-source-data"></a><span data-ttu-id="e2688-179">Atualizar dados de origem do gráfico</span><span class="sxs-lookup"><span data-stu-id="e2688-179">Update chart source data</span></span> 

<span data-ttu-id="e2688-180">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-180">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

<span data-ttu-id="e2688-181">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-181">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a><span data-ttu-id="e2688-182">Operações de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-182">Table operations</span></span> 

#### <a name="get-list-of-tables"></a><span data-ttu-id="e2688-183">Obter lista de tabelas</span><span class="sxs-lookup"><span data-stu-id="e2688-183">Get list of tables</span></span> 

<span data-ttu-id="e2688-184">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-184">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-185">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-185">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a><span data-ttu-id="e2688-186">Criar tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-186">Create Table</span></span>

<span data-ttu-id="e2688-187">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-187">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/$/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="e2688-188">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-188">Response</span></span> 
<!-- { "blockType": "ignored" } -->
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

#### <a name="update-table"></a><span data-ttu-id="e2688-189">Atualizar tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-189">Update table</span></span>

<span data-ttu-id="e2688-190">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-190">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
PATCH /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

<span data-ttu-id="e2688-191">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-191">Response</span></span> 
<!-- { "blockType": "ignored" } -->
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

#### <a name="get-list-of-table-rows"></a><span data-ttu-id="e2688-192">Obter lista de linhas de tabelas</span><span class="sxs-lookup"><span data-stu-id="e2688-192">Get list of table rows</span></span>
<span data-ttu-id="e2688-193">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-193">Request</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-194">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-194">Response</span></span>

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

#### <a name="get-list-of-table-columns"></a><span data-ttu-id="e2688-195">Obter lista de colunas de tabelas</span><span class="sxs-lookup"><span data-stu-id="e2688-195">Get list of table columns</span></span>

<span data-ttu-id="e2688-196">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-196">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-197">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-197">Response</span></span> 

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


#### <a name="add-a-table-row"></a><span data-ttu-id="e2688-198">Adicionar uma linha de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-198">Add a table row</span></span>

<span data-ttu-id="e2688-199">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-199">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

<span data-ttu-id="e2688-200">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-200">Response</span></span> 
<!-- { "blockType": "ignored" } -->
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

#### <a name="add-a-table-column"></a><span data-ttu-id="e2688-201">Adicionar uma coluna de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-201">Add a table column</span></span> 

<span data-ttu-id="e2688-202">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-202">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http 
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/Columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

<span data-ttu-id="e2688-203">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-203">Response</span></span> 

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

#### <a name="delete-table-row"></a><span data-ttu-id="e2688-204">Excluir linha de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-204">Delete table row</span></span>

<span data-ttu-id="e2688-205">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-205">Request</span></span> 
<!-- { "blockType": "ignored" } -->
```http  
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Rows/$/ItemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-206">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-206">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a><span data-ttu-id="e2688-207">Excluir coluna de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-207">Delete table column</span></span> 
<span data-ttu-id="e2688-208">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-208">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/Columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-209">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-209">Response</span></span> 
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a><span data-ttu-id="e2688-210">Converter tabela em intervalo</span><span class="sxs-lookup"><span data-stu-id="e2688-210">Convert table to range</span></span> 
<span data-ttu-id="e2688-211">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-211">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-212">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a><span data-ttu-id="e2688-213">Classificação de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-213">Table sort</span></span>
<span data-ttu-id="e2688-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-214">Request</span></span>
<!-- { "blockType": "ignored" } -->
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


<span data-ttu-id="e2688-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-215">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a><span data-ttu-id="e2688-216">Filtro de tabela</span><span class="sxs-lookup"><span data-stu-id="e2688-216">Table filter</span></span>
<span data-ttu-id="e2688-217">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-217">Request</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="e2688-218">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-218">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a><span data-ttu-id="e2688-219">Limpar filtro</span><span class="sxs-lookup"><span data-stu-id="e2688-219">Clear filter</span></span>
<span data-ttu-id="e2688-220">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-220">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-221">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-221">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a><span data-ttu-id="e2688-222">Operações de intervalo</span><span class="sxs-lookup"><span data-stu-id="e2688-222">Range operations</span></span>

#### <a name="get-range"></a><span data-ttu-id="e2688-223">Obter intervalo</span><span class="sxs-lookup"><span data-stu-id="e2688-223">Get Range</span></span> 

<span data-ttu-id="e2688-224">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-224">Request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-225">Response</span></span> 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#range",
  "@odata.type": "#microsoft.graph.range",
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

#### <a name="range-update"></a><span data-ttu-id="e2688-226">Atualização de intervalo</span><span class="sxs-lookup"><span data-stu-id="e2688-226">Range update</span></span> 

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
  "@odata.type": "#microsoft.graph.range",
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

#### <a name="range-sort"></a><span data-ttu-id="e2688-227">Classificação de intervalo</span><span class="sxs-lookup"><span data-stu-id="e2688-227">Range sort</span></span>
<span data-ttu-id="e2688-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-228">Request</span></span>
<!-- { "blockType": "ignored" } -->
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

<span data-ttu-id="e2688-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-229">Response</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a><span data-ttu-id="e2688-230">Itens nomeados</span><span class="sxs-lookup"><span data-stu-id="e2688-230">Named items</span></span>
<span data-ttu-id="e2688-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-231">Request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /{version}/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

<span data-ttu-id="e2688-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-232">Response</span></span> 

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

### <a name="work-with-nulls"></a><span data-ttu-id="e2688-233">Trabalhar com nulos</span><span class="sxs-lookup"><span data-stu-id="e2688-233">Work with nulls</span></span>

#### <a name="null-input-in-2-d-array"></a><span data-ttu-id="e2688-234">entrada nula em uma matriz 2D</span><span class="sxs-lookup"><span data-stu-id="e2688-234">null input in 2-D array</span></span>

<span data-ttu-id="e2688-p112">A entrada `null` em uma matriz bidimensional (para valores, formato de número ou fórmula) é ignorada nos recursos Range e Table. Nenhuma atualização será realizada no destino pretendido (célula) quando a entrada `null` for enviada em valores, formato de número ou grade de fórmula de valores.</span><span class="sxs-lookup"><span data-stu-id="e2688-p112">`null` input inside a two-dimensional array (for values, number-format, formula) is ignored in the Range and Table resources. No update will take place to the intended target (cell) when `null` input is sent in values or number-format or formula grid of values.</span></span>

<span data-ttu-id="e2688-237">Por exemplo, para atualizar somente partes específicas de Range, como o formato de número de uma célula, e para manter o formato de número existente em outras partes de Range, defina o formato de número onde for obrigatório e envie `null` para as outras células.</span><span class="sxs-lookup"><span data-stu-id="e2688-237">For example, to only update specific parts of the Range, such as a cell's Number Format, and to retain the existing number-format on other parts of the Range, set the Number Format where needed and send `null` for the other cells.</span></span>

<span data-ttu-id="e2688-238">Na solicitação de definição a seguir, somente algumas partes do formato de número de Range são definidas, enquanto o formato de número existente na parte restante é mantido (por meio da transmissão de nulos).</span><span class="sxs-lookup"><span data-stu-id="e2688-238">In the following set request, only some parts of the Range Number Format are set while the existing Number Format on the remaining part is retained (by passing nulls).</span></span>

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a><span data-ttu-id="e2688-239">entrada nula para uma propriedade</span><span class="sxs-lookup"><span data-stu-id="e2688-239">null input for a property</span></span>

<span data-ttu-id="e2688-p113">`null` não é uma entrada válida única para toda a propriedade. Por exemplo, o modelo a seguir não é válido, uma vez que os valores inteiros não podem ser ignorados ou definidos como nulos.</span><span class="sxs-lookup"><span data-stu-id="e2688-p113">`null` is not a valid single input for the entire property. For example, the following is not valid because the entire values cannot be set to null or ignored.</span></span>

```json
{
"values":  null
}

```

<span data-ttu-id="e2688-242">O exemplo a seguir também não é válido, porque nulo não é um valor de cor válido.</span><span class="sxs-lookup"><span data-stu-id="e2688-242">The following is not valid either as null is not a valid color value.</span></span>

```json
{
"color" :  null
}
```

#### <a name="null-response"></a><span data-ttu-id="e2688-243">Resposta nula</span><span class="sxs-lookup"><span data-stu-id="e2688-243">Null-Response</span></span>

<span data-ttu-id="e2688-244">Representação de propriedades de formatação que consiste em valores não uniformes que resultam no retorno de um valor nulo na resposta.</span><span class="sxs-lookup"><span data-stu-id="e2688-244">Representation of formatting properties that consists of non-uniform values results in the return of a null value in the response.</span></span>

<span data-ttu-id="e2688-p114">Por exemplo, um intervalo pode consistir em uma ou mais células. Nos casos em que as células individuais incluídas no intervalo especificado não apresentam valores de formatação uniformes, a representação de nível do intervalo será indefinida.</span><span class="sxs-lookup"><span data-stu-id="e2688-p114">For example, a Range can consist of one or more cells. In cases where the individual cells contained in the Range specified don't have uniform formatting values, the range level representation will be undefined.</span></span>

```json
{
  "size: : null,
  "color" : null
}
```


### <a name="blank-input-and-output"></a><span data-ttu-id="e2688-247">Entrada e saída em branco</span><span class="sxs-lookup"><span data-stu-id="e2688-247">Blank input and output</span></span>

<span data-ttu-id="e2688-p115">Valores em branco em solicitações de atualização são tratados como uma instrução para limpar ou redefinir a respectiva propriedade. Um valor em branco é representado por aspas duplas sem espaço entre elas: `""`</span><span class="sxs-lookup"><span data-stu-id="e2688-p115">Blank values in update requests are treated as an instruction to clear or reset the respective property. A blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

<span data-ttu-id="e2688-250">Exemplos:</span><span class="sxs-lookup"><span data-stu-id="e2688-250">Examples:</span></span>

* <span data-ttu-id="e2688-251">Para `values`, o valor do intervalo é removido. Isso equivale a limpar o conteúdo do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e2688-251">For `values`, the range value is cleared out. This is the same as clearing the contents in the application.</span></span>

* <span data-ttu-id="e2688-252">Para `numberFormat`, o formato de número é definido como `General`.</span><span class="sxs-lookup"><span data-stu-id="e2688-252">For `numberFormat`, the number format is set to `General`.</span></span>

* <span data-ttu-id="e2688-253">Para `formula` e `formulaLocale`, os valores de fórmula são excluídos.</span><span class="sxs-lookup"><span data-stu-id="e2688-253">For `formula` and `formulaLocale`, the formula values are cleared.</span></span>


<span data-ttu-id="e2688-p116">Para operações de leitura, espera-se receber valores em branco caso o conteúdo das células esteja em branco. Quando a célula não inclui dados ou valores, a API retorna um valor em branco. O valor em branco é representado por aspas duplas sem espaço entre elas: `""`</span><span class="sxs-lookup"><span data-stu-id="e2688-p116">For read operations, expect to receive blank values if the contents of the cells are blanks. If the cell contains no data or value, the API returns a blank value. Blank value is represented by two double quotation marks with no space in-between: `""`</span></span>

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


### <a name="unbounded-range"></a><span data-ttu-id="e2688-257">Intervalo não associado</span><span class="sxs-lookup"><span data-stu-id="e2688-257">Unbounded Range</span></span>

#### <a name="read"></a><span data-ttu-id="e2688-258">Leitura</span><span class="sxs-lookup"><span data-stu-id="e2688-258">Read</span></span>

<span data-ttu-id="e2688-259">Um endereço de intervalo não associado contém apenas os identificadores de coluna ou de linha e identificador não especificado de linha ou de coluna, respectivamente, como:</span><span class="sxs-lookup"><span data-stu-id="e2688-259">Unbounded Range address contains only column or row identifiers and unspecified row identifier or column identifiers (respectively), such as:</span></span>

* <span data-ttu-id="e2688-260">`C:C`, `A:F`, `A:XFD` (inclui linhas não especificadas)</span><span class="sxs-lookup"><span data-stu-id="e2688-260">`C:C`, `A:F`, `A:XFD` (contains unspecified rows)</span></span>
* <span data-ttu-id="e2688-261">`2:2`, `1:4`, `1:1048546` (inclui colunas não especificadas)</span><span class="sxs-lookup"><span data-stu-id="e2688-261">`2:2`, `1:4`, `1:1048546` (contains unspecified columns)</span></span>

<span data-ttu-id="e2688-p117">Quando a API faz uma solicitação para recuperar um intervalo não associado (`getRange('C:C')`), a resposta retornada contém `null` para as propriedades em nível de célula, como `values`, `text`, `numberFormat` ou `formula`. Outras propriedades de Range, como `address` ou `cellCount`, refletirão o intervalo não associado.</span><span class="sxs-lookup"><span data-stu-id="e2688-p117">When the API makes a request to retrieve an unbounded Range (`getRange('C:C')`), the response returned contains `null` for cell-level properties such as `values`, `text`, `numberFormat`, or `formula`. Other Range properties such as `address` or `cellCount` will reflect the unbounded range.</span></span>

#### <a name="write"></a><span data-ttu-id="e2688-264">Gravação</span><span class="sxs-lookup"><span data-stu-id="e2688-264">Write</span></span>

<span data-ttu-id="e2688-265">O sistema **não permite** a definição de propriedades de nível da célula (como values, numberFormat, etc.) em um intervalo não associado, pois a solicitação de entrada pode ser muito extensa para ser manipulada.</span><span class="sxs-lookup"><span data-stu-id="e2688-265">Setting cell level properties (such as values, numberFormat, etc.) on unbounded Range is **not allowed** because the input request might be too large to handle.</span></span>

<span data-ttu-id="e2688-266">O exemplo a seguir não é uma solicitação de atualização válida, pois o intervalo solicitado não está associado.</span><span class="sxs-lookup"><span data-stu-id="e2688-266">For example, the following is not a valid update request because the requested range is unbounded.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A:B")

{
  "values" : "Due Date"
}
```

<span data-ttu-id="e2688-267">Quando uma operação de atualização é tentada nesse intervalo, a API retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="e2688-267">When an update operation is attempted on such a Range, the API will return an error.</span></span>


### <a name="large-range"></a><span data-ttu-id="e2688-268">Intervalo longo</span><span class="sxs-lookup"><span data-stu-id="e2688-268">Large Range</span></span>

<span data-ttu-id="e2688-p118">Um intervalo longo significa um intervalo cujo tamanho é muito grande para uma única chamada à API. Muitos fatores, como o número de células, os valores, os formatos de número e as fórmulas incluídas no intervalo, podem fazer com que a resposta seja tão extensa a ponto de se tornar inadequada para interação com a API. A API faz a melhor tentativa para retornar ou gravar os dados solicitados. No entanto, o tamanho extenso envolvido pode resultar em uma condição de erro da API devido à intensa utilização de recursos.</span><span class="sxs-lookup"><span data-stu-id="e2688-p118">Large Range implies a Range of a size that is too large for a single API call. Many factors such as number of cells, values, numberFormat, and formulas contained in the range can make the response so large that it becomes unsuitable for API interaction. The API makes a best attempt to return or write to the requested data. However, the large size involved might result in an API error condition because of the large resource utilization.</span></span>

<span data-ttu-id="e2688-273">Para evitar isso, convém fazer leituras ou gravações para um intervalo longo em vários tamanhos de intervalo menores.</span><span class="sxs-lookup"><span data-stu-id="e2688-273">To avoid this, we recommend that you read or write for large Range in multiple smaller range sizes.</span></span>


### <a name="single-input-copy"></a><span data-ttu-id="e2688-274">Cópia de entrada única</span><span class="sxs-lookup"><span data-stu-id="e2688-274">Single input copy</span></span>

<span data-ttu-id="e2688-p119">Para dar suporte a atualização de um intervalo com os formatos de número ou valores idênticos, ou para a aplicação de uma mesma fórmula em um intervalo, você deve usar a seguinte convenção na API de configuração. No Excel, esse comportamento é semelhante a inserir valores ou fórmulas em um intervalo no modo Ctrl+Enter.</span><span class="sxs-lookup"><span data-stu-id="e2688-p119">To support updating a range with the same values or number-format or applying same formula across a range, the following convention is used in the set API. In Excel, this behavior is similar to inputting values or formulas to a range in the CTRL+Enter mode.</span></span>

<span data-ttu-id="e2688-277">A API vai procurar um *valor de célula única*, no entanto, se a dimensão do intervalo de destino não corresponder à dimensão do intervalo de entrada, ela aplicará a atualização ao intervalo inteiro no modo Ctrl+Enter com o valor ou fórmula fornecida na solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2688-277">The API will look for a *single cell value* and, if the target range dimension doesn't match the input range dimension, it will apply the update to the entire range in the CTRL+Enter model with the value or formula provided in the request.</span></span>

#### <a name="examples"></a><span data-ttu-id="e2688-278">Exemplos</span><span class="sxs-lookup"><span data-stu-id="e2688-278">Examples</span></span>

<span data-ttu-id="e2688-p120">A solicitação a seguir atualiza o intervalo selecionado com "Texto de amostra". Observe que o intervalo tem 200 células, ao passo que a entrada fornecida tem apenas 1 valor de célula.</span><span class="sxs-lookup"><span data-stu-id="e2688-p120">The following request updates the selected range with the text of "Sample text". Note that Range has 200 cells, whereas the provided input only has 1 cell value.</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets('Sheet1')/range(address="A1:B00")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a><span data-ttu-id="e2688-281">Funções de pasta de trabalho</span><span class="sxs-lookup"><span data-stu-id="e2688-281">Workbook functions</span></span> 
<span data-ttu-id="e2688-282">Você pode acessar as funções de pasta de trabalho por meio de uma coleção de funções incluídas no recurso /Functions.</span><span class="sxs-lookup"><span data-stu-id="e2688-282">You can access the workbook functions through a collection of functions included in the /Functions resource.</span></span> 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a><span data-ttu-id="e2688-283">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2688-283">Request</span></span>
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


##### <a name="response"></a><span data-ttu-id="e2688-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2688-284">Response</span></span> 

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

## <a name="error-information"></a><span data-ttu-id="e2688-285">Informações do erro</span><span class="sxs-lookup"><span data-stu-id="e2688-285">Error information</span></span> 

<span data-ttu-id="e2688-p121">Erros são retornados com um código de erro HTTP e um objeto de erro. Um `code` de erro e uma `message` explicam o motivo do erro.</span><span class="sxs-lookup"><span data-stu-id="e2688-p121">Errors are returned with an HTTP error code and an error object. An error `code` and `message` explain the reason for the error.</span></span>
 
<span data-ttu-id="e2688-288">Apresentamos um exemplo a seguir.</span><span class="sxs-lookup"><span data-stu-id="e2688-288">The following is an example.</span></span>

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

