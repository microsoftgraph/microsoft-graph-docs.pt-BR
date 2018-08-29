# <a name="range-merge"></a><span data-ttu-id="2c7ca-101">Range: merge</span><span class="sxs-lookup"><span data-stu-id="2c7ca-101">Range: merge</span></span>

<span data-ttu-id="2c7ca-102">Mescla as células do intervalo em uma região da planilha.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-102">Merge the range cells into one region in the worksheet.</span></span>
## <a name="permissions"></a><span data-ttu-id="2c7ca-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2c7ca-103">Permissions</span></span>
<span data-ttu-id="2c7ca-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2c7ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2c7ca-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2c7ca-106">Permission type</span></span>      | <span data-ttu-id="2c7ca-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2c7ca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c7ca-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2c7ca-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2c7ca-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2c7ca-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2c7ca-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2c7ca-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c7ca-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-111">Not supported.</span></span>    |
|<span data-ttu-id="2c7ca-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2c7ca-112">Application</span></span> | <span data-ttu-id="2c7ca-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2c7ca-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2c7ca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names/{name}/range/merge
POST /workbook/worksheets/{id|name}/range(address='<address>')/merge
POST /workbook/tables/{id|name}/columns/{id|name}/range/merge

```
## <a name="request-headers"></a><span data-ttu-id="2c7ca-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2c7ca-115">Request headers</span></span>
| <span data-ttu-id="2c7ca-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2c7ca-116">Name</span></span>       | <span data-ttu-id="2c7ca-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c7ca-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="2c7ca-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2c7ca-118">Authorization</span></span>  | <span data-ttu-id="2c7ca-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2c7ca-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2c7ca-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2c7ca-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c7ca-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2c7ca-124">Request body</span></span>
<span data-ttu-id="2c7ca-125">Forneça um objeto JSON com os seguintes parâmetros no corpo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-125">In the request body, provide a JSON object with the following parameters.</span></span>

| <span data-ttu-id="2c7ca-126">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="2c7ca-126">Parameter</span></span>    | <span data-ttu-id="2c7ca-127">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c7ca-127">Type</span></span>   |<span data-ttu-id="2c7ca-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c7ca-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2c7ca-129">across</span><span class="sxs-lookup"><span data-stu-id="2c7ca-129">across</span></span>|<span data-ttu-id="2c7ca-130">booliano</span><span class="sxs-lookup"><span data-stu-id="2c7ca-130">boolean</span></span>|<span data-ttu-id="2c7ca-p104">Opcional. Defina true para mesclar células em todas as linhas do intervalo especificado como células mescladas separadamente. O valor padrão é false.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-p104">Optional. Set true to merge cells in each row of the specified range as separate merged cells. The default value is false.</span></span>|

## <a name="response"></a><span data-ttu-id="2c7ca-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c7ca-134">Response</span></span>

<span data-ttu-id="2c7ca-p105">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-p105">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2c7ca-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2c7ca-137">Example</span></span>
<span data-ttu-id="2c7ca-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="2c7ca-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2c7ca-139">Request</span></span>
<span data-ttu-id="2c7ca-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "range_merge"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names/{name}/range/merge
Content-type: application/json
Content-length: 20

{
  "across": true
}
```

##### <a name="response"></a><span data-ttu-id="2c7ca-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2c7ca-141">Response</span></span>
<span data-ttu-id="2c7ca-142">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2c7ca-142">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Range: merge",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->