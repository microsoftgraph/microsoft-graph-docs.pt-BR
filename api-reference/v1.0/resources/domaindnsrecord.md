---
title: Tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar registro (s) DNS para o arquivo de zona DNS do domínio para que o domínio que possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsSrvRecord.
localization_priority: Normal
ms.openlocfilehash: 30c5f63f4ecac2c716f7884ccf82fd129125c8b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822341"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="922c7-105">Tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="922c7-105">domainDnsRecord resource type</span></span>

<span data-ttu-id="922c7-p102">Para cada domínio no locatário, talvez seja necessário adicionar os registros DNS ao arquivo de zona DNS do domínio para que ele possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. A entidade base das entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsSrvRecord](domaindnssrvrecord.md).</span><span class="sxs-lookup"><span data-stu-id="922c7-p102">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="922c7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="922c7-109">Methods</span></span>
<span data-ttu-id="922c7-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="922c7-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="922c7-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="922c7-112">Properties</span></span>
| <span data-ttu-id="922c7-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="922c7-113">Property</span></span>     | <span data-ttu-id="922c7-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="922c7-114">Type</span></span>   |<span data-ttu-id="922c7-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="922c7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="922c7-116">id</span><span class="sxs-lookup"><span data-stu-id="922c7-116">id</span></span>|<span data-ttu-id="922c7-117">String</span><span class="sxs-lookup"><span data-stu-id="922c7-117">String</span></span>| <span data-ttu-id="922c7-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="922c7-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="922c7-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="922c7-120">isOptional</span></span>|<span data-ttu-id="922c7-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="922c7-121">Boolean</span></span>| <span data-ttu-id="922c7-122">Se for falso, o registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="922c7-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="922c7-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="922c7-123">label</span></span>|<span data-ttu-id="922c7-124">String</span><span class="sxs-lookup"><span data-stu-id="922c7-124">String</span></span>| <span data-ttu-id="922c7-125">O valor usado ao configurar o nome da propriedade do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="922c7-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="922c7-126">recordType</span><span class="sxs-lookup"><span data-stu-id="922c7-126">recordType</span></span>|<span data-ttu-id="922c7-127">String</span><span class="sxs-lookup"><span data-stu-id="922c7-127">String</span></span>| <span data-ttu-id="922c7-128">Indica que tipo de registro DNS a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="922c7-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="922c7-129">O valor pode ser um dos seguintes: *CName*, *Mx*, *Srv* e *Txt*</span><span class="sxs-lookup"><span data-stu-id="922c7-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="922c7-130">Chave</span><span class="sxs-lookup"><span data-stu-id="922c7-130">Key</span></span> |
|<span data-ttu-id="922c7-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="922c7-131">supportedService</span></span>|<span data-ttu-id="922c7-132">String</span><span class="sxs-lookup"><span data-stu-id="922c7-132">String</span></span>| <span data-ttu-id="922c7-133">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro DNS.</span><span class="sxs-lookup"><span data-stu-id="922c7-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="922c7-134">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="922c7-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="922c7-135">ttl</span><span class="sxs-lookup"><span data-stu-id="922c7-135">ttl</span></span>|<span data-ttu-id="922c7-136">Int32</span><span class="sxs-lookup"><span data-stu-id="922c7-136">Int32</span></span>| <span data-ttu-id="922c7-p105">O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="922c7-p105">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="922c7-139">Relações</span><span class="sxs-lookup"><span data-stu-id="922c7-139">Relationships</span></span>
<span data-ttu-id="922c7-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="922c7-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="922c7-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="922c7-141">JSON representation</span></span>
<span data-ttu-id="922c7-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="922c7-142">Here is a JSON representation of the resource.</span></span>

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
