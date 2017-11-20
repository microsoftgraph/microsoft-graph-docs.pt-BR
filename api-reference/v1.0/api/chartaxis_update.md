# <a name="update-chartaxis"></a><span data-ttu-id="d843d-101">Atualizar chartaxis</span><span class="sxs-lookup"><span data-stu-id="d843d-101">Update chartaxis</span></span>

<span data-ttu-id="d843d-102">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="d843d-102">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="d843d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="d843d-103">Permissions</span></span>
<span data-ttu-id="d843d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="d843d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d843d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d843d-106">Permission type</span></span>      | <span data-ttu-id="d843d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="d843d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d843d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d843d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="d843d-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="d843d-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="d843d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d843d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d843d-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d843d-111">Not supported.</span></span>    |
|<span data-ttu-id="d843d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d843d-112">Application</span></span> | <span data-ttu-id="d843d-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d843d-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d843d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d843d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="d843d-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="d843d-115">Optional request headers</span></span>
| <span data-ttu-id="d843d-116">Nome</span><span class="sxs-lookup"><span data-stu-id="d843d-116">Name</span></span>       | <span data-ttu-id="d843d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="d843d-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="d843d-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="d843d-118">Authorization</span></span>  | <span data-ttu-id="d843d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d843d-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d843d-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="d843d-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="d843d-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="d843d-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d843d-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d843d-124">Request body</span></span>
<span data-ttu-id="d843d-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="d843d-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="d843d-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d843d-128">Property</span></span>     | <span data-ttu-id="d843d-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="d843d-129">Type</span></span>   |<span data-ttu-id="d843d-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="d843d-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d843d-131">majorUnit</span><span class="sxs-lookup"><span data-stu-id="d843d-131">majorUnit</span></span>|<span data-ttu-id="d843d-132">objeto</span><span class="sxs-lookup"><span data-stu-id="d843d-132">object</span></span>|<span data-ttu-id="d843d-p105">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="d843d-p105">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="d843d-136">maximum</span><span class="sxs-lookup"><span data-stu-id="d843d-136">maximum</span></span>|<span data-ttu-id="d843d-137">objeto</span><span class="sxs-lookup"><span data-stu-id="d843d-137">object</span></span>|<span data-ttu-id="d843d-p106">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="d843d-p106">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="d843d-141">minimum</span><span class="sxs-lookup"><span data-stu-id="d843d-141">minimum</span></span>|<span data-ttu-id="d843d-142">objeto</span><span class="sxs-lookup"><span data-stu-id="d843d-142">object</span></span>|<span data-ttu-id="d843d-p107">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="d843d-p107">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="d843d-146">minorUnit</span><span class="sxs-lookup"><span data-stu-id="d843d-146">minorUnit</span></span>|<span data-ttu-id="d843d-147">objeto</span><span class="sxs-lookup"><span data-stu-id="d843d-147">object</span></span>|<span data-ttu-id="d843d-p108">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="d843d-p108">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="d843d-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="d843d-151">Response</span></span>

<span data-ttu-id="d843d-152">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxis](../resources/chartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d843d-152">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d843d-153">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d843d-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d843d-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d843d-154">Request</span></span>
<span data-ttu-id="d843d-155">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d843d-155">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_chartaxis"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```
##### <a name="response"></a><span data-ttu-id="d843d-156">Resposta</span><span class="sxs-lookup"><span data-stu-id="d843d-156">Response</span></span>
<span data-ttu-id="d843d-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d843d-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.chartaxis"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 64

{
  "majorUnit": {
  },
  "maximum": {
  },
  "minimum": {
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update chartaxis",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->