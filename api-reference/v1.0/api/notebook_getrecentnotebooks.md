# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="a509b-101">notebook: getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="a509b-101">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="a509b-102">Obtenha uma lista de instâncias [recentNotebook](../resources/recentnotebook.md) que tenham sido acessadas pelo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="a509b-102">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="a509b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="a509b-103">Permissions</span></span>
<span data-ttu-id="a509b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="a509b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a509b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a509b-106">Permission type</span></span>      | <span data-ttu-id="a509b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a509b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a509b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a509b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="a509b-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span><span class="sxs-lookup"><span data-stu-id="a509b-109">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All</span></span>|
|<span data-ttu-id="a509b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a509b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a509b-111">Notes.Create, Notes.Read, Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a509b-111">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="a509b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a509b-112">Application</span></span> | <span data-ttu-id="a509b-113">Notes.Read.All, Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a509b-113">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a509b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a509b-114">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="a509b-115">O `<id | userPrincipalName>` para o usuário deve corresponder ao usuário codificado no token de autorização usado para fazer a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a509b-115">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a509b-116">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a509b-116">Request headers</span></span>
| <span data-ttu-id="a509b-117">Nome</span><span class="sxs-lookup"><span data-stu-id="a509b-117">Name</span></span>       | <span data-ttu-id="a509b-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="a509b-118">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a509b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="a509b-119">Authorization</span></span>  | <span data-ttu-id="a509b-120">Portador {código}</span><span class="sxs-lookup"><span data-stu-id="a509b-120">Bearer {code}</span></span>|

## <a name="request-parameters"></a><span data-ttu-id="a509b-121">Solicitar parâmetros</span><span class="sxs-lookup"><span data-stu-id="a509b-121">Request parameters</span></span>
<span data-ttu-id="a509b-122">Forneça os seguintes parâmetros de consulta com valores na URL solicitada.</span><span class="sxs-lookup"><span data-stu-id="a509b-122">In the request URL, provide following query parameters with values.</span></span>

| <span data-ttu-id="a509b-123">Parâmetro</span><span class="sxs-lookup"><span data-stu-id="a509b-123">Parameter</span></span>    | <span data-ttu-id="a509b-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a509b-124">Type</span></span>   |<span data-ttu-id="a509b-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a509b-125">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a509b-126">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="a509b-126">includePersonalNotebooks</span></span>|<span data-ttu-id="a509b-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="a509b-127">Boolean</span></span>|<span data-ttu-id="a509b-128">Inclua os blocos de anotações de propriedade do usuário.</span><span class="sxs-lookup"><span data-stu-id="a509b-128">Include notebooks owned by the user.</span></span> <span data-ttu-id="a509b-129">Defina para `true` para incluir os blocos de anotações pertencentes ao usuário; caso contrário, configure para `false`.</span><span class="sxs-lookup"><span data-stu-id="a509b-129">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="a509b-130">Se você não incluir o parâmetro `includePersonalNotebooks`, sua solicitação retornará uma resposta de erro `400`.</span><span class="sxs-lookup"><span data-stu-id="a509b-130">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a509b-131">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a509b-131">Request body</span></span>
<span data-ttu-id="a509b-132">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="a509b-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a509b-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="a509b-133">Response</span></span>
<span data-ttu-id="a509b-134">Uma resposta bem-sucedida retorna um `200 OK` que contém uma coleção JSON de **recentNotebooks**.</span><span class="sxs-lookup"><span data-stu-id="a509b-134">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="a509b-135">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a509b-135">Example</span></span>
<span data-ttu-id="a509b-136">O exemplo a seguir mostra como chamar essa API.</span><span class="sxs-lookup"><span data-stu-id="a509b-136">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="a509b-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a509b-137">Request</span></span>
<span data-ttu-id="a509b-138">O exemplo a seguir mostra a solicitação.</span><span class="sxs-lookup"><span data-stu-id="a509b-138">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

#### <a name="response"></a><span data-ttu-id="a509b-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="a509b-139">Response</span></span>
<span data-ttu-id="a509b-140">O exemplo a seguir mostra a resposta.</span><span class="sxs-lookup"><span data-stu-id="a509b-140">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
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
