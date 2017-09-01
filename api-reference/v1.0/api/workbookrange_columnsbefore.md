# <a name="workbookrange-columnsbefore"></a><span data-ttu-id="03b37-101">workbookRange: columnsBefore</span><span class="sxs-lookup"><span data-stu-id="03b37-101">workbookRange: columnsBefore</span></span>

<span data-ttu-id="03b37-102">Obtém um determinado número de colunas à esquerda do intervalo especificado.</span><span class="sxs-lookup"><span data-stu-id="03b37-102">Gets a certain number of columns to the left of the given range.</span></span>

## <a name="permissions"></a><span data-ttu-id="03b37-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="03b37-103">Permissions</span></span>
<span data-ttu-id="03b37-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="03b37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="03b37-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="03b37-106">Permission type</span></span>      | <span data-ttu-id="03b37-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="03b37-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03b37-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="03b37-108">Delegated (work or school account)</span></span> | <span data-ttu-id="03b37-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="03b37-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="03b37-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="03b37-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03b37-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03b37-111">Not supported.</span></span>    |
|<span data-ttu-id="03b37-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="03b37-112">Application</span></span> | <span data-ttu-id="03b37-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="03b37-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="03b37-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="03b37-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /me/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=n)

```
## <a name="request-headers"></a><span data-ttu-id="03b37-115">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="03b37-115">Request headers</span></span>
| <span data-ttu-id="03b37-116">Nome</span><span class="sxs-lookup"><span data-stu-id="03b37-116">Name</span></span>       | <span data-ttu-id="03b37-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b37-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="03b37-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="03b37-118">Authorization</span></span>  | <span data-ttu-id="03b37-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="03b37-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03b37-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="03b37-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="03b37-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="03b37-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="parameters"></a><span data-ttu-id="03b37-124">Parâmetros</span><span class="sxs-lookup"><span data-stu-id="03b37-124">Parameters</span></span>

| <span data-ttu-id="03b37-125">Parâmetro	</span><span class="sxs-lookup"><span data-stu-id="03b37-125">Parameter</span></span>    | <span data-ttu-id="03b37-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="03b37-126">Type</span></span>   |<span data-ttu-id="03b37-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="03b37-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="03b37-128">Count</span><span class="sxs-lookup"><span data-stu-id="03b37-128">count</span></span>|<span data-ttu-id="03b37-129">Int32</span><span class="sxs-lookup"><span data-stu-id="03b37-129">Int32</span></span>|<span data-ttu-id="03b37-p104">O número de colunas a serem incluídas no intervalo resultante. Em geral, use um número positivo para criar um intervalo fora do intervalo atual. Você também pode usar um número negativo para criar um intervalo dentro do intervalo atual. O valor padrão é 1.</span><span class="sxs-lookup"><span data-stu-id="03b37-p104">The number of columns to include in the resulting range. In general, use a positive number to create a range outside the current range. You can also use a negative number to create a range within the current range. The default value is 1</span></span>|

## <a name="request-body"></a><span data-ttu-id="03b37-134">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="03b37-134">Request body</span></span>

### <a name="response"></a><span data-ttu-id="03b37-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="03b37-135">Response</span></span>
<span data-ttu-id="03b37-136">Se bem-sucedido, este método retorna um código de resposta `200, OK` e um objeto [workbookRange](../resources/range.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="03b37-136">If successful, this method returns `200, OK` response code and [workbookRange](../resources/range.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03b37-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="03b37-137">Example</span></span>
<span data-ttu-id="03b37-138">Eis um exemplo de como chamar esta API.</span><span class="sxs-lookup"><span data-stu-id="03b37-138">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="03b37-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="03b37-139">Request</span></span>
<span data-ttu-id="03b37-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="03b37-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "workbookrange_columnsbefore"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root/workbook/worksheets/{id}/range/columnsBefore(count=2)
```

##### <a name="response"></a><span data-ttu-id="03b37-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="03b37-141">Response</span></span>
<span data-ttu-id="03b37-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="03b37-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
