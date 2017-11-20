# <a name="rangeformat-autofitrows"></a><span data-ttu-id="44c48-101">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="44c48-101">RangeFormat: autofitRows</span></span>

<span data-ttu-id="44c48-102">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="44c48-102">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="permissions"></a><span data-ttu-id="44c48-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="44c48-103">Permissions</span></span>
<span data-ttu-id="44c48-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="44c48-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="44c48-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="44c48-106">Permission type</span></span>      | <span data-ttu-id="44c48-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="44c48-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="44c48-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="44c48-108">Delegated (work or school account)</span></span> | <span data-ttu-id="44c48-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="44c48-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="44c48-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="44c48-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="44c48-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44c48-111">Not supported.</span></span>    |
|<span data-ttu-id="44c48-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="44c48-112">Application</span></span> | <span data-ttu-id="44c48-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="44c48-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="44c48-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="44c48-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(address='<address>')/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="44c48-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="44c48-115">Request headers</span></span>
| <span data-ttu-id="44c48-116">Nome</span><span class="sxs-lookup"><span data-stu-id="44c48-116">Name</span></span>       | <span data-ttu-id="44c48-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="44c48-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="44c48-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="44c48-118">Authorization</span></span>  | <span data-ttu-id="44c48-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="44c48-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="44c48-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="44c48-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="44c48-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="44c48-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="44c48-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="44c48-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="44c48-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="44c48-125">Response</span></span>

<span data-ttu-id="44c48-p104">Se bem-sucedido, este método retorna um código de resposta `200 OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44c48-p104">If successful, this method returns `200 OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="44c48-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="44c48-128">Example</span></span>
<span data-ttu-id="44c48-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="44c48-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="44c48-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="44c48-130">Request</span></span>
<span data-ttu-id="44c48-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="44c48-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="44c48-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="44c48-132">Response</span></span>
<span data-ttu-id="44c48-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="44c48-133">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.none"
} -->
```http
HTTP/1.1 200 OK
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "RangeFormat: autofitRows",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->