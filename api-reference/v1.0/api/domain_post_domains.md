# <a name="create-domain"></a><span data-ttu-id="6993b-101">Criar domínio</span><span class="sxs-lookup"><span data-stu-id="6993b-101">Create domain</span></span>

<span data-ttu-id="6993b-102">Adiciona um domínio ao inquilino.</span><span class="sxs-lookup"><span data-stu-id="6993b-102">Adds a domain to the tenant.</span></span>

<span data-ttu-id="6993b-p101">**Importante**: Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Confira [Listar verificationDnsRecords](domain_list_verificationdnsrecords.md) para obter mais detalhes. Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="6993b-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain_list_verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6993b-109">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6993b-109">Prerequisites</span></span>

<span data-ttu-id="6993b-110">Um dos seguintes **escopos** é obrigatório para executar esta API: *Domain.ReadWrite.All* ou *Directory.AccessAsUser.All*</span><span class="sxs-lookup"><span data-stu-id="6993b-110">One of the following **scopes** is required to execute this API: *Domain.ReadWrite.All* or *Directory.AccessAsUser.All*</span></span>

## <a name="http-request"></a><span data-ttu-id="6993b-111">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6993b-111">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="6993b-112">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6993b-112">Request headers</span></span>
| <span data-ttu-id="6993b-113">Nome</span><span class="sxs-lookup"><span data-stu-id="6993b-113">Name</span></span>       | <span data-ttu-id="6993b-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="6993b-114">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6993b-115">Autorização</span><span class="sxs-lookup"><span data-stu-id="6993b-115">Authorization</span></span>  | <span data-ttu-id="6993b-p102">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6993b-p102">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="6993b-118">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6993b-118">Content-Type</span></span>  | <span data-ttu-id="6993b-119">application/json</span><span class="sxs-lookup"><span data-stu-id="6993b-119">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="6993b-120">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6993b-120">Request body</span></span>
<span data-ttu-id="6993b-121">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="6993b-121">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="6993b-p103">O corpo da solicitação contém a propriedade id do novo domínio. Id é a única propriedade que pode ser especificada e isso é necessário. O valor da propriedade id é o nome de domínio totalmente qualificado para criar.</span><span class="sxs-lookup"><span data-stu-id="6993b-p103">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="6993b-125">Resposta</span><span class="sxs-lookup"><span data-stu-id="6993b-125">Response</span></span>

<span data-ttu-id="6993b-126">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6993b-126">If successful, this method returns `201, Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6993b-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6993b-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6993b-128">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6993b-128">Request</span></span>

<span data-ttu-id="6993b-129">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="6993b-129">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

<!-- {
  "blockType": "request",
  "id": "create_domain_from_domains"
}-->
```http
POST https://graph.microsoft.com/V1.0/domains
Content-type: application/json
Content-length: 192

{
  "id": "contoso.com"
}
```

##### <a name="response"></a><span data-ttu-id="6993b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="6993b-130">Response</span></span>
<span data-ttu-id="6993b-p104">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6993b-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.domain"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 192

{
  "authenticationType": "authenticationType-value",
  "availabilityStatus": "availabilityStatus-value",
  "id": "contoso.com",
  "isAdminManaged": true,
  "isDefault": true,
  "isInitial": true,
  "isRoot": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create domain",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->