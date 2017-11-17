# <a name="update-chartaxis"></a><span data-ttu-id="97277-101">Atualizar chartaxis</span><span class="sxs-lookup"><span data-stu-id="97277-101">Update chartaxis</span></span>

<span data-ttu-id="97277-102">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="97277-102">Update the properties of chartaxis object.</span></span>
## <a name="permissions"></a><span data-ttu-id="97277-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="97277-103">Permissions</span></span>
<span data-ttu-id="97277-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="97277-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97277-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="97277-106">Permission type</span></span>      | <span data-ttu-id="97277-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="97277-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="97277-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="97277-108">Delegated (work or school account)</span></span> | <span data-ttu-id="97277-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="97277-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="97277-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="97277-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="97277-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97277-111">Not supported.</span></span>    |
|<span data-ttu-id="97277-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="97277-112">Application</span></span> | <span data-ttu-id="97277-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="97277-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="97277-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="97277-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="97277-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="97277-115">Optional request headers</span></span>
| <span data-ttu-id="97277-116">Nome</span><span class="sxs-lookup"><span data-stu-id="97277-116">Name</span></span>       | <span data-ttu-id="97277-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="97277-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="97277-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="97277-118">Authorization</span></span>  | <span data-ttu-id="97277-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="97277-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97277-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="97277-121">Request body</span></span>
<span data-ttu-id="97277-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="97277-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="97277-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97277-125">Property</span></span>     | <span data-ttu-id="97277-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="97277-126">Type</span></span>   |<span data-ttu-id="97277-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="97277-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="97277-128">majorUnit</span><span class="sxs-lookup"><span data-stu-id="97277-128">majorUnit</span></span>|<span data-ttu-id="97277-129">object</span><span class="sxs-lookup"><span data-stu-id="97277-129">object</span></span>|<span data-ttu-id="97277-p104">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="97277-p104">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="97277-133">maximum</span><span class="sxs-lookup"><span data-stu-id="97277-133">maximum</span></span>|<span data-ttu-id="97277-134">object</span><span class="sxs-lookup"><span data-stu-id="97277-134">object</span></span>|<span data-ttu-id="97277-p105">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="97277-p105">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="97277-138">minimum</span><span class="sxs-lookup"><span data-stu-id="97277-138">minimum</span></span>|<span data-ttu-id="97277-139">object</span><span class="sxs-lookup"><span data-stu-id="97277-139">object</span></span>|<span data-ttu-id="97277-p106">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="97277-p106">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="97277-143">minorUnit</span><span class="sxs-lookup"><span data-stu-id="97277-143">minorUnit</span></span>|<span data-ttu-id="97277-144">object</span><span class="sxs-lookup"><span data-stu-id="97277-144">object</span></span>|<span data-ttu-id="97277-p107">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="97277-p107">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="97277-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="97277-148">Response</span></span>

<span data-ttu-id="97277-149">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxis](../resources/chartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="97277-149">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="97277-150">Exemplo</span><span class="sxs-lookup"><span data-stu-id="97277-150">Example</span></span>
##### <a name="request"></a><span data-ttu-id="97277-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="97277-151">Request</span></span>
<span data-ttu-id="97277-152">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="97277-152">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="97277-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="97277-153">Response</span></span>
<span data-ttu-id="97277-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="97277-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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