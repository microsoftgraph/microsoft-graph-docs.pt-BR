# <a name="get-photo"></a><span data-ttu-id="be63b-101">Obter foto</span><span class="sxs-lookup"><span data-stu-id="be63b-101">Get photo</span></span>

<span data-ttu-id="be63b-102">Recupere as propriedades e os relacionamentos do objeto de foto.</span><span class="sxs-lookup"><span data-stu-id="be63b-102">Retrieve the properties and relationships of photo object.</span></span>
## <a name="permissions"></a><span data-ttu-id="be63b-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="be63b-103">Permissions</span></span>
<span data-ttu-id="be63b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="be63b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="be63b-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="be63b-106">Permission type</span></span>      | <span data-ttu-id="be63b-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="be63b-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="be63b-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="be63b-108">Delegated (work or school account)</span></span> | <span data-ttu-id="be63b-109">Files.Read</span><span class="sxs-lookup"><span data-stu-id="be63b-109">Files.Read</span></span>    |
|<span data-ttu-id="be63b-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="be63b-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="be63b-111">Files.Read</span><span class="sxs-lookup"><span data-stu-id="be63b-111">Files.Read</span></span>    |
|<span data-ttu-id="be63b-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="be63b-112">Application</span></span> | <span data-ttu-id="be63b-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="be63b-113">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="be63b-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="be63b-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/photo
GET /groups/{id}/photo
GET /drive/root/createdByUser/photo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="be63b-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="be63b-115">Optional query parameters</span></span>
<span data-ttu-id="be63b-116">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="be63b-116">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="be63b-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="be63b-117">Request headers</span></span>
| <span data-ttu-id="be63b-118">Nome</span><span class="sxs-lookup"><span data-stu-id="be63b-118">Name</span></span>       | <span data-ttu-id="be63b-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="be63b-119">Type</span></span> | <span data-ttu-id="be63b-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="be63b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="be63b-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="be63b-121">Authorization</span></span>  | <span data-ttu-id="be63b-122">sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="be63b-122">string</span></span>  | <span data-ttu-id="be63b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="be63b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="be63b-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="be63b-125">Request body</span></span>
<span data-ttu-id="be63b-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="be63b-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="be63b-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="be63b-127">Response</span></span>

<span data-ttu-id="be63b-128">Se bem-sucedido, este método retorna o código de resposta `200 OK` e o objeto [photo](../resources/photo.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be63b-128">If successful, this method returns a `200 OK` response code and [photo](../resources/photo.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="be63b-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="be63b-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="be63b-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be63b-130">Request</span></span>
<span data-ttu-id="be63b-131">Veja a seguir um exemplo de solicitação de metadados de fotos.</span><span class="sxs-lookup"><span data-stu-id="be63b-131">Here is an example of the request for photo metadata.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo
```
##### <a name="response"></a><span data-ttu-id="be63b-132">Resposta</span><span class="sxs-lookup"><span data-stu-id="be63b-132">Response</span></span>
<span data-ttu-id="be63b-133">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be63b-133">Here is an example of the response.</span></span>
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.profilePhoto"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 53

{
  "height": 99,
  "width": 99,
  "id": "id-value"
}
```
##### <a name="request"></a><span data-ttu-id="be63b-134">Solicitação</span><span class="sxs-lookup"><span data-stu-id="be63b-134">Request</span></span>
<span data-ttu-id="be63b-135">Veja a seguir um exemplo de solicitação de bytes de fotos.</span><span class="sxs-lookup"><span data-stu-id="be63b-135">Here is an example of the request for the photo bytes.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_photo_value"
}-->
```http
GET https://graph.microsoft.com/v1.0/users/{id|userPrincipalName}/photo/$value
```
##### <a name="response"></a><span data-ttu-id="be63b-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="be63b-136">Response</span></span>
<span data-ttu-id="be63b-137">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="be63b-137">Here is an example of the response.</span></span>

<!-- { "blockType": "response", "@odata.type": "Edm.Stream" } -->

```http
HTTP/1.1 200 OK
Cache-Control: private
Content-Type: image/jpeg
ETag: "A19A6498"
request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
client-request-id: 16e1bff0-6d74-47d6-944c-61707916a74c
x-ms-ags-diagnostic: {"ServerInfo":{"DataCenter":"West US","Slice":"SliceA","Ring":"5","ScaleUnit":"003","Host":"AGSFE_IN_14","ADSiteName":"WST"}}
Access-Control-Allow-Origin: *
Access-Control-Expose-Headers: ETag, Location, Preference-Applied, Content-Range, request-id, client-request-id
Duration: 125.9389
Date: Wed, 13 Dec 2017 22:02:17 GMT
Content-Length: 250526

<binary image data>
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get photo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
