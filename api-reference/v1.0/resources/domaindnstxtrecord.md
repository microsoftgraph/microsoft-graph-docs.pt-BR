# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="28e47-101">Tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="28e47-101">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="28e47-p101">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="28e47-p101">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="28e47-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="28e47-104">Methods</span></span>
<span data-ttu-id="28e47-p102">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="28e47-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="28e47-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="28e47-107">Properties</span></span>
| <span data-ttu-id="28e47-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="28e47-108">Property</span></span>     | <span data-ttu-id="28e47-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="28e47-109">Type</span></span>   |<span data-ttu-id="28e47-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="28e47-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28e47-111">id</span><span class="sxs-lookup"><span data-stu-id="28e47-111">id</span></span>|<span data-ttu-id="28e47-112">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e47-112">String</span></span>| <span data-ttu-id="28e47-p103">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="28e47-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="28e47-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="28e47-115">isOptional</span></span>|<span data-ttu-id="28e47-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="28e47-116">Boolean</span></span>| <span data-ttu-id="28e47-117">Se for falso, o registro TXT deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="28e47-117">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="28e47-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="28e47-118">label</span></span>|<span data-ttu-id="28e47-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e47-119">String</span></span>| <span data-ttu-id="28e47-120">O valor a ser usado ao configurar a propriedade *name* do registro TXT no host DNS.</span><span class="sxs-lookup"><span data-stu-id="28e47-120">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="28e47-121">recordType</span><span class="sxs-lookup"><span data-stu-id="28e47-121">recordType</span></span>|<span data-ttu-id="28e47-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e47-122">String</span></span>| <span data-ttu-id="28e47-p104">Tipo do registro DNS. Este valor sempre será *Txt*. Chave</span><span class="sxs-lookup"><span data-stu-id="28e47-p104">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="28e47-126">supportedService</span><span class="sxs-lookup"><span data-stu-id="28e47-126">supportedService</span></span>|<span data-ttu-id="28e47-127">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e47-127">String</span></span>| <span data-ttu-id="28e47-128">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="28e47-128">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="28e47-129">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="28e47-129">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="28e47-130">text</span><span class="sxs-lookup"><span data-stu-id="28e47-130">text</span></span>|<span data-ttu-id="28e47-131">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="28e47-131">String</span></span>| <span data-ttu-id="28e47-132">O valor usado ao configurar a propriedade *text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="28e47-132">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="28e47-133">ttl</span><span class="sxs-lookup"><span data-stu-id="28e47-133">ttl</span></span>|<span data-ttu-id="28e47-134">Int32</span><span class="sxs-lookup"><span data-stu-id="28e47-134">Int32</span></span>| <span data-ttu-id="28e47-p105">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="28e47-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="28e47-137">Relações</span><span class="sxs-lookup"><span data-stu-id="28e47-137">Relationships</span></span>
<span data-ttu-id="28e47-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="28e47-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="28e47-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="28e47-139">JSON representation</span></span>
<span data-ttu-id="28e47-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="28e47-140">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->