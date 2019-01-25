---
title: Tipo de recurso domainDnsUnavailableRecord
description: Ao consultar a propriedade de navegação **serviceConfigurationRecords** de uma entidade Domain, você pode receber novamente uma ou mais entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e/ou DomainDnsTxtRecord. Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio antes que ele possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado da entidade DomainDnsRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: fe3c1eeae7ae3ddb634a3c120332dd8d8996f41c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527868"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="de69d-106">Tipo de recurso domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="de69d-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de69d-p102">Ao consultar a propriedade de navegação **serviceConfigurationRecords** de uma entidade [Domain](domain.md), você pode receber novamente uma ou mais entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e/ou [DomainDnsTxtRecord](domaindnstxtrecord.md). Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio antes que ele possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="de69d-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="de69d-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="de69d-111">Methods</span></span>
<span data-ttu-id="de69d-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="de69d-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="de69d-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="de69d-114">Properties</span></span>
| <span data-ttu-id="de69d-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="de69d-115">Property</span></span>     | <span data-ttu-id="de69d-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="de69d-116">Type</span></span>   |<span data-ttu-id="de69d-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="de69d-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de69d-118">description</span><span class="sxs-lookup"><span data-stu-id="de69d-118">description</span></span>|<span data-ttu-id="de69d-119">String</span><span class="sxs-lookup"><span data-stu-id="de69d-119">String</span></span>|<span data-ttu-id="de69d-120">Fornece a razão pela qual a entidade **DomainDnsUnavailableRecord** será retornada.</span><span class="sxs-lookup"><span data-stu-id="de69d-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="de69d-121">Relações</span><span class="sxs-lookup"><span data-stu-id="de69d-121">Relationships</span></span>
<span data-ttu-id="de69d-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="de69d-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="de69d-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="de69d-123">JSON representation</span></span>
<span data-ttu-id="de69d-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="de69d-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsUnavailableRecord"
}-->

```json
{
  "canonicalName": "String",
  "description": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnsunavailablerecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
