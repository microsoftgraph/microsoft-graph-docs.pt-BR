---
title: tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsSrvRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7b04e65da67bc61e3f3b91ed3dae7cba70a3d27
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543151"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="577ab-105">tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="577ab-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="577ab-106">Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="577ab-106">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="577ab-107">A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS.</span><span class="sxs-lookup"><span data-stu-id="577ab-107">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="577ab-108">Entidade base para entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsSrvRecord](domaindnssrvrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="577ab-108">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="577ab-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="577ab-109">Methods</span></span>
<span data-ttu-id="577ab-110">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="577ab-110">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="577ab-111">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="577ab-111">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="577ab-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="577ab-112">Properties</span></span>
| <span data-ttu-id="577ab-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="577ab-113">Property</span></span>     | <span data-ttu-id="577ab-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="577ab-114">Type</span></span>   |<span data-ttu-id="577ab-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="577ab-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="577ab-116">id</span><span class="sxs-lookup"><span data-stu-id="577ab-116">id</span></span>|<span data-ttu-id="577ab-117">String</span><span class="sxs-lookup"><span data-stu-id="577ab-117">String</span></span>| <span data-ttu-id="577ab-118">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="577ab-118">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="577ab-119">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="577ab-119">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="577ab-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="577ab-120">isOptional</span></span>|<span data-ttu-id="577ab-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="577ab-121">Boolean</span></span>| <span data-ttu-id="577ab-122">Se for false, esse registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="577ab-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="577ab-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="577ab-123">label</span></span>|<span data-ttu-id="577ab-124">String</span><span class="sxs-lookup"><span data-stu-id="577ab-124">String</span></span>| <span data-ttu-id="577ab-125">O valor usado ao configurar o nome do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="577ab-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="577ab-126">recordType</span><span class="sxs-lookup"><span data-stu-id="577ab-126">recordType</span></span>|<span data-ttu-id="577ab-127">String</span><span class="sxs-lookup"><span data-stu-id="577ab-127">String</span></span>| <span data-ttu-id="577ab-128">Indica o tipo de registro DNS que esta entidade representa.</span><span class="sxs-lookup"><span data-stu-id="577ab-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="577ab-129">O valor pode ser um dos seguintes: *CNAME*, *MX*, *SRV*, *txt*</span><span class="sxs-lookup"><span data-stu-id="577ab-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="577ab-130">Chave</span><span class="sxs-lookup"><span data-stu-id="577ab-130">Key</span></span> |
|<span data-ttu-id="577ab-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="577ab-131">supportedService</span></span>|<span data-ttu-id="577ab-132">String</span><span class="sxs-lookup"><span data-stu-id="577ab-132">String</span></span>| <span data-ttu-id="577ab-133">O Microsoft Online Services ou o recurso que tem uma dependência neste registro DNS.</span><span class="sxs-lookup"><span data-stu-id="577ab-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="577ab-134">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="577ab-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="577ab-135">TTL</span><span class="sxs-lookup"><span data-stu-id="577ab-135">ttl</span></span>|<span data-ttu-id="577ab-136">Int32</span><span class="sxs-lookup"><span data-stu-id="577ab-136">Int32</span></span>| <span data-ttu-id="577ab-137">O valor a ser usado ao configurar a propriedade time-to-Live (TTL) do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="577ab-137">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="577ab-138">Não anulável</span><span class="sxs-lookup"><span data-stu-id="577ab-138">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="577ab-139">Relações</span><span class="sxs-lookup"><span data-stu-id="577ab-139">Relationships</span></span>
<span data-ttu-id="577ab-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="577ab-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="577ab-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="577ab-141">JSON representation</span></span>
<span data-ttu-id="577ab-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="577ab-142">Here is a JSON representation of the resource.</span></span>

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
