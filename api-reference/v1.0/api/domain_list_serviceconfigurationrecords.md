# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="24056-101">Listar serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="24056-101">List serviceConfigurationRecords</span></span>

<span data-ttu-id="24056-102">Recupera uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) necessários para ativar os serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="24056-102">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="24056-p101">Use a lista retornada para adicionar registros para ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="24056-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24056-105">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="24056-105">Prerequisites</span></span>

<span data-ttu-id="24056-106">Um dos seguintes **escopos** é obrigatório para executar esta API: *Directory.Read.All* ou *Domain.ReadWrite.All*</span><span class="sxs-lookup"><span data-stu-id="24056-106">One of the following **scopes** is required to execute this API: *Directory.Read.All* or *Domain.ReadWrite.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="24056-107">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="24056-107">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="24056-108">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="24056-108">Optional query parameters</span></span>

<span data-ttu-id="24056-109">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="24056-109">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="24056-110">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="24056-110">Request headers</span></span>

| <span data-ttu-id="24056-111">Nome</span><span class="sxs-lookup"><span data-stu-id="24056-111">Name</span></span>      |<span data-ttu-id="24056-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="24056-112">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="24056-113">Autorização</span><span class="sxs-lookup"><span data-stu-id="24056-113">Authorization</span></span>  | <span data-ttu-id="24056-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="24056-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="24056-116">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24056-116">Content-Type</span></span>  | <span data-ttu-id="24056-117">application/json</span><span class="sxs-lookup"><span data-stu-id="24056-117">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="24056-118">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="24056-118">Request body</span></span>

<span data-ttu-id="24056-119">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="24056-119">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24056-120">Resposta</span><span class="sxs-lookup"><span data-stu-id="24056-120">Response</span></span>

<span data-ttu-id="24056-121">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="24056-121">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="24056-122">Exemplo</span><span class="sxs-lookup"><span data-stu-id="24056-122">Example</span></span>
##### <a name="request"></a><span data-ttu-id="24056-123">Solicitação</span><span class="sxs-lookup"><span data-stu-id="24056-123">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="24056-124">Resposta</span><span class="sxs-lookup"><span data-stu-id="24056-124">Response</span></span>
<span data-ttu-id="24056-p103">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="24056-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domainDnsRecord",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 220

{
  "value": [
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Mx",
      "supportedService": "Email",
      "ttl": 3600,
      "mailExchange": "contoso-com.mail.protection.outlook.com",
      "preference": 0
    },
    {
      "isOptional": false,
      "label": "contoso.com",
      "recordType": "Txt",
      "supportedServices": "Email",
      "ttl": 3600,
      "text": "v=spf1 include: spf.protection.outlook.com ~all"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List serviceConfigurationRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->