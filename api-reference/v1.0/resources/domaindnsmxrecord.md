# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="0c343-101">Tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="0c343-101">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="0c343-p101">Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="0c343-p101">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="0c343-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c343-104">Methods</span></span>
<span data-ttu-id="0c343-p102">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="0c343-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0c343-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c343-107">Properties</span></span>
| <span data-ttu-id="0c343-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c343-108">Property</span></span>     | <span data-ttu-id="0c343-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c343-109">Type</span></span>   |<span data-ttu-id="0c343-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c343-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c343-111">id</span><span class="sxs-lookup"><span data-stu-id="0c343-111">id</span></span>|<span data-ttu-id="0c343-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c343-112">String</span></span>| <span data-ttu-id="0c343-p103">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="0c343-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="0c343-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="0c343-115">isOptional</span></span>|<span data-ttu-id="0c343-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c343-116">Boolean</span></span>| <span data-ttu-id="0c343-117">Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="0c343-117">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="0c343-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="0c343-118">label</span></span>|<span data-ttu-id="0c343-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c343-119">String</span></span>| <span data-ttu-id="0c343-120">O valor usado ao configurar a propriedade *alias/host/name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="0c343-120">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="0c343-121">mailExchange</span><span class="sxs-lookup"><span data-stu-id="0c343-121">mailExchange</span></span>|<span data-ttu-id="0c343-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c343-122">String</span></span>| <span data-ttu-id="0c343-123">O valor usado ao configurar a propriedade *answer/destination/value* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="0c343-123">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="0c343-124">preference</span><span class="sxs-lookup"><span data-stu-id="0c343-124">preference</span></span>|<span data-ttu-id="0c343-125">Int32</span><span class="sxs-lookup"><span data-stu-id="0c343-125">Int32</span></span>| <span data-ttu-id="0c343-126">O valor usado ao configurar a propriedade *Preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="0c343-126">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="0c343-127">recordType</span><span class="sxs-lookup"><span data-stu-id="0c343-127">recordType</span></span>|<span data-ttu-id="0c343-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c343-128">String</span></span>| <span data-ttu-id="0c343-p104">Tipo do registro DNS. Este valor sempre será *Mx*. Chave</span><span class="sxs-lookup"><span data-stu-id="0c343-p104">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="0c343-132">supportedService</span><span class="sxs-lookup"><span data-stu-id="0c343-132">supportedService</span></span>|<span data-ttu-id="0c343-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="0c343-133">String</span></span>| <span data-ttu-id="0c343-134">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro MX.</span><span class="sxs-lookup"><span data-stu-id="0c343-134">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="0c343-135">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="0c343-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="0c343-136">ttl</span><span class="sxs-lookup"><span data-stu-id="0c343-136">ttl</span></span>|<span data-ttu-id="0c343-137">Int32</span><span class="sxs-lookup"><span data-stu-id="0c343-137">Int32</span></span>| <span data-ttu-id="0c343-p105">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="0c343-p105">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0c343-140">Relações</span><span class="sxs-lookup"><span data-stu-id="0c343-140">Relationships</span></span>
<span data-ttu-id="0c343-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c343-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0c343-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c343-142">JSON representation</span></span>
<span data-ttu-id="0c343-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c343-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->