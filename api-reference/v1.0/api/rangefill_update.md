# <a name="update-rangefill"></a><span data-ttu-id="19284-101">Atualizar rangefill</span><span class="sxs-lookup"><span data-stu-id="19284-101">Update rangefill</span></span>

<span data-ttu-id="19284-102">Atualize as propriedades do objeto rangefill.</span><span class="sxs-lookup"><span data-stu-id="19284-102">Update the properties of rangefill object.</span></span>
## <a name="permissions"></a><span data-ttu-id="19284-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="19284-103">Permissions</span></span>
<span data-ttu-id="19284-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="19284-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19284-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="19284-106">Permission type</span></span>      | <span data-ttu-id="19284-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="19284-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19284-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="19284-108">Delegated (work or school account)</span></span> | <span data-ttu-id="19284-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="19284-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="19284-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="19284-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19284-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19284-111">Not supported.</span></span>    |
|<span data-ttu-id="19284-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="19284-112">Application</span></span> | <span data-ttu-id="19284-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="19284-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="19284-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="19284-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/names(<name>)/range/format/fill
PATCH /workbook/worksheets/{id|name}/range(address='<address>')/format/fill
PATCH /workbook/tables/{id|name}/columns/{id|name}/range/format/fill
```
## <a name="optional-request-headers"></a><span data-ttu-id="19284-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="19284-115">Optional request headers</span></span>
| <span data-ttu-id="19284-116">Nome</span><span class="sxs-lookup"><span data-stu-id="19284-116">Name</span></span>       | <span data-ttu-id="19284-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="19284-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="19284-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="19284-118">Authorization</span></span>  | <span data-ttu-id="19284-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="19284-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19284-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="19284-121">Request body</span></span>
<span data-ttu-id="19284-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="19284-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="19284-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="19284-125">Property</span></span>     | <span data-ttu-id="19284-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="19284-126">Type</span></span>   |<span data-ttu-id="19284-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="19284-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="19284-128">color</span><span class="sxs-lookup"><span data-stu-id="19284-128">color</span></span>|<span data-ttu-id="19284-129">string</span><span class="sxs-lookup"><span data-stu-id="19284-129">string</span></span>|<span data-ttu-id="19284-130">Código de cor HTML que representa a cor #RRGGBB da linha de borda do formulário (por exemplo, "FFA500") ou uma cor HTML nomeada (por exemplo, "laranja").</span><span class="sxs-lookup"><span data-stu-id="19284-130">HTML color code representing the color of the border line, of the form #RRGGBB (e.g. "FFA500") or as a named HTML color (e.g. "orange")</span></span>|

## <a name="response"></a><span data-ttu-id="19284-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="19284-131">Response</span></span>

<span data-ttu-id="19284-132">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [RangeFill](../resources/rangefill.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="19284-132">If successful, this method returns a `200 OK` response code and updated [RangeFill](../resources/rangefill.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19284-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="19284-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19284-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="19284-134">Request</span></span>
<span data-ttu-id="19284-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="19284-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_rangefill"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/names(<name>)/range/format/fill
Content-type: application/json
Content-length: 28

{
  "color": "color-value"
}
```
##### <a name="response"></a><span data-ttu-id="19284-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="19284-136">Response</span></span>
<span data-ttu-id="19284-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="19284-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.rangeFill"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 28

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update rangefill",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->