# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="c2138-101">Tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="c2138-101">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="c2138-p101">Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="c2138-p101">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="c2138-104">Métodos</span><span class="sxs-lookup"><span data-stu-id="c2138-104">Methods</span></span>
<span data-ttu-id="c2138-p102">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="c2138-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c2138-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2138-107">Properties</span></span>
| <span data-ttu-id="c2138-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2138-108">Property</span></span>     | <span data-ttu-id="c2138-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2138-109">Type</span></span>   |<span data-ttu-id="c2138-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2138-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c2138-111">canonicalName</span><span class="sxs-lookup"><span data-stu-id="c2138-111">canonicalName</span></span>|<span data-ttu-id="c2138-112">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2138-112">String</span></span>| <span data-ttu-id="c2138-p103">O nome canônico do registro CNAME. Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c2138-p103">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="c2138-115">id</span><span class="sxs-lookup"><span data-stu-id="c2138-115">id</span></span>|<span data-ttu-id="c2138-116">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2138-116">String</span></span>| <span data-ttu-id="c2138-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura</span><span class="sxs-lookup"><span data-stu-id="c2138-p104">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="c2138-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="c2138-119">isOptional</span></span>|<span data-ttu-id="c2138-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c2138-120">Boolean</span></span>| <span data-ttu-id="c2138-p105">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. Não anulável</span><span class="sxs-lookup"><span data-stu-id="c2138-p105">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="c2138-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="c2138-123">label</span></span>|<span data-ttu-id="c2138-124">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2138-124">String</span></span>| <span data-ttu-id="c2138-125">O valor usado ao configurar a propriedade *alias/host/name* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c2138-125">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="c2138-126">recordType</span><span class="sxs-lookup"><span data-stu-id="c2138-126">recordType</span></span>|<span data-ttu-id="c2138-127">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2138-127">String</span></span>| <span data-ttu-id="c2138-p106">Tipo do registro DNS. Este valor sempre será *CName*. Chave</span><span class="sxs-lookup"><span data-stu-id="c2138-p106">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="c2138-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="c2138-131">supportedService</span></span>|<span data-ttu-id="c2138-132">Sequência de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2138-132">String</span></span>| <span data-ttu-id="c2138-133">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="c2138-133">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="c2138-134">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="c2138-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="c2138-135">ttl</span><span class="sxs-lookup"><span data-stu-id="c2138-135">ttl</span></span>|<span data-ttu-id="c2138-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c2138-136">Int32</span></span>| <span data-ttu-id="c2138-p107">O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro CNAME no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="c2138-p107">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="c2138-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c2138-139">Relationships</span></span>
<span data-ttu-id="c2138-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2138-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c2138-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2138-141">JSON representation</span></span>
<span data-ttu-id="c2138-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2138-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->