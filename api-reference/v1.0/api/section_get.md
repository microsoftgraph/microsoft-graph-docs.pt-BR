# <a name="get-section"></a><span data-ttu-id="1423b-101">Obter seção</span><span class="sxs-lookup"><span data-stu-id="1423b-101">Get section</span></span>

<span data-ttu-id="1423b-102">Recupere as propriedades e relacionamentos de um objeto [onenoteSection](../resources/section.md) .</span><span class="sxs-lookup"><span data-stu-id="1423b-102">Retrieve the properties and relationships of a [onenoteSection](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1423b-103">Permissions</span><span class="sxs-lookup"><span data-stu-id="1423b-103">Permissions</span></span>
<span data-ttu-id="1423b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1423b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1423b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1423b-106">Permission type</span></span>      | <span data-ttu-id="1423b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1423b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1423b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1423b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="1423b-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1423b-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="1423b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1423b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1423b-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="1423b-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span>    |
|<span data-ttu-id="1423b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1423b-112">Application</span></span> | <span data-ttu-id="1423b-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1423b-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1423b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1423b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="1423b-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="1423b-115">Optional query parameters</span></span>
<span data-ttu-id="1423b-116">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1423b-116">This method supports the `select` and `expand` [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="1423b-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="1423b-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="1423b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1423b-119">Request headers</span></span>
| <span data-ttu-id="1423b-120">Nome</span><span class="sxs-lookup"><span data-stu-id="1423b-120">Name</span></span>       | <span data-ttu-id="1423b-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="1423b-121">Type</span></span> | <span data-ttu-id="1423b-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="1423b-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1423b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="1423b-123">Authorization</span></span>  | <span data-ttu-id="1423b-124">string</span><span class="sxs-lookup"><span data-stu-id="1423b-124">string</span></span>  | <span data-ttu-id="1423b-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1423b-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="1423b-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1423b-127">Accept</span></span> | <span data-ttu-id="1423b-128">string</span><span class="sxs-lookup"><span data-stu-id="1423b-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="1423b-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1423b-129">Request body</span></span>
<span data-ttu-id="1423b-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="1423b-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1423b-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="1423b-131">Response</span></span>

<span data-ttu-id="1423b-132">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [onenoteSection](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1423b-132">If successful, this method returns a `200 OK` response code and a [onenoteSection](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="1423b-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1423b-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1423b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1423b-134">Request</span></span>
<span data-ttu-id="1423b-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1423b-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="1423b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="1423b-136">Response</span></span>
<span data-ttu-id="1423b-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1423b-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 272

{
  "isDefault": true,
  "pagesUrl": "pagesUrl-value",
  "displayName": "name-value",
  "createdBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  },
  "lastModifiedBy": {
    "user": {
      "id": "id-value",
      "displayName": "displayName-value"
    }
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get section",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->