# <a name="list-verificationdnsrecords"></a><span data-ttu-id="2dde3-101">Listar verificationDnsRecords</span><span class="sxs-lookup"><span data-stu-id="2dde3-101">List verificationDnsRecords</span></span>

<span data-ttu-id="2dde3-102">Recupere uma lista de objetos [domainDnsRecord](../resources/domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="2dde3-102">Retrieve a list of [domainDnsRecord](../resources/domaindnsrecord.md) objects.</span></span>

<span data-ttu-id="2dde3-p101">Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Para verificar a propriedade do domínio, recupere os registros de verificação de domínio e adicione os detalhes ao arquivo de zona do domínio. Isso pode ser feito por meio da configuração do servidor DNS ou do registrador de domínios.</span><span class="sxs-lookup"><span data-stu-id="2dde3-p101">You cannot use an associated domain with your Azure AD tenant until ownership is verified. To verify the ownership of the domain, retrieve the domain verification records and add the details to the zone file of the domain. This can be done through the domain registrar or DNS server configuration.</span></span>

<span data-ttu-id="2dde3-p102">Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="2dde3-p102">Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="2dde3-110">Permissões</span><span class="sxs-lookup"><span data-stu-id="2dde3-110">Permissions</span></span>

<span data-ttu-id="2dde3-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="2dde3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="2dde3-113">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2dde3-113">Permission type</span></span>      | <span data-ttu-id="2dde3-114">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="2dde3-114">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2dde3-115">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2dde3-115">Delegated (work or school account)</span></span> | <span data-ttu-id="2dde3-116">Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="2dde3-116">Directory.Read.All</span></span>    |
|<span data-ttu-id="2dde3-117">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2dde3-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2dde3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2dde3-118">Not supported.</span></span>    |
|<span data-ttu-id="2dde3-119">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="2dde3-119">Application</span></span> | <span data-ttu-id="2dde3-120">Directory.Read.All, Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2dde3-120">Directory.Read.All, Domain.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2dde3-121">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2dde3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /domains/{id}/verificationDnsRecords
```

> <span data-ttu-id="2dde3-122">Para {id}, especifique o domínio com seu nome de domínio totalmente qualificado.</span><span class="sxs-lookup"><span data-stu-id="2dde3-122">For {id}, specify the domain with its fully qualified domain name.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="2dde3-123">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="2dde3-123">Optional query parameters</span></span>

<span data-ttu-id="2dde3-124">Este método dá suporte a [Parâmetros de consulta OData](http://graph.microsoft.io/docs/overview/query_parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2dde3-124">This method supports the [OData Query Parameters](http://graph.microsoft.io/docs/overview/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2dde3-125">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2dde3-125">Request headers</span></span>

| <span data-ttu-id="2dde3-126">Nome</span><span class="sxs-lookup"><span data-stu-id="2dde3-126">Name</span></span>      |<span data-ttu-id="2dde3-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="2dde3-127">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2dde3-128">Autorização</span><span class="sxs-lookup"><span data-stu-id="2dde3-128">Authorization</span></span>  | <span data-ttu-id="2dde3-p104">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2dde3-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="2dde3-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2dde3-131">Content-Type</span></span>  | <span data-ttu-id="2dde3-132">application/json</span><span class="sxs-lookup"><span data-stu-id="2dde3-132">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="2dde3-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2dde3-133">Request body</span></span>

<span data-ttu-id="2dde3-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2dde3-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2dde3-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dde3-135">Response</span></span>

<span data-ttu-id="2dde3-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [domainDnsRecord](../resources/domaindnsrecord.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="2dde3-136">If successful, this method returns a `200 OK` response code and collection of [domainDnsRecord](../resources/domaindnsrecord.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2dde3-137">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2dde3-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2dde3-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2dde3-138">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_verificationdnsrecords"
}-->
```http
GET https://graph.microsoft.com/v1.0/domains/contoso.com/verificationDnsRecords
```

##### <a name="response"></a><span data-ttu-id="2dde3-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="2dde3-139">Response</span></span>

<span data-ttu-id="2dde3-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2dde3-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List verificationDnsRecords",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->