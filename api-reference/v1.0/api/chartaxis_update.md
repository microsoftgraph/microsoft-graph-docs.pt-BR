# <a name="update-chartaxis"></a><span data-ttu-id="bebe1-101">Atualizar chartaxis</span><span class="sxs-lookup"><span data-stu-id="bebe1-101">Update chartaxis</span></span>

<span data-ttu-id="bebe1-102">Atualiza as propriedades do objeto chartaxis.</span><span class="sxs-lookup"><span data-stu-id="bebe1-102">Update the properties of chartaxis object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bebe1-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="bebe1-103">Prerequisites</span></span>
<span data-ttu-id="bebe1-104">Os seguintes **escopos** são necessários para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="bebe1-104">The following **scopes** are required to execute this API:</span></span> 

    * <span data-ttu-id="bebe1-105">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bebe1-105">Files.ReadWrite</span></span>

## <a name="http-request"></a><span data-ttu-id="bebe1-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="bebe1-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/valueaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/seriesaxis
PATCH /workbook/worksheets/{id|name}/charts(<name>)/axes/categoryaxis
```
## <a name="optional-request-headers"></a><span data-ttu-id="bebe1-107">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="bebe1-107">Optional request headers</span></span>
| <span data-ttu-id="bebe1-108">Nome</span><span class="sxs-lookup"><span data-stu-id="bebe1-108">Name</span></span>       | <span data-ttu-id="bebe1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bebe1-109">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="bebe1-110">Autorização</span><span class="sxs-lookup"><span data-stu-id="bebe1-110">Authorization</span></span>  | <span data-ttu-id="bebe1-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p101">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="bebe1-113">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="bebe1-113">Request body</span></span>
<span data-ttu-id="bebe1-p102">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p102">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bebe1-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bebe1-117">Property</span></span>     | <span data-ttu-id="bebe1-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="bebe1-118">Type</span></span>   |<span data-ttu-id="bebe1-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="bebe1-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bebe1-120">majorUnit</span><span class="sxs-lookup"><span data-stu-id="bebe1-120">majorUnit</span></span>|<span data-ttu-id="bebe1-121">object</span><span class="sxs-lookup"><span data-stu-id="bebe1-121">object</span></span>|<span data-ttu-id="bebe1-p103">Representa o intervalo entre as duas principais marcas de escala. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia.  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p103">Represents the interval between two major tick marks. Can be set to a numeric value or an empty string.  The returned value is always a number.</span></span>|
|<span data-ttu-id="bebe1-125">maximum</span><span class="sxs-lookup"><span data-stu-id="bebe1-125">maximum</span></span>|<span data-ttu-id="bebe1-126">object</span><span class="sxs-lookup"><span data-stu-id="bebe1-126">object</span></span>|<span data-ttu-id="bebe1-p104">Representa o valor máximo no eixo dos valores.  Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p104">Represents the maximum value on the value axis.  Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="bebe1-130">minimum</span><span class="sxs-lookup"><span data-stu-id="bebe1-130">minimum</span></span>|<span data-ttu-id="bebe1-131">object</span><span class="sxs-lookup"><span data-stu-id="bebe1-131">object</span></span>|<span data-ttu-id="bebe1-p105">Representa o valor mínimo no eixo dos valores. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo).  O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p105">Represents the minimum value on the value axis. Can be set to a numeric value or an empty string (for automatic axis values).  The returned value is always a number.</span></span>|
|<span data-ttu-id="bebe1-135">minorUnit</span><span class="sxs-lookup"><span data-stu-id="bebe1-135">minorUnit</span></span>|<span data-ttu-id="bebe1-136">object</span><span class="sxs-lookup"><span data-stu-id="bebe1-136">object</span></span>|<span data-ttu-id="bebe1-p106">Representa o intervalo entre duas marcas de escala secundárias. Pode ser definido como um valor numérico ou uma cadeia de caracteres vazia (para valores automáticos de eixo). O valor retornado sempre é um número.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p106">Represents the interval between two minor tick marks. "Can be set to a numeric value or an empty string (for automatic axis values). The returned value is always a number.</span></span>|

## <a name="response"></a><span data-ttu-id="bebe1-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="bebe1-140">Response</span></span>

<span data-ttu-id="bebe1-141">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [ChartAxis](../resources/chartaxis.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="bebe1-141">If successful, this method returns a `200 OK` response code and updated [ChartAxis](../resources/chartaxis.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="bebe1-142">Exemplo</span><span class="sxs-lookup"><span data-stu-id="bebe1-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bebe1-143">Solicitação</span><span class="sxs-lookup"><span data-stu-id="bebe1-143">Request</span></span>
<span data-ttu-id="bebe1-144">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="bebe1-144">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="bebe1-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="bebe1-145">Response</span></span>
<span data-ttu-id="bebe1-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="bebe1-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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