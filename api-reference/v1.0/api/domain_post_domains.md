# <a name="create-domain"></a><span data-ttu-id="1a044-101">Criar domínio</span><span class="sxs-lookup"><span data-stu-id="1a044-101">Create domain</span></span>

<span data-ttu-id="1a044-102">Adiciona um domínio ao inquilino.</span><span class="sxs-lookup"><span data-stu-id="1a044-102">Adds a domain to the tenant.</span></span>

<span data-ttu-id="1a044-p101">**Importante**: Você não pode usar um domínio associado ao seu locatário do Azure AD até que a propriedade seja verificada. Confira [Listar verificationDnsRecords](domain_list_verificationdnsrecords.md) para obter mais detalhes. Os domínios raiz exigem verificação. Por exemplo, contoso.com exige verificação. Se um domínio raiz for verificado, os subdomínios do domínio raiz serão verificados automaticamente. Por exemplo, o subdominio.contoso.com é automaticamente verificado se contoso.com for verificado.</span><span class="sxs-lookup"><span data-stu-id="1a044-p101">**Important**: You cannot use an associated domain with your Azure AD tenant until ownership is verified. See [List verificationDnsRecords](domain_list_verificationdnsrecords.md) for details. Root domains require verification. For example, contoso.com requires verification. If a root domain is verified, subdomains of the root domain are automatically verified. For example, subdomain.contoso.com is automatically be verified if contoso.com has been verified.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a044-109">Permissões</span><span class="sxs-lookup"><span data-stu-id="1a044-109">Permissions</span></span>

<span data-ttu-id="1a044-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](../../../concepts/permissions_reference.md).</span><span class="sxs-lookup"><span data-stu-id="1a044-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>


|<span data-ttu-id="1a044-112">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1a044-112">Permission type</span></span>      | <span data-ttu-id="1a044-113">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="1a044-113">Permissions (from least to most privileged)</span></span>              | 
|:--------------------|:---------------------------------------------------------| 
|<span data-ttu-id="1a044-114">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1a044-114">Delegated (work or school account)</span></span> | <span data-ttu-id="1a044-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a044-115">Directory.AccessAsUser.All</span></span>    | 
|<span data-ttu-id="1a044-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1a044-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a044-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1a044-117">Not supported.</span></span>    | 
|<span data-ttu-id="1a044-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1a044-118">Application</span></span> | <span data-ttu-id="1a044-119">Domain.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a044-119">Domain.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="1a044-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1a044-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /domains
```
## <a name="request-headers"></a><span data-ttu-id="1a044-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1a044-121">Request headers</span></span>
| <span data-ttu-id="1a044-122">Nome</span><span class="sxs-lookup"><span data-stu-id="1a044-122">Name</span></span>       | <span data-ttu-id="1a044-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="1a044-123">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a044-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="1a044-124">Authorization</span></span>  | <span data-ttu-id="1a044-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1a044-p103">Bearer {token}. Required.</span></span>|
| <span data-ttu-id="1a044-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1a044-127">Content-Type</span></span>  | <span data-ttu-id="1a044-128">application/json</span><span class="sxs-lookup"><span data-stu-id="1a044-128">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a044-129">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1a044-129">Request body</span></span>
<span data-ttu-id="1a044-130">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="1a044-130">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

> <span data-ttu-id="1a044-p104">O corpo da solicitação contém a propriedade id do novo domínio. Id é a única propriedade que pode ser especificada e isso é necessário. O valor da propriedade id é o nome de domínio totalmente qualificado para criar.</span><span class="sxs-lookup"><span data-stu-id="1a044-p104">The request body contains the id property for the new domain. Id is the only property that can be specified and it is required. The id property value is the fully qualified domain name to create.</span></span>

## <a name="response"></a><span data-ttu-id="1a044-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a044-134">Response</span></span>

<span data-ttu-id="1a044-135">Se bem-sucedido, este método retorna o código de resposta `201, Created` e o objeto [domain](../resources/domain.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1a044-135">If successful, this method returns `201, Created` response code and [domain](../resources/domain.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a044-136">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1a044-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a044-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1a044-137">Request</span></span>

<span data-ttu-id="1a044-138">No corpo da solicitação, forneça uma representação JSON do objeto [domain](../resources/domain.md).</span><span class="sxs-lookup"><span data-stu-id="1a044-138">In the request body, supply a JSON representation of [domain](../resources/domain.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="1a044-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="1a044-139">Response</span></span>
<span data-ttu-id="1a044-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1a044-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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