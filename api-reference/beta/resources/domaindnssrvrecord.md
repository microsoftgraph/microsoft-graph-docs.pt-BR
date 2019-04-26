---
title: tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a80bfd1caa755a7b4f27f29e1c34ec4295a52f33
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340677"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="96506-104">tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="96506-104">domainDnsSrvRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="96506-105">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="96506-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="96506-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="96506-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="96506-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="96506-107">Methods</span></span>
<span data-ttu-id="96506-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="96506-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="96506-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="96506-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="96506-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96506-110">Properties</span></span>
| <span data-ttu-id="96506-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96506-111">Property</span></span>     | <span data-ttu-id="96506-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="96506-112">Type</span></span>   |<span data-ttu-id="96506-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="96506-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="96506-114">id</span><span class="sxs-lookup"><span data-stu-id="96506-114">id</span></span>|<span data-ttu-id="96506-115">String</span><span class="sxs-lookup"><span data-stu-id="96506-115">String</span></span>| <span data-ttu-id="96506-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="96506-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="96506-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="96506-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="96506-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="96506-118">isOptional</span></span>|<span data-ttu-id="96506-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="96506-119">Boolean</span></span>| <span data-ttu-id="96506-120">Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="96506-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="96506-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="96506-121">label</span></span>|<span data-ttu-id="96506-122">String</span><span class="sxs-lookup"><span data-stu-id="96506-122">String</span></span>| <span data-ttu-id="96506-123">O valor usado ao configurar a propriedade *Name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="96506-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="96506-124">nameTarget</span></span>|<span data-ttu-id="96506-125">String</span><span class="sxs-lookup"><span data-stu-id="96506-125">String</span></span>| <span data-ttu-id="96506-126">O valor a ser usado ao configurar a propriedade *target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="96506-127">propor</span><span class="sxs-lookup"><span data-stu-id="96506-127">port</span></span>|<span data-ttu-id="96506-128">Int32</span><span class="sxs-lookup"><span data-stu-id="96506-128">Int32</span></span>| <span data-ttu-id="96506-129">O valor a ser usado ao configurar a propriedade *Port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="96506-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="96506-130">priority</span></span>|<span data-ttu-id="96506-131">Int32</span><span class="sxs-lookup"><span data-stu-id="96506-131">Int32</span></span>| <span data-ttu-id="96506-132">O valor a ser usado ao configurar a propriedade *Priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="96506-133">RDP</span><span class="sxs-lookup"><span data-stu-id="96506-133">protocol</span></span>|<span data-ttu-id="96506-134">String</span><span class="sxs-lookup"><span data-stu-id="96506-134">String</span></span>| <span data-ttu-id="96506-135">O valor a ser usado ao configurar a propriedade *Protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="96506-136">recordType</span><span class="sxs-lookup"><span data-stu-id="96506-136">recordType</span></span>|<span data-ttu-id="96506-137">String</span><span class="sxs-lookup"><span data-stu-id="96506-137">String</span></span>|  <span data-ttu-id="96506-138">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-138">Type of DNS record.</span></span> <span data-ttu-id="96506-139">O valor é sempre *SRV*.</span><span class="sxs-lookup"><span data-stu-id="96506-139">The value is always *Srv*.</span></span> <span data-ttu-id="96506-140">Chave</span><span class="sxs-lookup"><span data-stu-id="96506-140">Key</span></span> |
|<span data-ttu-id="96506-141">service</span><span class="sxs-lookup"><span data-stu-id="96506-141">service</span></span>|<span data-ttu-id="96506-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="96506-142">String</span></span>| <span data-ttu-id="96506-143">O valor a ser usado ao configurar a propriedade *Service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="96506-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="96506-144">supportedService</span></span>|<span data-ttu-id="96506-145">String</span><span class="sxs-lookup"><span data-stu-id="96506-145">String</span></span>| <span data-ttu-id="96506-146">O Microsoft Online Services ou o recurso que tem uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="96506-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="96506-147">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="96506-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="96506-148">TTL</span><span class="sxs-lookup"><span data-stu-id="96506-148">ttl</span></span>|<span data-ttu-id="96506-149">Int32</span><span class="sxs-lookup"><span data-stu-id="96506-149">Int32</span></span>| <span data-ttu-id="96506-150">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="96506-151">Não anulável</span><span class="sxs-lookup"><span data-stu-id="96506-151">Not nullable</span></span> |
|<span data-ttu-id="96506-152">weight</span><span class="sxs-lookup"><span data-stu-id="96506-152">weight</span></span>|<span data-ttu-id="96506-153">Int32</span><span class="sxs-lookup"><span data-stu-id="96506-153">Int32</span></span>| <span data-ttu-id="96506-154">O valor a ser usado ao configurar a propriedade *Weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="96506-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="96506-155">Relações</span><span class="sxs-lookup"><span data-stu-id="96506-155">Relationships</span></span>
<span data-ttu-id="96506-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96506-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="96506-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96506-157">JSON representation</span></span>
<span data-ttu-id="96506-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96506-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "nameTarget": "String",
  "port": 1024,
  "priority": 1024,
  "protocol": "String",
  "recordType": "String",
  "service": "String",
  "supportedService": "String",
  "ttl": 1024,
  "weight": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
