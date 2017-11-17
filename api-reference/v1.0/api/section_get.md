# <a name="get-section"></a><span data-ttu-id="71cce-101">Obter seção</span><span class="sxs-lookup"><span data-stu-id="71cce-101">Get section</span></span>

<span data-ttu-id="71cce-102">Recupere as propriedades e os relacionamentos de um objeto [section](../resources/section.md).</span><span class="sxs-lookup"><span data-stu-id="71cce-102">Retrieve the properties and relationships of a [section](../resources/section.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="71cce-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="71cce-103">Permissions</span></span>
<span data-ttu-id="71cce-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="71cce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="71cce-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="71cce-106">Permission type</span></span>      | <span data-ttu-id="71cce-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="71cce-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71cce-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="71cce-108">Delegated (work or school account)</span></span> | <span data-ttu-id="71cce-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71cce-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="71cce-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="71cce-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71cce-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="71cce-111">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span>    |
|<span data-ttu-id="71cce-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="71cce-112">Application</span></span> | <span data-ttu-id="71cce-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71cce-113">Notes.Read, Notes.ReadWrite, Notes.Read.All, or Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="71cce-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="71cce-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/sections/{id}
GET /users/{id | userPrincipalName}/onenote/sections/{id}
GET /groups/{id}/onenote/sections/{id}
GET /sites/{id}/onenote/sections/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="71cce-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="71cce-115">Optional query parameters</span></span>
<span data-ttu-id="71cce-116">Este método dá suporte a `select` e `expand` [Parâmetros de Consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="71cce-116">This method supports the `select` and `expand` [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

<span data-ttu-id="71cce-p102">A consulta padrão expande `parentNotebook` e escolhe suas propriedades `id`, `displayName` e `self`. Os valores `expand` válidos para esse parâmetro são `parentNotebook` e `parentSectionGroup`.</span><span class="sxs-lookup"><span data-stu-id="71cce-p102">The default query expands `parentNotebook` and selects its `id`, `displayName`, and `self` properties. Valid `expand` values for sections are `parentNotebook` and `parentSectionGroup`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="71cce-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="71cce-119">Request headers</span></span>
| <span data-ttu-id="71cce-120">Nome</span><span class="sxs-lookup"><span data-stu-id="71cce-120">Name</span></span>       | <span data-ttu-id="71cce-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="71cce-121">Type</span></span> | <span data-ttu-id="71cce-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="71cce-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="71cce-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="71cce-123">Authorization</span></span>  | <span data-ttu-id="71cce-124">string</span><span class="sxs-lookup"><span data-stu-id="71cce-124">string</span></span>  | <span data-ttu-id="71cce-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="71cce-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="71cce-127">Aceitar</span><span class="sxs-lookup"><span data-stu-id="71cce-127">Accept</span></span> | <span data-ttu-id="71cce-128">string</span><span class="sxs-lookup"><span data-stu-id="71cce-128">string</span></span> | `application/json` |

## <a name="request-body"></a><span data-ttu-id="71cce-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="71cce-129">Request body</span></span>
<span data-ttu-id="71cce-130">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="71cce-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71cce-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cce-131">Response</span></span>

<span data-ttu-id="71cce-132">Se bem-sucedido, este método retorna o código de resposta `200 OK` e um objeto [section](../resources/section.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="71cce-132">If successful, this method returns a `200 OK` response code and a [section](../resources/section.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="71cce-133">Exemplo</span><span class="sxs-lookup"><span data-stu-id="71cce-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71cce-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="71cce-134">Request</span></span>
<span data-ttu-id="71cce-135">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="71cce-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_section"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/sections/{id}
```
##### <a name="response"></a><span data-ttu-id="71cce-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="71cce-136">Response</span></span>
<span data-ttu-id="71cce-p104">Veja a seguir um exemplo da resposta. Observação: O objeto response mostrado aqui está truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="71cce-p104">Here is an example of the response. Note: The response object shown here is truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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