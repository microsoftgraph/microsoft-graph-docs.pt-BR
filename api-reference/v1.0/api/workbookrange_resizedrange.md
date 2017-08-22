# <a name="workbookrange-resizedrange"></a><span data-ttu-id="0ba34-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="0ba34-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="0ba34-102">Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.</span><span class="sxs-lookup"><span data-stu-id="0ba34-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0ba34-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ba34-103">Prerequisites</span></span>
<span data-ttu-id="0ba34-104">Os seguintes **escopos** são necessários para executar esta API: _Files.Read, Files.ReadWrite_</span><span class="sxs-lookup"><span data-stu-id="0ba34-104">The following **scopes** are required to execute this API: _Files.Read, Files.ReadWrite_</span></span>
## <a name="http-request"></a><span data-ttu-id="0ba34-105">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ba34-105">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="0ba34-106">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ba34-106">Request headers</span></span>
| <span data-ttu-id="0ba34-107">Nome</span><span class="sxs-lookup"><span data-stu-id="0ba34-107">Name</span></span>       | <span data-ttu-id="0ba34-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba34-108">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="0ba34-109">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ba34-109">Authorization</span></span>  | <span data-ttu-id="0ba34-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ba34-p101">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="0ba34-112">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="0ba34-112">Workbook-Session-Id</span></span>  | <span data-ttu-id="0ba34-p102">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="0ba34-p102">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="0ba34-115">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="0ba34-115">Parameters</span></span>

| <span data-ttu-id="0ba34-116">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="0ba34-116">Parameter</span></span>    | <span data-ttu-id="0ba34-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ba34-117">Type</span></span>   |<span data-ttu-id="0ba34-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba34-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ba34-119">deltaRows</span><span class="sxs-lookup"><span data-stu-id="0ba34-119">deltarows</span></span>|<span data-ttu-id="0ba34-120">Int32</span><span class="sxs-lookup"><span data-stu-id="0ba34-120">Int32</span></span>|<span data-ttu-id="0ba34-p103">O número de linhas pelo qual expandir o canto inferior direito, referente ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo</span><span class="sxs-lookup"><span data-stu-id="0ba34-p103">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="0ba34-123">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="0ba34-123">deltaColumns</span></span>|<span data-ttu-id="0ba34-124">Int32</span><span class="sxs-lookup"><span data-stu-id="0ba34-124">Int32</span></span>|<span data-ttu-id="0ba34-p104">O número de colunas pelo qual expandir o canto inferior direito, em relação ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo.</span><span class="sxs-lookup"><span data-stu-id="0ba34-p104">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ba34-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ba34-127">Request body</span></span>
<span data-ttu-id="0ba34-128">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="0ba34-128">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="0ba34-129">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="0ba34-129">Parameter</span></span>    | <span data-ttu-id="0ba34-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ba34-130">Type</span></span>   |<span data-ttu-id="0ba34-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ba34-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0ba34-132">deltaRows</span><span class="sxs-lookup"><span data-stu-id="0ba34-132">deltaRows</span></span>|<span data-ttu-id="0ba34-133">Int32</span><span class="sxs-lookup"><span data-stu-id="0ba34-133">Int32</span></span>||
|<span data-ttu-id="0ba34-134">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="0ba34-134">deltaColumns</span></span>|<span data-ttu-id="0ba34-135">Int32</span><span class="sxs-lookup"><span data-stu-id="0ba34-135">Int32</span></span>||

## <a name="response"></a><span data-ttu-id="0ba34-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ba34-136">Response</span></span>

<span data-ttu-id="0ba34-137">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ba34-137">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ba34-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ba34-138">Example</span></span>
<span data-ttu-id="0ba34-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="0ba34-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="0ba34-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ba34-140">Request</span></span>
<span data-ttu-id="0ba34-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ba34-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="0ba34-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ba34-142">Response</span></span>
<span data-ttu-id="0ba34-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ba34-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "workbookRange: resizedRange",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
