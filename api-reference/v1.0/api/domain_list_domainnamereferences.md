# <a name="list-domainnamereferences"></a><span data-ttu-id="ff51d-101">Listar domainNameReferences</span><span class="sxs-lookup"><span data-stu-id="ff51d-101">List domainNameReferences</span></span>

<span data-ttu-id="ff51d-p101">Recupere uma lista de objetos [directoryObject](../resources/directoryobject.md) com uma referência ao domínio. A lista retornada conterá todos os objetos de diretório que tenham uma dependência no domínio.</span><span class="sxs-lookup"><span data-stu-id="ff51d-p101">Retrieve a list of [directoryObject](../resources/directoryobject.md) with a reference to the domain. The returned list will contain all directory objects that have a dependency on the domain.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff51d-104">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ff51d-104">Prerequisites</span></span>

<span data-ttu-id="ff51d-105">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Domain.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="ff51d-105">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Domain.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="ff51d-106">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ff51d-106">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/domainNameReferences
```

> <span data-ttu-id="ff51d-107">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="ff51d-107">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="ff51d-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="ff51d-108">Optional query parameters</span></span>

<span data-ttu-id="ff51d-109">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="ff51d-109">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff51d-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ff51d-110">Request headers</span></span>

| <span data-ttu-id="ff51d-111">Nome</span><span class="sxs-lookup"><span data-stu-id="ff51d-111">Name</span></span>      |<span data-ttu-id="ff51d-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff51d-112">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="ff51d-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="ff51d-113">Authorization</span></span>  | <span data-ttu-id="ff51d-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ff51d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff51d-116">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ff51d-116">Request body</span></span>

<span data-ttu-id="ff51d-117">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ff51d-117">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff51d-118">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff51d-118">Response</span></span>

<span data-ttu-id="ff51d-119">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ff51d-119">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff51d-120">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ff51d-120">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff51d-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ff51d-121">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_domainnamereferences"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com/domainNameReferences
```

##### <a name="response"></a><span data-ttu-id="ff51d-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="ff51d-122">Response</span></span>
<span data-ttu-id="ff51d-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ff51d-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
        "odata.type": "Microsoft.DirectoryServices.User",
        "objectType": "User",
        "objectId": "567a0db6-289c-43f7-a650-2645c03cbbbb",
        "accountEnabled": true,
        "displayName": "TestUser1",
        "facsimileTelephoneNumber": null,
        "mailNickname": "testuser1",
        "mobile": null,
        "userPrincipalName": "testuser1@contoso.com"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List domainNameReferences",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->