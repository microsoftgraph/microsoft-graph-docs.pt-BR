# <a name="update-worksheet"></a><span data-ttu-id="91235-101">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="91235-101">Update worksheet</span></span>

<span data-ttu-id="91235-102">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="91235-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="91235-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="91235-103">Permissions</span></span>
<span data-ttu-id="91235-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="91235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="91235-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="91235-106">Permission type</span></span>      | <span data-ttu-id="91235-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="91235-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91235-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="91235-108">Delegated (work or school account)</span></span> | <span data-ttu-id="91235-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="91235-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="91235-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="91235-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91235-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91235-111">Not supported.</span></span>    |
|<span data-ttu-id="91235-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="91235-112">Application</span></span> | <span data-ttu-id="91235-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="91235-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="91235-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="91235-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="91235-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="91235-115">Optional request headers</span></span>
| <span data-ttu-id="91235-116">Nome</span><span class="sxs-lookup"><span data-stu-id="91235-116">Name</span></span>       | <span data-ttu-id="91235-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="91235-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="91235-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="91235-118">Authorization</span></span>  | <span data-ttu-id="91235-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="91235-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="91235-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="91235-121">Request body</span></span>
<span data-ttu-id="91235-p103">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="91235-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91235-125">Propriedade</span><span class="sxs-lookup"><span data-stu-id="91235-125">Property</span></span>     | <span data-ttu-id="91235-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="91235-126">Type</span></span>   |<span data-ttu-id="91235-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="91235-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="91235-128">name</span><span class="sxs-lookup"><span data-stu-id="91235-128">name</span></span>|<span data-ttu-id="91235-129">string</span><span class="sxs-lookup"><span data-stu-id="91235-129">string</span></span>|<span data-ttu-id="91235-130">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="91235-130">The display name of the worksheet.</span></span>|
|<span data-ttu-id="91235-131">position</span><span class="sxs-lookup"><span data-stu-id="91235-131">position</span></span>|<span data-ttu-id="91235-132">int</span><span class="sxs-lookup"><span data-stu-id="91235-132">int</span></span>|<span data-ttu-id="91235-133">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="91235-133">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="91235-134">visibilidade</span><span class="sxs-lookup"><span data-stu-id="91235-134">visibility</span></span>|<span data-ttu-id="91235-135">string</span><span class="sxs-lookup"><span data-stu-id="91235-135">string</span></span>|<span data-ttu-id="91235-p104">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="91235-p104">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="91235-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="91235-138">Response</span></span>

<span data-ttu-id="91235-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="91235-139">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="91235-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="91235-140">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91235-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="91235-141">Request</span></span>
<span data-ttu-id="91235-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="91235-142">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_worksheet"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets/{id|name}
Content-type: application/json
Content-length: 100

{
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```
##### <a name="response"></a><span data-ttu-id="91235-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="91235-143">Response</span></span>
<span data-ttu-id="91235-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="91235-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.worksheet"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 100

{
  "id": "id-value",
  "position": 99,
  "name": "name-value",
  "visibility": "visibility-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update worksheet",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->