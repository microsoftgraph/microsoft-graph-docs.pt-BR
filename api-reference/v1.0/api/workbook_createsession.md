# <a name="create-session"></a><span data-ttu-id="0151a-101">Criar Sessão</span><span class="sxs-lookup"><span data-stu-id="0151a-101">Create Upload Session</span></span>

<span data-ttu-id="0151a-102">Use essa API para criar uma nova sessão de pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="0151a-102">Use this API to create a new plannerPlan.</span></span> 

<span data-ttu-id="0151a-103">As APIs do Excel podem ser chamadas em um destes dois modos:</span><span class="sxs-lookup"><span data-stu-id="0151a-103">Excel APIs can be called in one of two modes:</span></span> 

1. <span data-ttu-id="0151a-p101">Sessão persistente – Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo normal de operação.</span><span class="sxs-lookup"><span data-stu-id="0151a-p101">Persistent session - All changes made to the workbook are persisted (saved). This is the usual mode of operation.</span></span> 
2. <span data-ttu-id="0151a-p102">Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento.</span><span class="sxs-lookup"><span data-stu-id="0151a-p102">Non-persistent session - Changes made by the API are not saved to the source location. Instead, the Excel backend server keeps a temporary copy of the file that reflects the changes made during that particular API session. When the Excel session expires, the changes are lost. This mode is useful for apps that need to do analysis or obtain the results of a calculation or a chart image, but not affect the document state.</span></span>   

<span data-ttu-id="0151a-110">Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`.</span><span class="sxs-lookup"><span data-stu-id="0151a-110">To represent the session in the API, use the `workbook-session-id: {session-id}` header.</span></span> 

><span data-ttu-id="0151a-p103">**Observação:** O cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.</span><span class="sxs-lookup"><span data-stu-id="0151a-p103">**Note:** The session header is not required for an Excel API to work. However, we recommend that you use the session header to improve performance. If you don't use a session header, changes made during the API call _are_ persisted to the file.</span></span>  

## <a name="permissions"></a><span data-ttu-id="0151a-114">Permissões</span><span class="sxs-lookup"><span data-stu-id="0151a-114">Permissions</span></span>
<span data-ttu-id="0151a-p104">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="0151a-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0151a-117">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0151a-117">Permission type</span></span>      | <span data-ttu-id="0151a-118">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0151a-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0151a-119">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0151a-119">Delegated (work or school account)</span></span> | <span data-ttu-id="0151a-120">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0151a-120">Files.ReadWrite</span></span>    |
|<span data-ttu-id="0151a-121">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0151a-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0151a-122">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0151a-122">Not supported.</span></span>    |
|<span data-ttu-id="0151a-123">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0151a-123">Application</span></span> | <span data-ttu-id="0151a-124">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0151a-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0151a-125">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0151a-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/createSession

```
## <a name="request-headers"></a><span data-ttu-id="0151a-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0151a-126">Request headers</span></span>
| <span data-ttu-id="0151a-127">Nome</span><span class="sxs-lookup"><span data-stu-id="0151a-127">Name</span></span>       | <span data-ttu-id="0151a-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="0151a-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0151a-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="0151a-129">Authorization</span></span>  | <span data-ttu-id="0151a-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0151a-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0151a-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0151a-132">Request body</span></span>
<span data-ttu-id="0151a-133">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="0151a-133">In the request body, supply a JSON representation of [calendar](../resources/workbooksessioninfo.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0151a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="0151a-134">Response</span></span>

<span data-ttu-id="0151a-135">Se for bem-sucedido, esse método retornará o código de resposta `201, Created` e o objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0151a-135">If successful, this method returns `201, Created` response code and the new [page](../resources/workbooksessioninfo.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0151a-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0151a-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0151a-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0151a-137">Request</span></span>
<span data-ttu-id="0151a-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0151a-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_excel_session"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/createSession
Content-type: application/json
Content-length: 52

{
  "persistSession": true
}
```
<span data-ttu-id="0151a-139">No corpo da solicitação, forneça uma representação JSON do objeto [WorkbookSessionInfo](../resources/workbooksessioninfo.md).</span><span class="sxs-lookup"><span data-stu-id="0151a-139">In the request body, supply a JSON representation of [calendar](../resources/workbooksessioninfo.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="0151a-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="0151a-140">Response</span></span>
<span data-ttu-id="0151a-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0151a-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookSessionInfo"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 52

{
  "id": "id-value",
  "persistSession": true
}
```

