---
title: Tipo de recurso domainDnsRecord
description: A entidade DomainDnsRecord é usada para apresentar registros DNS.
localization_priority: Normal
author: adimitui
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e3a5152d5eb59a4a1547ee8c7fcc6dbf88c1d976
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137603"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="85564-103">Tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="85564-103">domainDnsRecord resource type</span></span>

<span data-ttu-id="85564-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85564-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85564-105">Para cada domínio no locatário, talvez seja necessário adicionar registros DNS ao arquivo de zona DNS do domínio antes que o domínio possa ser usado pelo Microsoft Online Services.</span><span class="sxs-lookup"><span data-stu-id="85564-105">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services.</span></span> <span data-ttu-id="85564-106">A **entidade DomainDnsRecord** é usada para apresentar esses registros DNS.</span><span class="sxs-lookup"><span data-stu-id="85564-106">The **DomainDnsRecord** entity is used to present such DNS records.</span></span> <span data-ttu-id="85564-107">Entidade base [para entidades DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [domainDnsTxtRecord.](domaindnstxtrecord.md)</span><span class="sxs-lookup"><span data-stu-id="85564-107">Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsTxtRecord](domaindnstxtrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="85564-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="85564-108">Methods</span></span>
<span data-ttu-id="85564-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="85564-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="85564-110">Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="85564-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="85564-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85564-111">Properties</span></span>
| <span data-ttu-id="85564-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85564-112">Property</span></span>     | <span data-ttu-id="85564-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="85564-113">Type</span></span>   |<span data-ttu-id="85564-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="85564-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="85564-115">id</span><span class="sxs-lookup"><span data-stu-id="85564-115">id</span></span>|<span data-ttu-id="85564-116">String</span><span class="sxs-lookup"><span data-stu-id="85564-116">String</span></span>| <span data-ttu-id="85564-117">Identificador exclusivo atribuído a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="85564-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="85564-118">Não anulavel, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="85564-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="85564-119">isOptional</span><span class="sxs-lookup"><span data-stu-id="85564-119">isOptional</span></span>|<span data-ttu-id="85564-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="85564-120">Boolean</span></span>| <span data-ttu-id="85564-121">Se for falso, esse registro deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para operar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="85564-121">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="85564-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="85564-122">label</span></span>|<span data-ttu-id="85564-123">String</span><span class="sxs-lookup"><span data-stu-id="85564-123">String</span></span>| <span data-ttu-id="85564-124">Valor usado ao configurar o nome do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="85564-124">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="85564-125">recordType</span><span class="sxs-lookup"><span data-stu-id="85564-125">recordType</span></span>|<span data-ttu-id="85564-126">String</span><span class="sxs-lookup"><span data-stu-id="85564-126">String</span></span>| <span data-ttu-id="85564-127">Indica o tipo de registro DNS que essa entidade representa.</span><span class="sxs-lookup"><span data-stu-id="85564-127">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="85564-128">O valor pode ser um dos seguintes: *CName*, *Mx*, *Srv*, *Txt*</span><span class="sxs-lookup"><span data-stu-id="85564-128">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="85564-129">Chave</span><span class="sxs-lookup"><span data-stu-id="85564-129">Key</span></span> |
|<span data-ttu-id="85564-130">supportedService</span><span class="sxs-lookup"><span data-stu-id="85564-130">supportedService</span></span>|<span data-ttu-id="85564-131">String</span><span class="sxs-lookup"><span data-stu-id="85564-131">String</span></span>| <span data-ttu-id="85564-132">Microsoft Online Service ou recurso que tem uma dependência nesse registro DNS.</span><span class="sxs-lookup"><span data-stu-id="85564-132">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="85564-133">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="85564-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="85564-134">ttl</span><span class="sxs-lookup"><span data-stu-id="85564-134">ttl</span></span>|<span data-ttu-id="85564-135">Int32</span><span class="sxs-lookup"><span data-stu-id="85564-135">Int32</span></span>| <span data-ttu-id="85564-136">Valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="85564-136">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host.</span></span> <span data-ttu-id="85564-137">Não anulavel</span><span class="sxs-lookup"><span data-stu-id="85564-137">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="85564-138">Relações</span><span class="sxs-lookup"><span data-stu-id="85564-138">Relationships</span></span>
<span data-ttu-id="85564-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85564-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="85564-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85564-140">JSON representation</span></span>
<span data-ttu-id="85564-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85564-141">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


