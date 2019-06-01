---
title: tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1e7563d90a92e319ceec5a5ca11d7edb4f267c5b
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657662"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="f6e18-104">tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="f6e18-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="f6e18-105">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="f6e18-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="f6e18-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="f6e18-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f6e18-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f6e18-107">Methods</span></span>
<span data-ttu-id="f6e18-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="f6e18-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="f6e18-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="f6e18-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f6e18-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f6e18-110">Properties</span></span>
| <span data-ttu-id="f6e18-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f6e18-111">Property</span></span>     | <span data-ttu-id="f6e18-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f6e18-112">Type</span></span>   |<span data-ttu-id="f6e18-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f6e18-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f6e18-114">id</span><span class="sxs-lookup"><span data-stu-id="f6e18-114">id</span></span>|<span data-ttu-id="f6e18-115">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-115">String</span></span>| <span data-ttu-id="f6e18-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="f6e18-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="f6e18-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f6e18-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="f6e18-118">IsOptional</span><span class="sxs-lookup"><span data-stu-id="f6e18-118">isOptional</span></span>|<span data-ttu-id="f6e18-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="f6e18-119">Boolean</span></span>| <span data-ttu-id="f6e18-120">Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="f6e18-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="f6e18-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="f6e18-121">label</span></span>|<span data-ttu-id="f6e18-122">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-122">String</span></span>| <span data-ttu-id="f6e18-123">O valor usado ao configurar a propriedade *Name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="f6e18-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="f6e18-124">nameTarget</span></span>|<span data-ttu-id="f6e18-125">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-125">String</span></span>| <span data-ttu-id="f6e18-126">O valor a ser usado ao configurar a propriedade *target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="f6e18-127">propor</span><span class="sxs-lookup"><span data-stu-id="f6e18-127">port</span></span>|<span data-ttu-id="f6e18-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e18-128">Int32</span></span>| <span data-ttu-id="f6e18-129">O valor a ser usado ao configurar a propriedade *Port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="f6e18-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="f6e18-130">priority</span></span>|<span data-ttu-id="f6e18-131">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e18-131">Int32</span></span>| <span data-ttu-id="f6e18-132">O valor a ser usado ao configurar a propriedade *Priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="f6e18-133">RDP</span><span class="sxs-lookup"><span data-stu-id="f6e18-133">protocol</span></span>|<span data-ttu-id="f6e18-134">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-134">String</span></span>| <span data-ttu-id="f6e18-135">O valor a ser usado ao configurar a propriedade *Protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="f6e18-136">recordType</span><span class="sxs-lookup"><span data-stu-id="f6e18-136">recordType</span></span>|<span data-ttu-id="f6e18-137">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-137">String</span></span>|  <span data-ttu-id="f6e18-138">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-138">Type of DNS record.</span></span> <span data-ttu-id="f6e18-139">O valor é sempre *SRV*.</span><span class="sxs-lookup"><span data-stu-id="f6e18-139">The value is always *Srv*.</span></span> <span data-ttu-id="f6e18-140">Chave</span><span class="sxs-lookup"><span data-stu-id="f6e18-140">Key</span></span> |
|<span data-ttu-id="f6e18-141">service</span><span class="sxs-lookup"><span data-stu-id="f6e18-141">service</span></span>|<span data-ttu-id="f6e18-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f6e18-142">String</span></span>| <span data-ttu-id="f6e18-143">O valor a ser usado ao configurar a propriedade *Service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="f6e18-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="f6e18-144">supportedService</span></span>|<span data-ttu-id="f6e18-145">String</span><span class="sxs-lookup"><span data-stu-id="f6e18-145">String</span></span>| <span data-ttu-id="f6e18-146">O Microsoft Online Services ou o recurso que tem uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="f6e18-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="f6e18-147">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="f6e18-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="f6e18-148">TTL</span><span class="sxs-lookup"><span data-stu-id="f6e18-148">ttl</span></span>|<span data-ttu-id="f6e18-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e18-149">Int32</span></span>| <span data-ttu-id="f6e18-150">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="f6e18-151">Não anulável</span><span class="sxs-lookup"><span data-stu-id="f6e18-151">Not nullable</span></span> |
|<span data-ttu-id="f6e18-152">weight</span><span class="sxs-lookup"><span data-stu-id="f6e18-152">weight</span></span>|<span data-ttu-id="f6e18-153">Int32</span><span class="sxs-lookup"><span data-stu-id="f6e18-153">Int32</span></span>| <span data-ttu-id="f6e18-154">O valor a ser usado ao configurar a propriedade *Weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f6e18-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f6e18-155">Relações</span><span class="sxs-lookup"><span data-stu-id="f6e18-155">Relationships</span></span>
<span data-ttu-id="f6e18-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f6e18-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f6e18-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f6e18-157">JSON representation</span></span>
<span data-ttu-id="f6e18-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f6e18-158">Here is a JSON representation of the resource.</span></span>

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
