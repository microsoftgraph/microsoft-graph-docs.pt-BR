---
title: tipo de recurso domainDnsUnavailableRecord
description: Ao consultar a propriedade de navegação **serviceConfigurationRecords** para uma entidade de domínio, você pode obter uma ou mais entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e/ou DomainDnsTxtRecord. Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio, antes que o domínio possa ser usado pelo Microsoft Online Services. Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada. Herdado de entidade DomainDnsRecord.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bf51b05614a89318fb7ba1afee9c4154ea1f6f27
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973101"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="862a9-106">tipo de recurso domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="862a9-106">domainDnsUnavailableRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="862a9-107">Ao consultar a propriedade de navegação **serviceConfigurationRecords** para uma entidade de [domínio](domain.md) , você pode obter uma ou mais [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md)e/ou [ Entidades DomainDnsTxtRecord](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="862a9-107">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="862a9-108">Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio, antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="862a9-108">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="862a9-109">Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada.</span><span class="sxs-lookup"><span data-stu-id="862a9-109">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="862a9-110">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="862a9-110">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="862a9-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="862a9-111">Methods</span></span>
<span data-ttu-id="862a9-112">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="862a9-112">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="862a9-113">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="862a9-113">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="862a9-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="862a9-114">Properties</span></span>
| <span data-ttu-id="862a9-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="862a9-115">Property</span></span>     | <span data-ttu-id="862a9-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="862a9-116">Type</span></span>   |<span data-ttu-id="862a9-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="862a9-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="862a9-118">description</span><span class="sxs-lookup"><span data-stu-id="862a9-118">description</span></span>|<span data-ttu-id="862a9-119">String</span><span class="sxs-lookup"><span data-stu-id="862a9-119">String</span></span>|<span data-ttu-id="862a9-120">Fornece o motivo pelo qual a entidade **DomainDnsUnavailableRecord** é retornada.</span><span class="sxs-lookup"><span data-stu-id="862a9-120">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="862a9-121">Relações</span><span class="sxs-lookup"><span data-stu-id="862a9-121">Relationships</span></span>
<span data-ttu-id="862a9-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="862a9-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="862a9-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="862a9-123">JSON representation</span></span>
<span data-ttu-id="862a9-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="862a9-124">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
