# <a name="rangeformat-autofitrows"></a><span data-ttu-id="29bc6-101">RangeFormat: autofitRows</span><span class="sxs-lookup"><span data-stu-id="29bc6-101">RangeFormat: autofitRows</span></span>

<span data-ttu-id="29bc6-102">Altera a altura das linhas do intervalo atual para obter o melhor ajuste, com base nos dados atuais nas colunas.</span><span class="sxs-lookup"><span data-stu-id="29bc6-102">Changes the height of the rows of the current range to achieve the best fit, based on the current data in the columns.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="29bc6-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="29bc6-103">Prerequisites</span></span>
<span data-ttu-id="29bc6-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="29bc6-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="29bc6-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="29bc6-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="29bc6-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="29bc6-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/names(<name>)/range/format/autofitRows
POST /workbook/worksheets/{id|name}/range(<address>)/format/autofitRows
POST /workbook/tables/{id|name}/columns/{id|name}/range/format/autofitRows

```
## <a name="request-headers"></a><span data-ttu-id="29bc6-107">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="29bc6-107">Request headers</span></span>
| <span data-ttu-id="29bc6-108">Nome</span><span class="sxs-lookup"><span data-stu-id="29bc6-108">Name</span></span>       | <span data-ttu-id="29bc6-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="29bc6-109">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="29bc6-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="29bc6-110">Authorization</span></span>  | <span data-ttu-id="29bc6-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="29bc6-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="29bc6-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="29bc6-113">Request body</span></span>

## <a name="response"></a><span data-ttu-id="29bc6-114">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bc6-114">Response</span></span>

<span data-ttu-id="29bc6-p102">Se bem-sucedido, este método retorna um código de resposta `200, OK`. Não retorna nada no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29bc6-p102">If successful, this method returns `200, OK` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="29bc6-117">Exemplo</span><span class="sxs-lookup"><span data-stu-id="29bc6-117">Example</span></span>
<span data-ttu-id="29bc6-118">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="29bc6-118">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="29bc6-119">Solicitação</span><span class="sxs-lookup"><span data-stu-id="29bc6-119">Request</span></span>
<span data-ttu-id="29bc6-120">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="29bc6-120">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "rangeformat_autofitrows"
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/autofitRows
```

##### <a name="response"></a><span data-ttu-id="29bc6-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="29bc6-121">Response</span></span>
<span data-ttu-id="29bc6-122">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="29bc6-122">Here is an example of the response.</span></span> 
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