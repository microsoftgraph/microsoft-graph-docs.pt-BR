# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="835db-101">Tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="835db-101">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="835db-p101">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="835db-p101">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="835db-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="835db-104">Methods</span></span>
<span data-ttu-id="835db-p102">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="835db-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="835db-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="835db-107">Properties</span></span>
| <span data-ttu-id="835db-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="835db-108">Property</span></span>     | <span data-ttu-id="835db-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="835db-109">Type</span></span>   |<span data-ttu-id="835db-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="835db-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="835db-111">id</span><span class="sxs-lookup"><span data-stu-id="835db-111">id</span></span>|<span data-ttu-id="835db-112">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-112">String</span></span>| <span data-ttu-id="835db-p103">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="835db-p103">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="835db-115">isOptional</span><span class="sxs-lookup"><span data-stu-id="835db-115">isOptional</span></span>|<span data-ttu-id="835db-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="835db-116">Boolean</span></span>| <span data-ttu-id="835db-117">Se for falso, o registro SRV deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="835db-117">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="835db-118">rótulo</span><span class="sxs-lookup"><span data-stu-id="835db-118">label</span></span>|<span data-ttu-id="835db-119">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-119">String</span></span>| <span data-ttu-id="835db-120">O valor usado ao configurar a propriedade *name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-120">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="835db-121">nameTarget</span><span class="sxs-lookup"><span data-stu-id="835db-121">nameTarget</span></span>|<span data-ttu-id="835db-122">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-122">String</span></span>| <span data-ttu-id="835db-123">O valor a ser usado ao configurar a propriedade *Target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-123">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="835db-124">porta</span><span class="sxs-lookup"><span data-stu-id="835db-124">port</span></span>|<span data-ttu-id="835db-125">Int32</span><span class="sxs-lookup"><span data-stu-id="835db-125">Int32</span></span>| <span data-ttu-id="835db-126">O valor a ser usado ao configurar a propriedade *port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-126">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="835db-127">prioridade</span><span class="sxs-lookup"><span data-stu-id="835db-127">priority</span></span>|<span data-ttu-id="835db-128">Int32</span><span class="sxs-lookup"><span data-stu-id="835db-128">Int32</span></span>| <span data-ttu-id="835db-129">O valor a ser usado ao configurar a propriedade *priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-129">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="835db-130">protocolo</span><span class="sxs-lookup"><span data-stu-id="835db-130">protocol</span></span>|<span data-ttu-id="835db-131">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-131">String</span></span>| <span data-ttu-id="835db-132">O valor a ser usado ao configurar a propriedade *protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-132">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="835db-133">recordType</span><span class="sxs-lookup"><span data-stu-id="835db-133">recordType</span></span>|<span data-ttu-id="835db-134">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-134">String</span></span>|  <span data-ttu-id="835db-p104">Tipo do registro DNS. Este valor sempre será *Srv*. Chave</span><span class="sxs-lookup"><span data-stu-id="835db-p104">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="835db-138">service</span><span class="sxs-lookup"><span data-stu-id="835db-138">service</span></span>|<span data-ttu-id="835db-139">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-139">String</span></span>| <span data-ttu-id="835db-140">O valor a ser usado ao configurar a propriedade *service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-140">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="835db-141">supportedService</span><span class="sxs-lookup"><span data-stu-id="835db-141">supportedService</span></span>|<span data-ttu-id="835db-142">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="835db-142">String</span></span>| <span data-ttu-id="835db-143">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="835db-143">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="835db-144">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="835db-144">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="835db-145">ttl</span><span class="sxs-lookup"><span data-stu-id="835db-145">ttl</span></span>|<span data-ttu-id="835db-146">Int32</span><span class="sxs-lookup"><span data-stu-id="835db-146">Int32</span></span>| <span data-ttu-id="835db-p105">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="835db-p105">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="835db-149">weight</span><span class="sxs-lookup"><span data-stu-id="835db-149">weight</span></span>|<span data-ttu-id="835db-150">Int32</span><span class="sxs-lookup"><span data-stu-id="835db-150">Int32</span></span>| <span data-ttu-id="835db-151">O valor a ser usado ao configurar a propriedade *weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="835db-151">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="835db-152">Relações</span><span class="sxs-lookup"><span data-stu-id="835db-152">Relationships</span></span>
<span data-ttu-id="835db-153">Nenhum</span><span class="sxs-lookup"><span data-stu-id="835db-153">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="835db-154">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="835db-154">JSON representation</span></span>
<span data-ttu-id="835db-155">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="835db-155">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->