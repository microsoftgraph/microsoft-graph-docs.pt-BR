# <a name="workbookrange-rowsabove"></a><span data-ttu-id="3e4ca-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="3e4ca-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="3e4ca-102">Obtém um determinado número de linhas acima de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-102">Gets a certain number of rows above a given range.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3e4ca-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3e4ca-103">Prerequisites</span></span>
<span data-ttu-id="3e4ca-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="3e4ca-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="3e4ca-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3e4ca-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="3e4ca-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4ca-106">Request headers</span></span>
| <span data-ttu-id="3e4ca-107">Nome</span><span class="sxs-lookup"><span data-stu-id="3e4ca-107">Name</span></span>       | <span data-ttu-id="3e4ca-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e4ca-108">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="3e4ca-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="3e4ca-109">Authorization</span></span>  | <span data-ttu-id="3e4ca-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="3e4ca-112">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="3e4ca-112">Workbook-Session-Id</span></span>  | <span data-ttu-id="3e4ca-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="3e4ca-115">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="3e4ca-115">Parameters</span></span>

| <span data-ttu-id="3e4ca-116">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="3e4ca-116">Parameter</span></span>    | <span data-ttu-id="3e4ca-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="3e4ca-117">Type</span></span>   |<span data-ttu-id="3e4ca-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="3e4ca-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e4ca-119">Count</span><span class="sxs-lookup"><span data-stu-id="3e4ca-119">count</span></span>|<span data-ttu-id="3e4ca-120">Int32</span><span class="sxs-lookup"><span data-stu-id="3e4ca-120">Int32</span></span>|<span data-ttu-id="3e4ca-p103">O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="3e4ca-p103">The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-body"></a><span data-ttu-id="3e4ca-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4ca-125">Request body</span></span>

## <a name="response"></a><span data-ttu-id="3e4ca-126">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e4ca-126">Response</span></span>

<span data-ttu-id="3e4ca-127">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-127">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e4ca-128">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3e4ca-128">Example</span></span>
<span data-ttu-id="3e4ca-129">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="3e4ca-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3e4ca-130">Request</span></span>
<span data-ttu-id="3e4ca-131">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_rowsAbove"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="3e4ca-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="3e4ca-132">Response</span></span>
<span data-ttu-id="3e4ca-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3e4ca-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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