---
title: tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 32a9461cb28bc51489ddca6f3b569871bcc584d0
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531591"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="c68e9-104">tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="c68e9-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="c68e9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c68e9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c68e9-106">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="c68e9-106">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="c68e9-107">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="c68e9-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="c68e9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="c68e9-108">Methods</span></span>
<span data-ttu-id="c68e9-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="c68e9-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="c68e9-110">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="c68e9-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="c68e9-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c68e9-111">Properties</span></span>
| <span data-ttu-id="c68e9-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c68e9-112">Property</span></span>     | <span data-ttu-id="c68e9-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="c68e9-113">Type</span></span>   |<span data-ttu-id="c68e9-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="c68e9-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c68e9-115">id</span><span class="sxs-lookup"><span data-stu-id="c68e9-115">id</span></span>|<span data-ttu-id="c68e9-116">String</span><span class="sxs-lookup"><span data-stu-id="c68e9-116">String</span></span>| <span data-ttu-id="c68e9-117">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="c68e9-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="c68e9-118">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c68e9-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="c68e9-119">IsOptional</span><span class="sxs-lookup"><span data-stu-id="c68e9-119">isOptional</span></span>|<span data-ttu-id="c68e9-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="c68e9-120">Boolean</span></span>| <span data-ttu-id="c68e9-121">Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="c68e9-121">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="c68e9-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="c68e9-122">label</span></span>|<span data-ttu-id="c68e9-123">String</span><span class="sxs-lookup"><span data-stu-id="c68e9-123">String</span></span>| <span data-ttu-id="c68e9-124">O valor usado ao configurar a propriedade *Name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-124">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c68e9-125">nameTarget</span><span class="sxs-lookup"><span data-stu-id="c68e9-125">nameTarget</span></span>|<span data-ttu-id="c68e9-126">String</span><span class="sxs-lookup"><span data-stu-id="c68e9-126">String</span></span>| <span data-ttu-id="c68e9-127">O valor a ser usado ao configurar a propriedade *target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-127">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c68e9-128">propor</span><span class="sxs-lookup"><span data-stu-id="c68e9-128">port</span></span>|<span data-ttu-id="c68e9-129">Int32</span><span class="sxs-lookup"><span data-stu-id="c68e9-129">Int32</span></span>| <span data-ttu-id="c68e9-130">O valor a ser usado ao configurar a propriedade *Port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-130">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c68e9-131">prioridade</span><span class="sxs-lookup"><span data-stu-id="c68e9-131">priority</span></span>|<span data-ttu-id="c68e9-132">Int32</span><span class="sxs-lookup"><span data-stu-id="c68e9-132">Int32</span></span>| <span data-ttu-id="c68e9-133">O valor a ser usado ao configurar a propriedade *Priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-133">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c68e9-134">RDP</span><span class="sxs-lookup"><span data-stu-id="c68e9-134">protocol</span></span>|<span data-ttu-id="c68e9-135">String</span><span class="sxs-lookup"><span data-stu-id="c68e9-135">String</span></span>| <span data-ttu-id="c68e9-136">O valor a ser usado ao configurar a propriedade *Protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-136">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c68e9-137">recordType</span><span class="sxs-lookup"><span data-stu-id="c68e9-137">recordType</span></span>|<span data-ttu-id="c68e9-138">String</span><span class="sxs-lookup"><span data-stu-id="c68e9-138">String</span></span>|  <span data-ttu-id="c68e9-139">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-139">Type of DNS record.</span></span> <span data-ttu-id="c68e9-140">O valor é sempre *SRV*.</span><span class="sxs-lookup"><span data-stu-id="c68e9-140">The value is always *Srv*.</span></span> <span data-ttu-id="c68e9-141">Chave</span><span class="sxs-lookup"><span data-stu-id="c68e9-141">Key</span></span> |
|<span data-ttu-id="c68e9-142">service</span><span class="sxs-lookup"><span data-stu-id="c68e9-142">service</span></span>|<span data-ttu-id="c68e9-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c68e9-143">String</span></span>| <span data-ttu-id="c68e9-144">O valor a ser usado ao configurar a propriedade *Service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-144">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="c68e9-145">supportedService</span><span class="sxs-lookup"><span data-stu-id="c68e9-145">supportedService</span></span>|<span data-ttu-id="c68e9-146">String</span><span class="sxs-lookup"><span data-stu-id="c68e9-146">String</span></span>| <span data-ttu-id="c68e9-147">O Microsoft Online Services ou o recurso que tem uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="c68e9-147">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="c68e9-148">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="c68e9-148">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="c68e9-149">TTL</span><span class="sxs-lookup"><span data-stu-id="c68e9-149">ttl</span></span>|<span data-ttu-id="c68e9-150">Int32</span><span class="sxs-lookup"><span data-stu-id="c68e9-150">Int32</span></span>| <span data-ttu-id="c68e9-151">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-151">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="c68e9-152">Não anulável</span><span class="sxs-lookup"><span data-stu-id="c68e9-152">Not nullable</span></span> |
|<span data-ttu-id="c68e9-153">weight</span><span class="sxs-lookup"><span data-stu-id="c68e9-153">weight</span></span>|<span data-ttu-id="c68e9-154">Int32</span><span class="sxs-lookup"><span data-stu-id="c68e9-154">Int32</span></span>| <span data-ttu-id="c68e9-155">O valor a ser usado ao configurar a propriedade *Weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="c68e9-155">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c68e9-156">Relações</span><span class="sxs-lookup"><span data-stu-id="c68e9-156">Relationships</span></span>
<span data-ttu-id="c68e9-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c68e9-157">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="c68e9-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c68e9-158">JSON representation</span></span>
<span data-ttu-id="c68e9-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c68e9-159">Here is a JSON representation of the resource.</span></span>

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
