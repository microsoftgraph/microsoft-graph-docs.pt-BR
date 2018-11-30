---
title: Tipo de recurso domainDnsUnavailableRecord
description: Quando você consulta para a propriedade de navegação **serviceConfigurationRecords** para uma entidade de domínio, você pode obter novamente uma ou mais entidades de DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e/ou DomainDnsTxtRecord. Essas entidades indicam quais registros DNS, você deve adicionar o arquivo de zona do domínio, antes que o domínio pode ser usado pelo Microsoft Online Services. Quando não é possível gerar tais entidades, uma entidade DomainDnsUnavailableRecord é retornada em vez disso. Herdado de entidade DomainDnsRecord.
ms.openlocfilehash: 0d920a2185cc84f5ca5cff571e1bb2c2d00400b5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033770"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="553d6-106">Tipo de recurso domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="553d6-106">domainDnsUnavailableRecord resource type</span></span>

> <span data-ttu-id="553d6-107">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="553d6-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="553d6-108">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="553d6-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="553d6-p103">Ao consultar a propriedade de navegação **serviceConfigurationRecords** de uma entidade [Domain](domain.md), você pode receber novamente uma ou mais entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e/ou [DomainDnsTxtRecord](domaindnstxtrecord.md). Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio antes que ele possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="553d6-p103">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="553d6-113">Métodos</span><span class="sxs-lookup"><span data-stu-id="553d6-113">Methods</span></span>
<span data-ttu-id="553d6-p104">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="553d6-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="553d6-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="553d6-116">Properties</span></span>
| <span data-ttu-id="553d6-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="553d6-117">Property</span></span>     | <span data-ttu-id="553d6-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="553d6-118">Type</span></span>   |<span data-ttu-id="553d6-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="553d6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="553d6-120">description</span><span class="sxs-lookup"><span data-stu-id="553d6-120">description</span></span>|<span data-ttu-id="553d6-121">String</span><span class="sxs-lookup"><span data-stu-id="553d6-121">String</span></span>|<span data-ttu-id="553d6-122">Fornece a razão pela qual a entidade **DomainDnsUnavailableRecord** será retornada.</span><span class="sxs-lookup"><span data-stu-id="553d6-122">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="553d6-123">Relações</span><span class="sxs-lookup"><span data-stu-id="553d6-123">Relationships</span></span>
<span data-ttu-id="553d6-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="553d6-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="553d6-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="553d6-125">JSON representation</span></span>
<span data-ttu-id="553d6-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="553d6-126">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsUnavailableRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->