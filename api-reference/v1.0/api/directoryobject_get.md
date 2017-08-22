# <a name="get-directoryobject"></a><span data-ttu-id="54713-101">Obter directoryObject</span><span class="sxs-lookup"><span data-stu-id="54713-101">Get directoryObject</span></span>

<span data-ttu-id="54713-102">Recupere as propriedades e os relacionamentos do objeto directoryObject.</span><span class="sxs-lookup"><span data-stu-id="54713-102">Retrieve the properties and relationships of directoryObject object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="54713-103">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="54713-103">Prerequisites</span></span>
<span data-ttu-id="54713-104">Um dos seguintes **escopos** é obrigatório para executar esta API:</span><span class="sxs-lookup"><span data-stu-id="54713-104">One of the following **scopes** is required to execute this API:</span></span> 
- <span data-ttu-id="54713-105">_Directory.Read.All_</span><span class="sxs-lookup"><span data-stu-id="54713-105">_Directory.Read.All_</span></span> 
- <span data-ttu-id="54713-106">_Directory.AccessAsUser.All_</span><span class="sxs-lookup"><span data-stu-id="54713-106">_Directory.AccessAsUser.All_</span></span>

> <span data-ttu-id="54713-107">Observação: escopos de permissão são listados em ordem de privilégio menos necessário.</span><span class="sxs-lookup"><span data-stu-id="54713-107">Note: Permission scopes are listed in least privilege required order.</span></span>

## <a name="http-request"></a><span data-ttu-id="54713-108">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="54713-108">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryObjects/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="54713-109">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="54713-109">Optional query parameters</span></span>
<span data-ttu-id="54713-110">Este método dá suporte a [Parâmetros de consulta OData](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="54713-110">This method supports the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="54713-111">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="54713-111">Request headers</span></span>
| <span data-ttu-id="54713-112">Nome</span><span class="sxs-lookup"><span data-stu-id="54713-112">Name</span></span>       | <span data-ttu-id="54713-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="54713-113">Type</span></span> | <span data-ttu-id="54713-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="54713-114">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="54713-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="54713-115">Authorization</span></span>  | <span data-ttu-id="54713-116">string</span><span class="sxs-lookup"><span data-stu-id="54713-116">string</span></span>  | <span data-ttu-id="54713-p101">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="54713-p101">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="54713-119">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="54713-119">Request body</span></span>
<span data-ttu-id="54713-120">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="54713-120">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="54713-121">Resposta</span><span class="sxs-lookup"><span data-stu-id="54713-121">Response</span></span>

<span data-ttu-id="54713-122">Se bem-sucedido, este método retorna um código de resposta `200 OK` e um objeto [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="54713-122">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="54713-123">Exemplo</span><span class="sxs-lookup"><span data-stu-id="54713-123">Example</span></span>
##### <a name="request"></a><span data-ttu-id="54713-124">Solicitação</span><span class="sxs-lookup"><span data-stu-id="54713-124">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directoryobject"
}-->
```http
GET https://graph.microsoft.com/v1.0/directoryObjects/{id}
```
##### <a name="response"></a><span data-ttu-id="54713-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="54713-125">Response</span></span>
<span data-ttu-id="54713-p102">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="54713-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
