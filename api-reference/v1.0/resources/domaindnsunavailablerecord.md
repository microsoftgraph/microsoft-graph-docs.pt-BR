# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="58592-101">Tipo de recurso domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="58592-101">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="58592-p101">Ao consultar a propriedade de navegação **serviceConfigurationRecords** de uma entidade [Domain](domain.md), você pode receber novamente uma ou mais entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e/ou [DomainDnsTxtRecord](domaindnstxtrecord.md). Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio antes que ele possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="58592-p101">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="58592-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="58592-106">Methods</span></span>
<span data-ttu-id="58592-p102">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="58592-p102">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="58592-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="58592-109">Properties</span></span>
| <span data-ttu-id="58592-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58592-110">Property</span></span>     | <span data-ttu-id="58592-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="58592-111">Type</span></span>   |<span data-ttu-id="58592-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="58592-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="58592-113">descrição</span><span class="sxs-lookup"><span data-stu-id="58592-113">description</span></span>|<span data-ttu-id="58592-114">String</span><span class="sxs-lookup"><span data-stu-id="58592-114">String</span></span>|<span data-ttu-id="58592-115">Fornece a razão pela qual a entidade **DomainDnsUnavailableRecord** será retornada.</span><span class="sxs-lookup"><span data-stu-id="58592-115">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="58592-116">Relações</span><span class="sxs-lookup"><span data-stu-id="58592-116">Relationships</span></span>
<span data-ttu-id="58592-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="58592-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58592-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="58592-118">JSON representation</span></span>
<span data-ttu-id="58592-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="58592-119">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "description": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->