# <a name="workbookrange-columnsafter"></a><span data-ttu-id="20015-101">workbookRange: columnsAfter</span><span class="sxs-lookup"><span data-stu-id="20015-101">workbookRange: columnsAfter</span></span>

<span data-ttu-id="20015-102">Obtém um determinado número de colunas à direita do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="20015-102">Gets a certain number of columns to the right of the given range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20015-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20015-103">Prerequisites</span></span>
<span data-ttu-id="20015-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="20015-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="20015-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20015-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="20015-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20015-106">Request headers</span></span>
| <span data-ttu-id="20015-107">Nome</span><span class="sxs-lookup"><span data-stu-id="20015-107">Name</span></span>       | <span data-ttu-id="20015-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="20015-108">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="20015-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="20015-109">Authorization</span></span>  | <span data-ttu-id="20015-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20015-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="20015-112">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="20015-112">Workbook-Session-Id</span></span>  | <span data-ttu-id="20015-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="20015-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="20015-115">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="20015-115">Parameters</span></span>

| <span data-ttu-id="20015-116">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="20015-116">Parameter</span></span>    | <span data-ttu-id="20015-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="20015-117">Type</span></span>   |<span data-ttu-id="20015-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="20015-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20015-119">Count</span><span class="sxs-lookup"><span data-stu-id="20015-119">count</span></span>|<span data-ttu-id="20015-120">Int32</span><span class="sxs-lookup"><span data-stu-id="20015-120">Int32</span></span>|<span data-ttu-id="20015-p103">O número de colunas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="20015-p103">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|


## <a name="request-body"></a><span data-ttu-id="20015-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20015-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="20015-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="20015-126">Response</span></span>

<span data-ttu-id="20015-127">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20015-127">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20015-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20015-128">Example</span></span>
<span data-ttu-id="20015-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="20015-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="20015-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20015-130">Request</span></span>
<span data-ttu-id="20015-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20015-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsafter"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/columnsAfter(count=2)
```

##### <a name="response"></a><span data-ttu-id="20015-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="20015-132">Response</span></span>
<span data-ttu-id="20015-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20015-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.range"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 157

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
