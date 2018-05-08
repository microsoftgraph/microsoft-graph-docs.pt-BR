# <a name="update-outlook-category"></a><span data-ttu-id="77f1c-101">Atualizar a categoria do Outlook</span><span class="sxs-lookup"><span data-stu-id="77f1c-101">Update Outlook category</span></span>


<span data-ttu-id="77f1c-102">Atualize a propriedade gravável, **color**, do objeto [outlookCategory](../resources/outlookCategory.md) especificado.</span><span class="sxs-lookup"><span data-stu-id="77f1c-102">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookCategory.md) object.</span></span> <span data-ttu-id="77f1c-103">Não é possível modificar a propriedade **displayName** depois de criar a categoria.</span><span class="sxs-lookup"><span data-stu-id="77f1c-103">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="77f1c-104">Permissões</span><span class="sxs-lookup"><span data-stu-id="77f1c-104">Permissions</span></span>
<span data-ttu-id="77f1c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="77f1c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="77f1c-107">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="77f1c-107">Permission type</span></span>      | <span data-ttu-id="77f1c-108">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="77f1c-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="77f1c-109">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="77f1c-109">Delegated (work or school account)</span></span> | <span data-ttu-id="77f1c-110">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77f1c-110">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="77f1c-111">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="77f1c-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="77f1c-112">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77f1c-112">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="77f1c-113">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="77f1c-113">Application</span></span> | <span data-ttu-id="77f1c-114">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="77f1c-114">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="77f1c-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="77f1c-115">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="77f1c-116">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="77f1c-116">Optional query parameters</span></span>
<span data-ttu-id="77f1c-117">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="77f1c-117">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="77f1c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="77f1c-118">Request headers</span></span>
| <span data-ttu-id="77f1c-119">Nome</span><span class="sxs-lookup"><span data-stu-id="77f1c-119">Name</span></span>      |<span data-ttu-id="77f1c-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f1c-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="77f1c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="77f1c-121">Authorization</span></span>  | <span data-ttu-id="77f1c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="77f1c-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="77f1c-124">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="77f1c-124">Request body</span></span>
<span data-ttu-id="77f1c-p104">No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter melhor desempenho, não inclua valores existentes que não foram alterados.</span><span class="sxs-lookup"><span data-stu-id="77f1c-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="77f1c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="77f1c-128">Property</span></span>     | <span data-ttu-id="77f1c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="77f1c-129">Type</span></span>   |<span data-ttu-id="77f1c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="77f1c-130">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="77f1c-131">color</span><span class="sxs-lookup"><span data-stu-id="77f1c-131">color</span></span>|<span data-ttu-id="77f1c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="77f1c-132">String</span></span>|<span data-ttu-id="77f1c-133">Uma constante de cor predefinida que caracteriza uma categoria e que é mapeada para uma das 25 cores predefinidas.</span><span class="sxs-lookup"><span data-stu-id="77f1c-133">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="77f1c-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f1c-134">Response</span></span>

<span data-ttu-id="77f1c-135">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [outlookCategory](../resources/outlookCategory.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="77f1c-135">If successful, this method returns a `200 OK` response code and updated [contactFolder](../resources/outlookCategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="77f1c-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="77f1c-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="77f1c-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="77f1c-137">Request</span></span>
<span data-ttu-id="77f1c-138">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="77f1c-138">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/me/outlook/masterCategories('bac262b7-485d-4739-b436-e31467d64fac')
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="77f1c-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="77f1c-139">Response</span></span>
<span data-ttu-id="77f1c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="77f1c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->