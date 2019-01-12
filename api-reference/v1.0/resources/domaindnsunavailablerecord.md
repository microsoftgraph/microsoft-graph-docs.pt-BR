---
title: Tipo de recurso domainDnsUnavailableRecord
description: Quando você consulta para a propriedade de navegação **serviceConfigurationRecords** para uma entidade de domínio, você pode obter novamente uma ou mais entidades de DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e/ou DomainDnsTxtRecord. Essas entidades indicam quais registros DNS, você deve adicionar o arquivo de zona do domínio, antes que o domínio pode ser usado pelo Microsoft Online Services. Quando não é possível gerar tais entidades, uma entidade DomainDnsUnavailableRecord é retornada em vez disso. Herdado de entidade DomainDnsRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5f033c39c9cf8dc11c2a41b0cedb0b8de5ce7736
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27968173"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="ca700-106">Tipo de recurso domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="ca700-106">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="ca700-p102">Ao consultar a propriedade de navegação **serviceConfigurationRecords** de uma entidade [Domain](domain.md), você pode receber novamente uma ou mais entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e/ou [DomainDnsTxtRecord](domaindnstxtrecord.md). Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio antes que ele possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="ca700-p102">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities. These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services. When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="ca700-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="ca700-111">Methods</span></span>
<span data-ttu-id="ca700-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="ca700-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ca700-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ca700-114">Properties</span></span>
| <span data-ttu-id="ca700-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca700-115">Property</span></span>     | <span data-ttu-id="ca700-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca700-116">Type</span></span>   |<span data-ttu-id="ca700-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca700-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca700-118">description</span><span class="sxs-lookup"><span data-stu-id="ca700-118">description</span></span>|<span data-ttu-id="ca700-119">String</span><span class="sxs-lookup"><span data-stu-id="ca700-119">String</span></span>|<span data-ttu-id="ca700-120">Fornece a razão pela qual a entidade **DomainDnsUnavailableRecord** será retornada.</span><span class="sxs-lookup"><span data-stu-id="ca700-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ca700-121">Relações</span><span class="sxs-lookup"><span data-stu-id="ca700-121">Relationships</span></span>
<span data-ttu-id="ca700-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ca700-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ca700-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ca700-123">JSON representation</span></span>
<span data-ttu-id="ca700-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ca700-124">Here is a JSON representation of the resource.</span></span>

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
