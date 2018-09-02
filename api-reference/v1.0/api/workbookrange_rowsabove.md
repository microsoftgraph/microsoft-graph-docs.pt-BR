# <a name="workbookrange-rowsabove"></a><span data-ttu-id="64f0f-101">workbookRange: rowsAbove</span><span class="sxs-lookup"><span data-stu-id="64f0f-101">workbookRange: rowsAbove</span></span>

<span data-ttu-id="64f0f-102">Obtém um determinado número de linhas acima de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="64f0f-102">Gets a certain number of rows above a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="64f0f-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="64f0f-103">Permissions</span></span>
<span data-ttu-id="64f0f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="64f0f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="64f0f-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="64f0f-106">Permission type</span></span>      | <span data-ttu-id="64f0f-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="64f0f-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="64f0f-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="64f0f-108">Delegated (work or school account)</span></span> | <span data-ttu-id="64f0f-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="64f0f-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="64f0f-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="64f0f-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="64f0f-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64f0f-111">Not supported.</span></span>    |
|<span data-ttu-id="64f0f-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="64f0f-112">Application</span></span> | <span data-ttu-id="64f0f-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="64f0f-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="64f0f-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="64f0f-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=n)

```

## <a name="function-parameters"></a><span data-ttu-id="64f0f-115">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="64f0f-115">Function parameters</span></span>

| <span data-ttu-id="64f0f-116">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="64f0f-116">Parameter</span></span>    | <span data-ttu-id="64f0f-117">Tipo</span><span class="sxs-lookup"><span data-stu-id="64f0f-117">Type</span></span>   |<span data-ttu-id="64f0f-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f0f-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64f0f-119">Count</span><span class="sxs-lookup"><span data-stu-id="64f0f-119">count</span></span>|<span data-ttu-id="64f0f-120">Int32</span><span class="sxs-lookup"><span data-stu-id="64f0f-120">Int32</span></span>|<span data-ttu-id="64f0f-p102">Opcional. O número de linhas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="64f0f-p102">Optional. The number of rows to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="64f0f-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="64f0f-126">Request headers</span></span>
| <span data-ttu-id="64f0f-127">Nome</span><span class="sxs-lookup"><span data-stu-id="64f0f-127">Name</span></span>       | <span data-ttu-id="64f0f-128">Descrição</span><span class="sxs-lookup"><span data-stu-id="64f0f-128">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="64f0f-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="64f0f-129">Authorization</span></span>  | <span data-ttu-id="64f0f-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="64f0f-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="64f0f-132">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="64f0f-132">Workbook-Session-Id</span></span>  | <span data-ttu-id="64f0f-p104">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="64f0f-p104">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="64f0f-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="64f0f-135">Request body</span></span>
<span data-ttu-id="64f0f-136">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="64f0f-136">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="64f0f-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f0f-137">Response</span></span>
<span data-ttu-id="64f0f-138">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="64f0f-138">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="64f0f-139">Exemplo</span><span class="sxs-lookup"><span data-stu-id="64f0f-139">Example</span></span>
<span data-ttu-id="64f0f-140">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="64f0f-140">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="64f0f-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64f0f-141">Request</span></span>
<span data-ttu-id="64f0f-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="64f0f-142">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove(count=2)
```

##### <a name="response"></a><span data-ttu-id="64f0f-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f0f-143">Response</span></span>
<span data-ttu-id="64f0f-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="64f0f-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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

<span data-ttu-id="64f0f-147">Se chamada sem o `count`  parâmetro opcional, essa função retorna a única linha acima do intervalo.</span><span class="sxs-lookup"><span data-stu-id="64f0f-147">If called without the optional `count` parameter, this function returns the single row above the range.</span></span>

##### <a name="request"></a><span data-ttu-id="64f0f-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="64f0f-148">Request</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsAbove_nocount",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsAbove
```

##### <a name="response"></a><span data-ttu-id="64f0f-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="64f0f-149">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
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