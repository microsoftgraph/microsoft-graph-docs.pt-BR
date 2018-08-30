# <a name="workbookrange-rowsbelow"></a><span data-ttu-id="c304e-101">workbookRange: rowsBelow</span><span class="sxs-lookup"><span data-stu-id="c304e-101">workbookRange: rowsBelow</span></span>

<span data-ttu-id="c304e-102">Obtém um determinado número de linhas abaixo de um determinado intervalo.</span><span class="sxs-lookup"><span data-stu-id="c304e-102">Gets certain number of rows below a given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="c304e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="c304e-103">Permissions</span></span>
<span data-ttu-id="c304e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="c304e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="c304e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c304e-106">Permission type</span></span>      | <span data-ttu-id="c304e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="c304e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c304e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c304e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="c304e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="c304e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="c304e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c304e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c304e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c304e-111">Not supported.</span></span>    |
|<span data-ttu-id="c304e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c304e-112">Application</span></span> | <span data-ttu-id="c304e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c304e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c304e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c304e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="c304e-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c304e-115">Request headers</span></span>
| <span data-ttu-id="c304e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="c304e-116">Name</span></span>       | <span data-ttu-id="c304e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="c304e-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c304e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="c304e-118">Authorization</span></span>  | <span data-ttu-id="c304e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c304e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c304e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="c304e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="c304e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="c304e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="c304e-124">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="c304e-124">Parameters</span></span>

| <span data-ttu-id="c304e-125">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="c304e-125">Parameter</span></span>    | <span data-ttu-id="c304e-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="c304e-126">Type</span></span>   |<span data-ttu-id="c304e-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="c304e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c304e-128">Count</span><span class="sxs-lookup"><span data-stu-id="c304e-128">count</span></span>|<span data-ttu-id="c304e-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c304e-129">Int32</span></span>| <span data-ttu-id="c304e-130">Opcional.</span><span class="sxs-lookup"><span data-stu-id="c304e-130">Optional.</span></span> <span data-ttu-id="c304e-131">O número de linhas a serem incluídas no intervalo resultante.</span><span class="sxs-lookup"><span data-stu-id="c304e-131">The number of rows to include in the resulting range.</span></span> <span data-ttu-id="c304e-132">Em geral, use um número positivo para criar um intervalo fora do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="c304e-132">In general, use a positive number to create a range outside the current range.</span></span> <span data-ttu-id="c304e-133">Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual.</span><span class="sxs-lookup"><span data-stu-id="c304e-133">You can also use a negative number to create a range within the current range.</span></span> <span data-ttu-id="c304e-134">O valor padrão é 1</span><span class="sxs-lookup"><span data-stu-id="c304e-134">The default value is 1.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c304e-135">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c304e-135">Request body</span></span>

### <a name="response"></a><span data-ttu-id="c304e-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="c304e-136">Response</span></span>
<span data-ttu-id="c304e-137">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c304e-137">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c304e-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c304e-138">Example</span></span>
<span data-ttu-id="c304e-139">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="c304e-139">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="c304e-140">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c304e-140">Request</span></span>
<span data-ttu-id="c304e-141">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c304e-141">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow",
  "idempotent": true
}-->
```http
POST https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow(count=2)
```

##### <a name="response"></a><span data-ttu-id="c304e-142">Resposta</span><span class="sxs-lookup"><span data-stu-id="c304e-142">Response</span></span>
<span data-ttu-id="c304e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c304e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<span data-ttu-id="c304e-146">Se for chamado sem o `count` parâmetro, essa função tem por padrão uma linha.</span><span class="sxs-lookup"><span data-stu-id="c304e-146">If called without the `count` parameter, this function defaults to one row.</span></span>

##### <a name="request"></a><span data-ttu-id="c304e-147">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c304e-147">Request</span></span>
<span data-ttu-id="c304e-148">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c304e-148">Here is an example of the request.</span></span>
<!--{
  "blockType": "request",
  "isComposable": true,
  "name": "workbookrange_rowsBelow_nocount",
  "idempotent": true
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive/root/workbook/worksheets/{id}/range/rowsBelow
```

##### <a name="response"></a><span data-ttu-id="c304e-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="c304e-149">Response</span></span>
<span data-ttu-id="c304e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c304e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workbookRange"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "address": "address-value",
  "addressLocal": "addressLocal-value",
  "cellCount": 99,
  "columnCount": 99,
  "columnHidden": true,
  "columnIndex": 99
}
```
