# <a name="get-directoryobject"></a><span data-ttu-id="6af3e-101">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="6af3e-101">Get directoryObject</span></span>

<span data-ttu-id="6af3e-102">Recupere as propriedades e os relacionamentos do objeto directoryObject.</span><span class="sxs-lookup"><span data-stu-id="6af3e-102">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6af3e-103">Permissões</span><span class="sxs-lookup"><span data-stu-id="6af3e-103">Permissions</span></span>
<span data-ttu-id="6af3e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="6af3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="6af3e-106">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6af3e-106">Permission type</span></span>      | <span data-ttu-id="6af3e-107">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6af3e-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6af3e-108">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6af3e-108">Delegated (work or school account)</span></span> | <span data-ttu-id="6af3e-109">Directory.Read.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6af3e-109">Directory.Read.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6af3e-110">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6af3e-110">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6af3e-111">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6af3e-111">Not supported.</span></span>    |
|<span data-ttu-id="6af3e-112">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6af3e-112">Application</span></span> | <span data-ttu-id="6af3e-113">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="6af3e-113">Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6af3e-114">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6af3e-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6af3e-115">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6af3e-115">Optional query parameters</span></span>
<span data-ttu-id="6af3e-116">Este método dá suporte a [Parâmetros de consulta OData](https://developer.microsoft.com/graph/docs/concepts/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6af3e-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="6af3e-117">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6af3e-117">Request headers</span></span>
| <span data-ttu-id="6af3e-118">Nome</span><span class="sxs-lookup"><span data-stu-id="6af3e-118">Name</span></span>       | <span data-ttu-id="6af3e-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="6af3e-119">Type</span></span> | <span data-ttu-id="6af3e-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="6af3e-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="6af3e-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="6af3e-121">Authorization</span></span>  | <span data-ttu-id="6af3e-122">string</span><span class="sxs-lookup"><span data-stu-id="6af3e-122">string</span></span>  | <span data-ttu-id="6af3e-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6af3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6af3e-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6af3e-125">Request body</span></span>
<span data-ttu-id="6af3e-126">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6af3e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af3e-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af3e-127">Response</span></span>

<span data-ttu-id="6af3e-128">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6af3e-128">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6af3e-129">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6af3e-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6af3e-130">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6af3e-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="6af3e-131">Resposta</span><span class="sxs-lookup"><span data-stu-id="6af3e-131">Response</span></span>
<span data-ttu-id="6af3e-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6af3e-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directoryObject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
