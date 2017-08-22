# <a name="worksheetcollection-add"></a><span data-ttu-id="587fc-101">WorksheetCollection: add</span><span class="sxs-lookup"><span data-stu-id="587fc-101">WorksheetCollection: add</span></span>

<span data-ttu-id="587fc-p101">Adiciona uma nova planilha à pasta de trabalho. A planilha será adicionada ao final das planilhas existentes. Se você quiser ativar a planilha recém-adicionada, chame “.activate()” nela.</span><span class="sxs-lookup"><span data-stu-id="587fc-p101">Adds a new worksheet to the workbook. The worksheet will be added at the end of existing worksheets. If you wish to activate the newly added worksheet, call ".activate() on it.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="587fc-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="587fc-105">Prerequisites</span></span>
<span data-ttu-id="587fc-106">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="587fc-106">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="587fc-107">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="587fc-107">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="587fc-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="587fc-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/worksheets/

```
## <a name="request-headers"></a><span data-ttu-id="587fc-109">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="587fc-109">Request headers</span></span>
| <span data-ttu-id="587fc-110">Nome</span><span class="sxs-lookup"><span data-stu-id="587fc-110">Name</span></span>       | <span data-ttu-id="587fc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="587fc-111">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="587fc-112">Autorização</span><span class="sxs-lookup"><span data-stu-id="587fc-112">Authorization</span></span>  | <span data-ttu-id="587fc-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="587fc-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="587fc-115">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="587fc-115">Request body</span></span>
<span data-ttu-id="587fc-116">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="587fc-116">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="587fc-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="587fc-117">Parameter</span></span>    | <span data-ttu-id="587fc-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="587fc-118">Type</span></span>   |<span data-ttu-id="587fc-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="587fc-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="587fc-120">name</span><span class="sxs-lookup"><span data-stu-id="587fc-120">name</span></span>|<span data-ttu-id="587fc-121">string</span><span class="sxs-lookup"><span data-stu-id="587fc-121">string</span></span>|<span data-ttu-id="587fc-p103">Opcional. O nome da planilha a ser adicionada. Se especificado, o nome deve ser exclusivo. Se não especificado, o Excel determina o nome da nova planilha.</span><span class="sxs-lookup"><span data-stu-id="587fc-p103">Optional. The name of the worksheet to be added. If specified, name should be unqiue. If not specified, Excel determines the name of the new worksheet.</span></span>|

## <a name="response"></a><span data-ttu-id="587fc-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="587fc-126">Response</span></span>

<span data-ttu-id="587fc-127">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [Worksheet](../resources/worksheet.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="587fc-127">If successful, this method returns `200, OK` response code and [Worksheet](../resources/worksheet.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="587fc-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="587fc-128">Example</span></span>
<span data-ttu-id="587fc-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="587fc-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="587fc-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="587fc-130">Request</span></span>
<span data-ttu-id="587fc-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="587fc-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "worksheetcollection_add"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/add
Content-type: application/json
Content-length: 26

{
  "name": "name-value"
}
```

##### <a name="response"></a><span data-ttu-id="587fc-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="587fc-132">Response</span></span>
<span data-ttu-id="587fc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="587fc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "WorksheetCollection: add",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->