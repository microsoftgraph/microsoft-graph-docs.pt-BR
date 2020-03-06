---
title: tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsTxtRecord.
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9402ec0785da87236fa94a9749f8b400f3164e1e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531598"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="cdc6c-105">tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="cdc6c-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="cdc6c-106">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cdc6c-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cdc6c-107">Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-107">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="cdc6c-108">A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-108">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="cdc6c-109">Entidade base para entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsTxtRecord](domaindnstxtrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="cdc6c-109">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="cdc6c-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="cdc6c-110">Methods</span></span>
<span data-ttu-id="cdc6c-111">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-111">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="cdc6c-112">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-112">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="cdc6c-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cdc6c-113">Properties</span></span>
| <span data-ttu-id="cdc6c-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cdc6c-114">Property</span></span>     | <span data-ttu-id="cdc6c-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="cdc6c-115">Type</span></span>   |<span data-ttu-id="cdc6c-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="cdc6c-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cdc6c-117">id</span><span class="sxs-lookup"><span data-stu-id="cdc6c-117">id</span></span>|<span data-ttu-id="cdc6c-118">String</span><span class="sxs-lookup"><span data-stu-id="cdc6c-118">String</span></span>| <span data-ttu-id="cdc6c-119">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-119">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="cdc6c-120">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-120">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="cdc6c-121">IsOptional</span><span class="sxs-lookup"><span data-stu-id="cdc6c-121">isOptional</span></span>|<span data-ttu-id="cdc6c-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="cdc6c-122">Boolean</span></span>| <span data-ttu-id="cdc6c-123">Se for false, esse registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-123">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="cdc6c-124">rótulo</span><span class="sxs-lookup"><span data-stu-id="cdc6c-124">label</span></span>|<span data-ttu-id="cdc6c-125">String</span><span class="sxs-lookup"><span data-stu-id="cdc6c-125">String</span></span>| <span data-ttu-id="cdc6c-126">O valor usado ao configurar o nome do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-126">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="cdc6c-127">recordType</span><span class="sxs-lookup"><span data-stu-id="cdc6c-127">recordType</span></span>|<span data-ttu-id="cdc6c-128">String</span><span class="sxs-lookup"><span data-stu-id="cdc6c-128">String</span></span>| <span data-ttu-id="cdc6c-129">Indica o tipo de registro DNS que esta entidade representa.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-129">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="cdc6c-130">O valor pode ser um dos seguintes: *CNAME*, *MX*, *SRV*, *txt*</span><span class="sxs-lookup"><span data-stu-id="cdc6c-130">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="cdc6c-131">Chave</span><span class="sxs-lookup"><span data-stu-id="cdc6c-131">Key</span></span> |
|<span data-ttu-id="cdc6c-132">supportedService</span><span class="sxs-lookup"><span data-stu-id="cdc6c-132">supportedService</span></span>|<span data-ttu-id="cdc6c-133">String</span><span class="sxs-lookup"><span data-stu-id="cdc6c-133">String</span></span>| <span data-ttu-id="cdc6c-134">O Microsoft Online Services ou o recurso que tem uma dependência neste registro DNS.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-134">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="cdc6c-135">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="cdc6c-135">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="cdc6c-136">TTL</span><span class="sxs-lookup"><span data-stu-id="cdc6c-136">ttl</span></span>|<span data-ttu-id="cdc6c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="cdc6c-137">Int32</span></span>| <span data-ttu-id="cdc6c-138">O valor a ser usado ao configurar a propriedade time-to-Live (TTL) do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-138">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="cdc6c-139">Não anulável</span><span class="sxs-lookup"><span data-stu-id="cdc6c-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="cdc6c-140">Relações</span><span class="sxs-lookup"><span data-stu-id="cdc6c-140">Relationships</span></span>
<span data-ttu-id="cdc6c-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cdc6c-141">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cdc6c-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cdc6c-142">JSON representation</span></span>
<span data-ttu-id="cdc6c-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cdc6c-143">Here is a JSON representation of the resource.</span></span>

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
