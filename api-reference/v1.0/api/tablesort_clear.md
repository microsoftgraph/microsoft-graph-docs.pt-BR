# <a name="tablesort-clear"></a><span data-ttu-id="50515-101">TableSort: clear</span><span class="sxs-lookup"><span data-stu-id="50515-101">TableSort: clear</span></span>

<span data-ttu-id="50515-p101">Limpa a classificação que está na tabela. Essa ação não modifica a ordenação da tabela, mas limpa o estado dos botões do cabeçalho.</span><span class="sxs-lookup"><span data-stu-id="50515-p101">Clears the sorting that is currently on the table. While this doesn't modify the table's ordering, it clears the state of the header buttons.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="50515-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="50515-104">Prerequisites</span></span>
<span data-ttu-id="50515-105">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="50515-105">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="50515-106">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="50515-106">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="50515-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="50515-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/tables/{id|name}/sort/clear
POST /workbook/worksheets/{id|name}/tables/{id|name}/sort/clear

```
## <a name="request-headers"></a><span data-ttu-id="50515-108">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="50515-108">Request headers</span></span>
| <span data-ttu-id="50515-109">Nome</span><span class="sxs-lookup"><span data-stu-id="50515-109">Name</span></span>       | <span data-ttu-id="50515-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50515-110">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="50515-111">Autorização</span><span class="sxs-lookup"><span data-stu-id="50515-111">Authorization</span></span>  | <span data-ttu-id="50515-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="50515-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="50515-114">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="50515-114">Request body</span></span>

## <a name="response"></a><span data-ttu-id="50515-115">Resposta</span><span class="sxs-lookup"><span data-stu-id="50515-115">Response</span></span>

<span data-ttu-id="50515-p103">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50515-p103">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50515-118">Exemplo</span><span class="sxs-lookup"><span data-stu-id="50515-118">Example</span></span>
<span data-ttu-id="50515-119">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="50515-119">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="50515-120">Solicitação</span><span class="sxs-lookup"><span data-stu-id="50515-120">Request</span></span>
<span data-ttu-id="50515-121">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="50515-121">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "tablesort_clear"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/clear
```

##### <a name="response"></a><span data-ttu-id="50515-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="50515-122">Response</span></span>
<span data-ttu-id="50515-123">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="50515-123">Here is an example of the response.</span></span> 
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
  "description": "TableSort: clear",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->