# <a name="update-worksheet"></a><span data-ttu-id="2849e-101">Atualizar planilha</span><span class="sxs-lookup"><span data-stu-id="2849e-101">Update worksheet</span></span>

<span data-ttu-id="2849e-102">Atualize as propriedades do objeto de planilha.</span><span class="sxs-lookup"><span data-stu-id="2849e-102">Update the properties of worksheet object.</span></span>
## <a name="permissions"></a><span data-ttu-id="2849e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="2849e-103">Permissions</span></span>
<span data-ttu-id="2849e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2849e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2849e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2849e-106">Permission type</span></span>      | <span data-ttu-id="2849e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2849e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2849e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2849e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="2849e-109">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="2849e-109">Files.ReadWrite</span></span>    |
|<span data-ttu-id="2849e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2849e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2849e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2849e-111">Not supported.</span></span>    |
|<span data-ttu-id="2849e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2849e-112">Application</span></span> | <span data-ttu-id="2849e-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2849e-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2849e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2849e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /workbook/worksheets/{id|name}
```
## <a name="optional-request-headers"></a><span data-ttu-id="2849e-115">Cabeçalhos de solicitação opcionais</span><span class="sxs-lookup"><span data-stu-id="2849e-115">Optional request headers</span></span>
| <span data-ttu-id="2849e-116">Nome</span><span class="sxs-lookup"><span data-stu-id="2849e-116">Name</span></span>       | <span data-ttu-id="2849e-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="2849e-117">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="2849e-118">Autorização</span><span class="sxs-lookup"><span data-stu-id="2849e-118">Authorization</span></span>  | <span data-ttu-id="2849e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2849e-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2849e-121">Workbook-Session-Id</span><span class="sxs-lookup"><span data-stu-id="2849e-121">Workbook-Session-Id</span></span>  | <span data-ttu-id="2849e-p103">ID de sessão de pasta de trabalho que determina se as alterações são persistentes ou não. Opcional.</span><span class="sxs-lookup"><span data-stu-id="2849e-p103">Workbook session Id that determines if changes are persisted or not. Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2849e-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2849e-124">Request body</span></span>
<span data-ttu-id="2849e-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="2849e-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="2849e-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2849e-128">Property</span></span>     | <span data-ttu-id="2849e-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="2849e-129">Type</span></span>   |<span data-ttu-id="2849e-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="2849e-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2849e-131">name</span><span class="sxs-lookup"><span data-stu-id="2849e-131">name</span></span>|<span data-ttu-id="2849e-132">string</span><span class="sxs-lookup"><span data-stu-id="2849e-132">string</span></span>|<span data-ttu-id="2849e-133">O nome de exibição da planilha.</span><span class="sxs-lookup"><span data-stu-id="2849e-133">The display name of the worksheet.</span></span>|
|<span data-ttu-id="2849e-134">position</span><span class="sxs-lookup"><span data-stu-id="2849e-134">position</span></span>|<span data-ttu-id="2849e-135">int</span><span class="sxs-lookup"><span data-stu-id="2849e-135">int</span></span>|<span data-ttu-id="2849e-136">A posição baseada em zero da planilha na pasta de trabalho.</span><span class="sxs-lookup"><span data-stu-id="2849e-136">The zero-based position of the worksheet within the workbook.</span></span>|
|<span data-ttu-id="2849e-137">visibilidade</span><span class="sxs-lookup"><span data-stu-id="2849e-137">visibility</span></span>|<span data-ttu-id="2849e-138">string</span><span class="sxs-lookup"><span data-stu-id="2849e-138">string</span></span>|<span data-ttu-id="2849e-p105">A visibilidade da planilha. Os valores possíveis são: `Visible`, `Hidden` e `VeryHidden`.</span><span class="sxs-lookup"><span data-stu-id="2849e-p105">The Visibility of the worksheet. Possible values are: `Visible`, `Hidden`, `VeryHidden`.</span></span>|

## <a name="response"></a><span data-ttu-id="2849e-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="2849e-141">Response</span></span>

<span data-ttu-id="2849e-142">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [Worksheet](../resources/worksheet.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2849e-142">If successful, this method returns a `200 OK` response code and updated [Worksheet](../resources/worksheet.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="2849e-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2849e-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2849e-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2849e-144">Request</span></span>
<span data-ttu-id="2849e-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2849e-145">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="2849e-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="2849e-146">Response</span></span>
<span data-ttu-id="2849e-p106">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2849e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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