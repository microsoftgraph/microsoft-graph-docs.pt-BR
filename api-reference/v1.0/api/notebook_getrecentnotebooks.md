# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="221c7-101">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="221c7-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="221c7-102">Obtenha uma lista de instâncias [recentNotebook](../resources/recentnotebook.md) que tenham sido acessadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="221c7-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="221c7-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="221c7-103">Permissions</span></span>
<span data-ttu-id="221c7-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="221c7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="221c7-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="221c7-106">Permission type</span></span>      | <span data-ttu-id="221c7-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="221c7-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="221c7-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="221c7-108">Delegated (work or school account)</span></span> | <span data-ttu-id="221c7-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="221c7-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="221c7-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="221c7-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="221c7-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="221c7-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="221c7-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="221c7-112">Application</span></span> | <span data-ttu-id="221c7-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="221c7-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="221c7-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="221c7-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="221c7-115">O `<id | userPrincipalName>` para o usuário deve corresponder ao usuário codificado no token de autorização usado para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="221c7-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="221c7-116">Parâmetros de função</span><span class="sxs-lookup"><span data-stu-id="221c7-116">Function parameters</span></span>

| <span data-ttu-id="221c7-117">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="221c7-117">Parameter</span></span>    | <span data-ttu-id="221c7-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="221c7-118">Type</span></span>   |<span data-ttu-id="221c7-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="221c7-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="221c7-120">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="221c7-120">includePersonalNotebooks</span></span>|<span data-ttu-id="221c7-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="221c7-121">Boolean</span></span>|<span data-ttu-id="221c7-122">Inclua os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="221c7-122">Include notebooks owned by the user.</span></span> <span data-ttu-id="221c7-123">Defina para `true` para incluir os blocos de anotações pertencentes ao usuário; caso contrário, configure para `false`.</span><span class="sxs-lookup"><span data-stu-id="221c7-123">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="221c7-124">Se você não incluir o `includePersonalNotebooks` parâmetro, sua solicitação retornará uma `400` resposta de erro.</span><span class="sxs-lookup"><span data-stu-id="221c7-124">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="221c7-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="221c7-125">Request headers</span></span>
| <span data-ttu-id="221c7-126">Nome</span><span class="sxs-lookup"><span data-stu-id="221c7-126">Name</span></span>       | <span data-ttu-id="221c7-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="221c7-127">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="221c7-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="221c7-128">Authorization</span></span>  | <span data-ttu-id="221c7-129">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="221c7-129">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="221c7-130">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="221c7-130">Request body</span></span>
<span data-ttu-id="221c7-131">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="221c7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="221c7-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="221c7-132">Response</span></span>
<span data-ttu-id="221c7-133">Uma resposta bem-sucedida retorna um `200 OK` que contém uma coleção JSON de **recentNotebooks**.</span><span class="sxs-lookup"><span data-stu-id="221c7-133">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="221c7-134">Exemplo</span><span class="sxs-lookup"><span data-stu-id="221c7-134">Example</span></span>
<span data-ttu-id="221c7-135">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="221c7-135">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="221c7-136">Solicitação</span><span class="sxs-lookup"><span data-stu-id="221c7-136">Request</span></span>
<span data-ttu-id="221c7-137">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="221c7-137">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="221c7-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="221c7-138">Response</span></span>
<span data-ttu-id="221c7-139">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="221c7-139">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.recentNotebook)",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "displayName":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "displayName":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
