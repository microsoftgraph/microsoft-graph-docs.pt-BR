# <a name="list-sections"></a><span data-ttu-id="f800d-101">Listar seções</span><span class="sxs-lookup"><span data-stu-id="f800d-101">List sections</span></span>

<span data-ttu-id="f800d-102">Recupere uma lista de objetos [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="f800d-102">Retrieve a list of [section](../resources/section.md) objects.</span></span>
## <a name="permissions"></a><span data-ttu-id="f800d-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="f800d-103">Permissions</span></span>
<span data-ttu-id="f800d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="f800d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f800d-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f800d-106">Permission type</span></span>      | <span data-ttu-id="f800d-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f800d-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f800d-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f800d-108">Delegated (work or school account)</span></span> | <span data-ttu-id="f800d-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f800d-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f800d-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f800d-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f800d-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f800d-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="f800d-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f800d-112">Application</span></span> | <span data-ttu-id="f800d-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f800d-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f800d-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f800d-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections
GET /users/{id | userPrincipalName}/onenote/sections
GET /groups/{id}/onenote/sections
GET /sites/{id}/onenote/sections
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f800d-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f800d-115">Optional query parameters</span></span>
<span data-ttu-id="f800d-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="f800d-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="f800d-117">A ordem de classificação padrão é `name asc`.</span><span class="sxs-lookup"><span data-stu-id="f800d-117">The default sort order is `name asc`.</span></span>

<span data-ttu-id="f800d-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="f800d-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f800d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f800d-120">Request headers</span></span>
| <span data-ttu-id="f800d-121">Nome</span><span class="sxs-lookup"><span data-stu-id="f800d-121">Name</span></span>       | <span data-ttu-id="f800d-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="f800d-122">Type</span></span> | <span data-ttu-id="f800d-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="f800d-123">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="f800d-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="f800d-124">Authorization</span></span>  | <span data-ttu-id="f800d-125">string</span><span class="sxs-lookup"><span data-stu-id="f800d-125">string</span></span>  | <span data-ttu-id="f800d-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f800d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f800d-128">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f800d-128">Accept</span></span> | <span data-ttu-id="f800d-129">string</span><span class="sxs-lookup"><span data-stu-id="f800d-129">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="f800d-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f800d-130">Request body</span></span>
<span data-ttu-id="f800d-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f800d-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f800d-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="f800d-132">Response</span></span>

<span data-ttu-id="f800d-133">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f800d-133">If successful, this method returns a `200 OK` response code and collection of [section](../resources/section.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f800d-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f800d-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f800d-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f800d-135">Request</span></span>
<span data-ttu-id="f800d-136">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f800d-136">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_sections"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections
```
##### <a name="response"></a><span data-ttu-id="f800d-137">Resposta</span><span class="sxs-lookup"><span data-stu-id="f800d-137">Response</span></span>
<span data-ttu-id="f800d-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f800d-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.onenoteSection",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 345

{
  "value": [
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
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List sections",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->