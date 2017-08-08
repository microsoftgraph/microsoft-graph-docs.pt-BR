<span data-ttu-id="25ea0-p101">Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md). Uma Unidade é o contêiner de nível superior para um sistema de arquivos. A API do Graph permite o acesso ao recurso de Unidade do OneDrive ou do OneDrive for Business de um usuário ou a bibliotecas de documentos do SharePoint.</span><span class="sxs-lookup"><span data-stu-id="25ea0-p101">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource. A Drive is the top-level container for a file system. Graph API allows access to the Drive resource for a user's OneDrive or OneDrive for Business, or SharePoint document libraries.</span></span>

Recupere as propriedades e as relações de um recurso [Drive](../resources/drive.md). Uma Unidade é o contêiner de nível superior para um sistema de arquivos. A API do Graph permite o acesso ao recurso de Unidade do OneDrive ou do OneDrive for Business de um usuário ou a bibliotecas de documentos do SharePoint.

## <a name="prerequisites"></a><span data-ttu-id="25ea0-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="25ea0-105">Prerequisites</span></span>

<span data-ttu-id="25ea0-106">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="25ea0-106">One of the following **scopes** is required to execute this API:</span></span>

* <span data-ttu-id="25ea0-107">Files.Read</span><span class="sxs-lookup"><span data-stu-id="25ea0-107">Files.Read</span></span>
* <span data-ttu-id="25ea0-108">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="25ea0-108">Files.ReadWrite</span></span>
* <span data-ttu-id="25ea0-109">Files.Read.All</span><span class="sxs-lookup"><span data-stu-id="25ea0-109">Files.Read.All</span></span>
* <span data-ttu-id="25ea0-110">Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ea0-110">Files.ReadWrite.All</span></span>
* <span data-ttu-id="25ea0-111">Sites.Read.All</span><span class="sxs-lookup"><span data-stu-id="25ea0-111">Sites.Read.All</span></span>
* <span data-ttu-id="25ea0-112">Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25ea0-112">Sites.ReadWrite.All</span></span>

## <a name="get-a-users-onedrive"></a><span data-ttu-id="25ea0-113">Obtenha o OneDrive de um usuário</span><span class="sxs-lookup"><span data-stu-id="25ea0-113">Get a user's OneDrive</span></span>

<span data-ttu-id="25ea0-114">Para acessar o OneDrive ou o OneDrive for Business de um usuário, seu aplicativo deve solicitar a relação **drive** no recurso [User](../resources/user.md).</span><span class="sxs-lookup"><span data-stu-id="25ea0-114">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the [User](../resources/user.md) resource.</span></span>

## <a name="http-request"></a><span data-ttu-id="25ea0-115">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25ea0-115">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /me/drive
GET /users/{idOrUserPrincipalName}/drive
```

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="25ea0-116">Obtenha a biblioteca de documentos associada a um grupo</span><span class="sxs-lookup"><span data-stu-id="25ea0-116">Get the document library associated with a group</span></span>

<span data-ttu-id="25ea0-117">Para acessar uma biblioteca de documentos padrão [de um Grupo](../resources/group.md), o aplicativo solicita a relação **drive** no grupo.</span><span class="sxs-lookup"><span data-stu-id="25ea0-117">To access a [Group's](../resources/group.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

## <a name="http-request"></a><span data-ttu-id="25ea0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="25ea0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{idOrUserPrincipalName}/drive
```


## <a name="optional-query-parameters"></a><span data-ttu-id="25ea0-119">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="25ea0-119">Optional query parameters</span></span>

<span data-ttu-id="25ea0-120">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="25ea0-120">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-body"></a><span data-ttu-id="25ea0-121">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="25ea0-121">Request body</span></span>

<span data-ttu-id="25ea0-122">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="25ea0-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="25ea0-123">Resposta</span><span class="sxs-lookup"><span data-stu-id="25ea0-123">Response</span></span>

<span data-ttu-id="25ea0-124">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o recurso [Drive](../resources/drive.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25ea0-124">If successful, this method returns a `200 OK` response code and [Drive](../resources/drive.md) resource in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25ea0-125">Exemplo</span><span class="sxs-lookup"><span data-stu-id="25ea0-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="25ea0-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="25ea0-126">Request</span></span>

<span data-ttu-id="25ea0-127">Aqui está um exemplo da solicitação para obter o OneDrive ou o OneDrive for Business do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="25ea0-127">Here is an example of the request to get the sign-in user's OneDrive or OneDrive for Business.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_drive"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/drive
```

##### <a name="response"></a><span data-ttu-id="25ea0-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="25ea0-128">Response</span></span>

<span data-ttu-id="25ea0-129">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="25ea0-129">Here is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.drive"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",    
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "OneDrive/Drive/Get Drive"
}-->
