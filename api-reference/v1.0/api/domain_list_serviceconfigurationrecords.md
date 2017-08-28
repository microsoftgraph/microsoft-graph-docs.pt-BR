# <a name="list-serviceconfigurationrecords"></a><span data-ttu-id="09e20-101">Listar serviceConfigurationRecords</span><span class="sxs-lookup"><span data-stu-id="09e20-101">List serviceConfigurationRecords</span></span>

<span data-ttu-id="09e20-102">Recupera uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md) necessários para ativar os serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="09e20-102">Retrieves a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects needed to enable services for the domain.</span></span>

<span data-ttu-id="09e20-p101">Use a lista retornada para adicionar registros para ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="09e20-p101">Use the returned list to add records to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

## <a name="permissions"></a><span data-ttu-id="09e20-105">Permissões</span><span class="sxs-lookup"><span data-stu-id="09e20-105">Permissions</span></span>

<span data-ttu-id="09e20-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="09e20-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="09e20-108">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="09e20-108">Permission type</span></span>      | <span data-ttu-id="09e20-109">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="09e20-109">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="09e20-110">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="09e20-110">Delegated (work or school account)</span></span> | <span data-ttu-id="09e20-111">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="09e20-111">Directory.Read.All</span></span>    | 
|<span data-ttu-id="09e20-112">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="09e20-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="09e20-113">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="09e20-113">Not supported.</span></span>    | 
|<span data-ttu-id="09e20-114">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="09e20-114">Application</span></span> | <span data-ttu-id="09e20-115">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09e20-115">Directory.Read.All, Domain.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="09e20-116">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="09e20-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/contoso.com/serviceConfigurationRecords
```

## <a name="optional-query-parameters"></a><span data-ttu-id="09e20-117">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="09e20-117">Optional query parameters</span></span>

<span data-ttu-id="09e20-118">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="09e20-118">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="09e20-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="09e20-119">Request headers</span></span>

| <span data-ttu-id="09e20-120">Nome</span><span class="sxs-lookup"><span data-stu-id="09e20-120">Name</span></span>      |<span data-ttu-id="09e20-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="09e20-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="09e20-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="09e20-122">Authorization</span></span>  | <span data-ttu-id="09e20-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="09e20-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="09e20-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="09e20-125">Content-Type</span></span>  | <span data-ttu-id="09e20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09e20-126">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="09e20-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="09e20-127">Request body</span></span>

<span data-ttu-id="09e20-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="09e20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="09e20-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="09e20-129">Response</span></span>

<span data-ttu-id="09e20-130">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="09e20-130">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09e20-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="09e20-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="09e20-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="09e20-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_serviceconfigurationrecords"
}-->
```http
GET https://graph.microsoft.com/V1.0/domains/contoso.com/serviceConfigurationRecords
```
##### <a name="response"></a><span data-ttu-id="09e20-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="09e20-133">Response</span></span>
<span data-ttu-id="09e20-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="09e20-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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