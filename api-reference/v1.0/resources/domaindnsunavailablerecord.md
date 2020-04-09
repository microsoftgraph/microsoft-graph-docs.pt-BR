---
title: tipo de recurso domainDnsUnavailableRecord
description: Indica que o serviceConfigurationRecords não pode ser gerado.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 67871266e6a51101ea6ad718ab9959b6daff2a1d
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181620"
---
# <a name="domaindnsunavailablerecord-resource-type"></a><span data-ttu-id="5427e-103">tipo de recurso domainDnsUnavailableRecord</span><span class="sxs-lookup"><span data-stu-id="5427e-103">domainDnsUnavailableRecord resource type</span></span>

<span data-ttu-id="5427e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5427e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5427e-105">Ao consultar a propriedade de navegação **serviceConfigurationRecords** para uma entidade de [domínio](domain.md) , você pode obter uma ou mais entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md)e/ou [DomainDnsTxtRecord](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="5427e-105">When you query for the navigation property **serviceConfigurationRecords** for a [Domain](domain.md) entity, you may get back one or more [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md), and/or [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span> <span data-ttu-id="5427e-106">Essas entidades indicam quais registros DNS você deve adicionar ao arquivo de zona do domínio, antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="5427e-106">These entities indicate what DNS records you must add to the zone file of the domain, before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="5427e-107">Quando não for possível gerar essas entidades, uma entidade DomainDnsUnavailableRecord será retornada.</span><span class="sxs-lookup"><span data-stu-id="5427e-107">When it is not possible to generate such entities, a DomainDnsUnavailableRecord Entity is returned instead.</span></span> <span data-ttu-id="5427e-108">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="5427e-108">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5427e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="5427e-109">Methods</span></span>
<span data-ttu-id="5427e-110">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="5427e-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="5427e-111">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="5427e-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5427e-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5427e-112">Properties</span></span>
| <span data-ttu-id="5427e-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5427e-113">Property</span></span>     | <span data-ttu-id="5427e-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="5427e-114">Type</span></span>   |<span data-ttu-id="5427e-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="5427e-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5427e-116">description</span><span class="sxs-lookup"><span data-stu-id="5427e-116">description</span></span>|<span data-ttu-id="5427e-117">String</span><span class="sxs-lookup"><span data-stu-id="5427e-117">String</span></span>|<span data-ttu-id="5427e-118">Fornece o motivo pelo qual a entidade **DomainDnsUnavailableRecord** é retornada.</span><span class="sxs-lookup"><span data-stu-id="5427e-118">Provides the reason why the **DomainDnsUnavailableRecord** entity is returned.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5427e-119">Relações</span><span class="sxs-lookup"><span data-stu-id="5427e-119">Relationships</span></span>
<span data-ttu-id="5427e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5427e-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5427e-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5427e-121">JSON representation</span></span>
<span data-ttu-id="5427e-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5427e-122">Here is a JSON representation of the resource.</span></span>

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
