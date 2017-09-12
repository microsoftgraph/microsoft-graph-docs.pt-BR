# <a name="update-icon"></a><span data-ttu-id="86db9-101">Atualizar ícone</span><span class="sxs-lookup"><span data-stu-id="86db9-101">Update icon</span></span>

<span data-ttu-id="86db9-102">Atualize as propriedades do objeto de ícone.</span><span class="sxs-lookup"><span data-stu-id="86db9-102">Update the properties of icon object.</span></span>
## <a name="permissions"></a><span data-ttu-id="86db9-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="86db9-103">Permissions</span></span>
<span data-ttu-id="86db9-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="86db9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="86db9-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86db9-106">Permission type</span></span>      | <span data-ttu-id="86db9-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86db9-107">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="86db9-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86db9-108">Delegated (work or school account)</span></span> | <span data-ttu-id="86db9-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="86db9-109">Files.ReadWrite</span></span>    | 
|<span data-ttu-id="86db9-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86db9-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="86db9-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86db9-111">Not supported.</span></span>    | 
|<span data-ttu-id="86db9-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86db9-112">Application</span></span> | <span data-ttu-id="86db9-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86db9-113">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="86db9-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86db9-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/tables/{id|name}/sort/fields/icon
PATCH /workbook/worksheets/{id|name}/tables/{id|name}/sort/fields/icon
```
## <a name="optional-request-headers"></a><span data-ttu-id="86db9-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="86db9-115">Optional request headers</span></span>
| <span data-ttu-id="86db9-116">Nome</span><span class="sxs-lookup"><span data-stu-id="86db9-116">Name</span></span>       | <span data-ttu-id="86db9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="86db9-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="86db9-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="86db9-118">Authorization</span></span>  | <span data-ttu-id="86db9-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86db9-p102">Bearer {token}. Required.</span></span> |


## <a name="request-body"></a><span data-ttu-id="86db9-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86db9-121">Request body</span></span>
<span data-ttu-id="86db9-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="86db9-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="86db9-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86db9-125">Property</span></span>     | <span data-ttu-id="86db9-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="86db9-126">Type</span></span>   |<span data-ttu-id="86db9-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="86db9-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86db9-128">índice</span><span class="sxs-lookup"><span data-stu-id="86db9-128">index</span></span>|<span data-ttu-id="86db9-129">int</span><span class="sxs-lookup"><span data-stu-id="86db9-129">int</span></span>|<span data-ttu-id="86db9-130">Representa o índice do ícone em determinado conjunto.</span><span class="sxs-lookup"><span data-stu-id="86db9-130">Represents the index of the icon in the given set.</span></span>|
|<span data-ttu-id="86db9-131">set</span><span class="sxs-lookup"><span data-stu-id="86db9-131">set</span></span>|<span data-ttu-id="86db9-132">string</span><span class="sxs-lookup"><span data-stu-id="86db9-132">string</span></span>|<span data-ttu-id="86db9-p104">Representa o conjunto do qual o ícone faz parte. Os valores possíveis são: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles` e `FiveBoxes`.</span><span class="sxs-lookup"><span data-stu-id="86db9-p104">Represents the set that the icon is part of. Possible values are: `Invalid`, `ThreeArrows`, `ThreeArrowsGray`, `ThreeFlags`, `ThreeTrafficLights1`, `ThreeTrafficLights2`, `ThreeSigns`, `ThreeSymbols`, `ThreeSymbols2`, `FourArrows`, `FourArrowsGray`, `FourRedToBlack`, `FourRating`, `FourTrafficLights`, `FiveArrows`, `FiveArrowsGray`, `FiveRating`, `FiveQuarters`, `ThreeStars`, `ThreeTriangles`, `FiveBoxes`.</span></span>|

## <a name="response"></a><span data-ttu-id="86db9-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="86db9-135">Response</span></span>

<span data-ttu-id="86db9-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Icon](../resources/icon.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86db9-136">If successful, this method returns a `200 OK` response code and updated [Icon](../resources/icon.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="86db9-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86db9-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="86db9-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86db9-138">Request</span></span>
<span data-ttu-id="86db9-139">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86db9-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_icon"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/tables/{id|name}/sort/fields/icon
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```
##### <a name="response"></a><span data-ttu-id="86db9-140">Resposta</span><span class="sxs-lookup"><span data-stu-id="86db9-140">Response</span></span>
<span data-ttu-id="86db9-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86db9-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.icon"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 39

{
  "set": "set-value",
  "index": 99
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update icon",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->