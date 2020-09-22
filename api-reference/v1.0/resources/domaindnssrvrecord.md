---
title: tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1c0ac0fce1291c5f6a5134bf7439cbe01c841fe9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48018652"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="c1b2c-103">tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="c1b2c-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="c1b2c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1b2c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c1b2c-105">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="c1b2c-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="c1b2c-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c1b2c-107">Methods</span><span class="sxs-lookup"><span data-stu-id="c1b2c-107">Methods</span></span>
<span data-ttu-id="c1b2c-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="c1b2c-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c1b2c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c1b2c-110">Properties</span></span>
| <span data-ttu-id="c1b2c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c1b2c-111">Property</span></span>     | <span data-ttu-id="c1b2c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="c1b2c-112">Type</span></span>   |<span data-ttu-id="c1b2c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="c1b2c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c1b2c-114">id</span><span class="sxs-lookup"><span data-stu-id="c1b2c-114">id</span></span>|<span data-ttu-id="c1b2c-115">String</span><span class="sxs-lookup"><span data-stu-id="c1b2c-115">String</span></span>| <span data-ttu-id="c1b2c-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="c1b2c-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="c1b2c-118">IsOptional</span><span class="sxs-lookup"><span data-stu-id="c1b2c-118">isOptional</span></span>|<span data-ttu-id="c1b2c-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1b2c-119">Boolean</span></span>| <span data-ttu-id="c1b2c-120">Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="c1b2c-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="c1b2c-121">label</span></span>|<span data-ttu-id="c1b2c-122">String</span><span class="sxs-lookup"><span data-stu-id="c1b2c-122">String</span></span>| <span data-ttu-id="c1b2c-123">O valor usado ao configurar a propriedade *Name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c1b2c-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="c1b2c-124">nameTarget</span></span>|<span data-ttu-id="c1b2c-125">String</span><span class="sxs-lookup"><span data-stu-id="c1b2c-125">String</span></span>| <span data-ttu-id="c1b2c-126">O valor a ser usado ao configurar a propriedade *target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c1b2c-127">propor</span><span class="sxs-lookup"><span data-stu-id="c1b2c-127">port</span></span>|<span data-ttu-id="c1b2c-128">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b2c-128">Int32</span></span>| <span data-ttu-id="c1b2c-129">O valor a ser usado ao configurar a propriedade *Port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c1b2c-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="c1b2c-130">priority</span></span>|<span data-ttu-id="c1b2c-131">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b2c-131">Int32</span></span>| <span data-ttu-id="c1b2c-132">O valor a ser usado ao configurar a propriedade *Priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c1b2c-133">RDP</span><span class="sxs-lookup"><span data-stu-id="c1b2c-133">protocol</span></span>|<span data-ttu-id="c1b2c-134">String</span><span class="sxs-lookup"><span data-stu-id="c1b2c-134">String</span></span>| <span data-ttu-id="c1b2c-135">O valor a ser usado ao configurar a propriedade *Protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c1b2c-136">recordType</span><span class="sxs-lookup"><span data-stu-id="c1b2c-136">recordType</span></span>|<span data-ttu-id="c1b2c-137">String</span><span class="sxs-lookup"><span data-stu-id="c1b2c-137">String</span></span>|  <span data-ttu-id="c1b2c-138">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-138">Type of DNS record.</span></span> <span data-ttu-id="c1b2c-139">O valor é sempre *SRV*.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-139">The value is always *Srv*.</span></span> <span data-ttu-id="c1b2c-140">Chave</span><span class="sxs-lookup"><span data-stu-id="c1b2c-140">Key</span></span> |
|<span data-ttu-id="c1b2c-141">service</span><span class="sxs-lookup"><span data-stu-id="c1b2c-141">service</span></span>|<span data-ttu-id="c1b2c-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c1b2c-142">String</span></span>| <span data-ttu-id="c1b2c-143">O valor a ser usado ao configurar a propriedade *Service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c1b2c-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="c1b2c-144">supportedService</span></span>|<span data-ttu-id="c1b2c-145">String</span><span class="sxs-lookup"><span data-stu-id="c1b2c-145">String</span></span>| <span data-ttu-id="c1b2c-146">O Microsoft Online Services ou o recurso que tem uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="c1b2c-147">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="c1b2c-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="c1b2c-148">TTL</span><span class="sxs-lookup"><span data-stu-id="c1b2c-148">ttl</span></span>|<span data-ttu-id="c1b2c-149">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b2c-149">Int32</span></span>| <span data-ttu-id="c1b2c-150">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="c1b2c-151">Não anulável</span><span class="sxs-lookup"><span data-stu-id="c1b2c-151">Not nullable</span></span> |
|<span data-ttu-id="c1b2c-152">weight</span><span class="sxs-lookup"><span data-stu-id="c1b2c-152">weight</span></span>|<span data-ttu-id="c1b2c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="c1b2c-153">Int32</span></span>| <span data-ttu-id="c1b2c-154">O valor a ser usado ao configurar a propriedade *Weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c1b2c-155">Relações</span><span class="sxs-lookup"><span data-stu-id="c1b2c-155">Relationships</span></span>
<span data-ttu-id="c1b2c-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c1b2c-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c1b2c-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c1b2c-157">JSON representation</span></span>
<span data-ttu-id="c1b2c-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c1b2c-158">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsSrvRecord"
}-->

```json
{
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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

