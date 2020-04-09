---
title: tipo de recurso domainDnsRecord
description: A entidade DomainDnsRecord é usada para apresentar registros DNS.
localization_priority: Normal
author: adimitui
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6e2b64a15f49e31384045adcfe85758af06e1e92
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181641"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="8c630-103">tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="8c630-103">domainDnsRecord resource type</span></span>

<span data-ttu-id="8c630-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c630-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8c630-105">Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="8c630-105">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="8c630-106">A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS.</span><span class="sxs-lookup"><span data-stu-id="8c630-106">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="8c630-107">Entidade base para entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsTxtRecord](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="8c630-107">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="8c630-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="8c630-108">Methods</span></span>
<span data-ttu-id="8c630-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="8c630-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8c630-110">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="8c630-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8c630-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8c630-111">Properties</span></span>
| <span data-ttu-id="8c630-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8c630-112">Property</span></span>     | <span data-ttu-id="8c630-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="8c630-113">Type</span></span>   |<span data-ttu-id="8c630-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c630-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8c630-115">id</span><span class="sxs-lookup"><span data-stu-id="8c630-115">id</span></span>|<span data-ttu-id="8c630-116">String</span><span class="sxs-lookup"><span data-stu-id="8c630-116">String</span></span>| <span data-ttu-id="8c630-117">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="8c630-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8c630-118">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8c630-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="8c630-119">IsOptional</span><span class="sxs-lookup"><span data-stu-id="8c630-119">isOptional</span></span>|<span data-ttu-id="8c630-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="8c630-120">Boolean</span></span>| <span data-ttu-id="8c630-121">Se for false, esse registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="8c630-121">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8c630-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="8c630-122">label</span></span>|<span data-ttu-id="8c630-123">String</span><span class="sxs-lookup"><span data-stu-id="8c630-123">String</span></span>| <span data-ttu-id="8c630-124">O valor usado ao configurar o nome do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="8c630-124">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="8c630-125">recordType</span><span class="sxs-lookup"><span data-stu-id="8c630-125">recordType</span></span>|<span data-ttu-id="8c630-126">String</span><span class="sxs-lookup"><span data-stu-id="8c630-126">String</span></span>| <span data-ttu-id="8c630-127">Indica o tipo de registro DNS que esta entidade representa.</span><span class="sxs-lookup"><span data-stu-id="8c630-127">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="8c630-128">O valor pode ser um dos seguintes: *CNAME*, *MX*, *SRV*, *txt*</span><span class="sxs-lookup"><span data-stu-id="8c630-128">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="8c630-129">Chave</span><span class="sxs-lookup"><span data-stu-id="8c630-129">Key</span></span> |
|<span data-ttu-id="8c630-130">supportedService</span><span class="sxs-lookup"><span data-stu-id="8c630-130">supportedService</span></span>|<span data-ttu-id="8c630-131">String</span><span class="sxs-lookup"><span data-stu-id="8c630-131">String</span></span>| <span data-ttu-id="8c630-132">O Microsoft Online Services ou o recurso que tem uma dependência neste registro DNS.</span><span class="sxs-lookup"><span data-stu-id="8c630-132">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="8c630-133">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="8c630-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="8c630-134">TTL</span><span class="sxs-lookup"><span data-stu-id="8c630-134">ttl</span></span>|<span data-ttu-id="8c630-135">Int32</span><span class="sxs-lookup"><span data-stu-id="8c630-135">Int32</span></span>| <span data-ttu-id="8c630-136">O valor a ser usado ao configurar a propriedade time-to-Live (TTL) do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="8c630-136">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="8c630-137">Não anulável</span><span class="sxs-lookup"><span data-stu-id="8c630-137">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8c630-138">Relações</span><span class="sxs-lookup"><span data-stu-id="8c630-138">Relationships</span></span>
<span data-ttu-id="8c630-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8c630-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c630-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8c630-140">JSON representation</span></span>
<span data-ttu-id="8c630-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8c630-141">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
