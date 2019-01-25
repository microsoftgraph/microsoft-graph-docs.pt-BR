---
title: Tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar os registros DNS ao arquivo de zona DNS do domínio para que ele possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. A entidade base das entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsSrvRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b7b04e65da67bc61e3f3b91ed3dae7cba70a3d27
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519280"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="c31a5-105">Tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="c31a5-105">domainDnsRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c31a5-p102">Para cada domínio no locatário, talvez seja necessário adicionar os registros DNS ao arquivo de zona DNS do domínio para que ele possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. A entidade base das entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsSrvRecord](domaindnssrvrecord.md).</span><span class="sxs-lookup"><span data-stu-id="c31a5-p102">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="c31a5-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="c31a5-109">Methods</span></span>
<span data-ttu-id="c31a5-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="c31a5-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c31a5-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c31a5-112">Properties</span></span>
| <span data-ttu-id="c31a5-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c31a5-113">Property</span></span>     | <span data-ttu-id="c31a5-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="c31a5-114">Type</span></span>   |<span data-ttu-id="c31a5-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="c31a5-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c31a5-116">id</span><span class="sxs-lookup"><span data-stu-id="c31a5-116">id</span></span>|<span data-ttu-id="c31a5-117">String</span><span class="sxs-lookup"><span data-stu-id="c31a5-117">String</span></span>| <span data-ttu-id="c31a5-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="c31a5-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="c31a5-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="c31a5-120">isOptional</span></span>|<span data-ttu-id="c31a5-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c31a5-121">Boolean</span></span>| <span data-ttu-id="c31a5-122">Se for falso, o registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="c31a5-122">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="c31a5-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="c31a5-123">label</span></span>|<span data-ttu-id="c31a5-124">String</span><span class="sxs-lookup"><span data-stu-id="c31a5-124">String</span></span>| <span data-ttu-id="c31a5-125">O valor usado ao configurar o nome da propriedade do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c31a5-125">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="c31a5-126">recordType</span><span class="sxs-lookup"><span data-stu-id="c31a5-126">recordType</span></span>|<span data-ttu-id="c31a5-127">String</span><span class="sxs-lookup"><span data-stu-id="c31a5-127">String</span></span>| <span data-ttu-id="c31a5-128">Indica que tipo de registro DNS a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="c31a5-128">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="c31a5-129">O valor pode ser um dos seguintes: *CName*, *Mx*, *Srv* e *Txt*</span><span class="sxs-lookup"><span data-stu-id="c31a5-129">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="c31a5-130">Tecla</span><span class="sxs-lookup"><span data-stu-id="c31a5-130">Key</span></span> |
|<span data-ttu-id="c31a5-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="c31a5-131">supportedService</span></span>|<span data-ttu-id="c31a5-132">String</span><span class="sxs-lookup"><span data-stu-id="c31a5-132">String</span></span>| <span data-ttu-id="c31a5-133">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro DNS.</span><span class="sxs-lookup"><span data-stu-id="c31a5-133">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="c31a5-134">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="c31a5-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="c31a5-135">ttl</span><span class="sxs-lookup"><span data-stu-id="c31a5-135">ttl</span></span>|<span data-ttu-id="c31a5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="c31a5-136">Int32</span></span>| <span data-ttu-id="c31a5-p105">O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="c31a5-p105">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="c31a5-139">Relações</span><span class="sxs-lookup"><span data-stu-id="c31a5-139">Relationships</span></span>
<span data-ttu-id="c31a5-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c31a5-140">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c31a5-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c31a5-141">JSON representation</span></span>
<span data-ttu-id="c31a5-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c31a5-142">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnsrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
