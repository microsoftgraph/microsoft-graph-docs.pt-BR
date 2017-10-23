# <a name="workbookrange-resizedrange"></a><span data-ttu-id="a1ce6-101">workbookRange: resizedRange</span><span class="sxs-lookup"><span data-stu-id="a1ce6-101">workbookRange: resizedRange</span></span>
<span data-ttu-id="a1ce6-102">Obtém um objeto range semelhante ao objeto range atual, mas com seu canto inferior direito expandido (ou recolhido) por um determinado número de linhas e colunas.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-102">Gets a range object similar to the current range object, but with its bottom-right corner expanded (or contracted) by some number of rows and columns.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1ce6-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a1ce6-103">Permissions</span></span>
<span data-ttu-id="a1ce6-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a1ce6-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a1ce6-106">Permission type</span></span>      | <span data-ttu-id="a1ce6-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a1ce6-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1ce6-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a1ce6-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a1ce6-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a1ce6-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="a1ce6-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a1ce6-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a1ce6-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-111">Not supported.</span></span>    |
|<span data-ttu-id="a1ce6-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a1ce6-112">Application</span></span> | <span data-ttu-id="a1ce6-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a1ce6-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a1ce6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/resizedRange(deltaRows={n}, deltaColumns={n})

```
## <a name="request-headers"></a><span data-ttu-id="a1ce6-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ce6-115">Request headers</span></span>
| <span data-ttu-id="a1ce6-116">Nome</span><span class="sxs-lookup"><span data-stu-id="a1ce6-116">Name</span></span>       | <span data-ttu-id="a1ce6-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ce6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a1ce6-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="a1ce6-118">Authorization</span></span>  | <span data-ttu-id="a1ce6-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a1ce6-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="a1ce6-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="a1ce6-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="a1ce6-124">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="a1ce6-124">Parameters</span></span>

| <span data-ttu-id="a1ce6-125">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="a1ce6-125">Parameter</span></span>    | <span data-ttu-id="a1ce6-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1ce6-126">Type</span></span>   |<span data-ttu-id="a1ce6-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ce6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1ce6-128">deltaRows</span><span class="sxs-lookup"><span data-stu-id="a1ce6-128">deltarows</span></span>|<span data-ttu-id="a1ce6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ce6-129">Int32</span></span>|<span data-ttu-id="a1ce6-p104">O número de linhas pelo qual expandir o canto inferior direito, referente ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p104">The number of rows by which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it</span></span>|
|<span data-ttu-id="a1ce6-132">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="a1ce6-132">deltaColumns</span></span>|<span data-ttu-id="a1ce6-133">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ce6-133">Int32</span></span>|<span data-ttu-id="a1ce6-p105">O número de colunas pelo qual expandir o canto inferior direito, em relação ao intervalo atual. Use um número positivo para expandir o intervalo ou um número negativo para diminuí-lo.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p105">The number of columnsby which to expand the bottom-right corner, relative to the current range. Use a positive number to expand the range, or a negative number to decrease it.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1ce6-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ce6-136">Request body</span></span>
<span data-ttu-id="a1ce6-137">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-137">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="a1ce6-138">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a1ce6-138">Parameter</span></span>    | <span data-ttu-id="a1ce6-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="a1ce6-139">Type</span></span>   |<span data-ttu-id="a1ce6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="a1ce6-140">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a1ce6-141">deltaRows</span><span class="sxs-lookup"><span data-stu-id="a1ce6-141">deltaRows</span></span>|<span data-ttu-id="a1ce6-142">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ce6-142">Int32</span></span>||
|<span data-ttu-id="a1ce6-143">deltaColumns</span><span class="sxs-lookup"><span data-stu-id="a1ce6-143">deltaColumns</span></span>|<span data-ttu-id="a1ce6-144">Int32</span><span class="sxs-lookup"><span data-stu-id="a1ce6-144">Int32</span></span>||

### <a name="response"></a><span data-ttu-id="a1ce6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1ce6-145">Response</span></span>
<span data-ttu-id="a1ce6-146">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-146">If successful, this method returns `200 OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1ce6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a1ce6-147">Example</span></span>
<span data-ttu-id="a1ce6-148">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-148">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a1ce6-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a1ce6-149">Request</span></span>
<span data-ttu-id="a1ce6-150">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-150">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_resizedrange"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/resizedRange(deltarows={n}, deltaColumns={n})
```

##### <a name="response"></a><span data-ttu-id="a1ce6-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="a1ce6-151">Response</span></span>
<span data-ttu-id="a1ce6-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a1ce6-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
