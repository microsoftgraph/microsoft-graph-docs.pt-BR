---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: d8fbdb6a99e2a4c88b38d350ace3976842eb7f92
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318820"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="5fe65-104">Tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="5fe65-104">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="5fe65-p102">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="5fe65-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="5fe65-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5fe65-107">Methods</span></span>
<span data-ttu-id="5fe65-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="5fe65-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="5fe65-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5fe65-110">Properties</span></span>
| <span data-ttu-id="5fe65-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5fe65-111">Property</span></span>     | <span data-ttu-id="5fe65-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="5fe65-112">Type</span></span>   |<span data-ttu-id="5fe65-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fe65-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5fe65-114">id</span><span class="sxs-lookup"><span data-stu-id="5fe65-114">id</span></span>|<span data-ttu-id="5fe65-115">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-115">String</span></span>| <span data-ttu-id="5fe65-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="5fe65-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="5fe65-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="5fe65-118">isOptional</span></span>|<span data-ttu-id="5fe65-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="5fe65-119">Boolean</span></span>| <span data-ttu-id="5fe65-120">Se for falso, o registro SRV deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="5fe65-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="5fe65-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="5fe65-121">label</span></span>|<span data-ttu-id="5fe65-122">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-122">String</span></span>| <span data-ttu-id="5fe65-123">O valor usado ao configurar a propriedade *name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5fe65-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="5fe65-124">nameTarget</span></span>|<span data-ttu-id="5fe65-125">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-125">String</span></span>| <span data-ttu-id="5fe65-126">O valor a ser usado ao configurar a propriedade *Target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5fe65-127">porta</span><span class="sxs-lookup"><span data-stu-id="5fe65-127">port</span></span>|<span data-ttu-id="5fe65-128">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe65-128">Int32</span></span>| <span data-ttu-id="5fe65-129">O valor a ser usado ao configurar a propriedade *port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5fe65-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="5fe65-130">priority</span></span>|<span data-ttu-id="5fe65-131">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe65-131">Int32</span></span>| <span data-ttu-id="5fe65-132">O valor a ser usado ao configurar a propriedade *priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5fe65-133">protocolo</span><span class="sxs-lookup"><span data-stu-id="5fe65-133">protocol</span></span>|<span data-ttu-id="5fe65-134">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-134">String</span></span>| <span data-ttu-id="5fe65-135">O valor a ser usado ao configurar a propriedade *protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5fe65-136">recordType</span><span class="sxs-lookup"><span data-stu-id="5fe65-136">recordType</span></span>|<span data-ttu-id="5fe65-137">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-137">String</span></span>|  <span data-ttu-id="5fe65-p105">Tipo do registro DNS. Este valor sempre será *Srv*. Chave</span><span class="sxs-lookup"><span data-stu-id="5fe65-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="5fe65-141">service</span><span class="sxs-lookup"><span data-stu-id="5fe65-141">service</span></span>|<span data-ttu-id="5fe65-142">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-142">String</span></span>| <span data-ttu-id="5fe65-143">O valor a ser usado ao configurar a propriedade *service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="5fe65-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="5fe65-144">supportedService</span></span>|<span data-ttu-id="5fe65-145">String</span><span class="sxs-lookup"><span data-stu-id="5fe65-145">String</span></span>| <span data-ttu-id="5fe65-146">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="5fe65-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="5fe65-147">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="5fe65-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="5fe65-148">ttl</span><span class="sxs-lookup"><span data-stu-id="5fe65-148">ttl</span></span>|<span data-ttu-id="5fe65-149">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe65-149">Int32</span></span>| <span data-ttu-id="5fe65-p106">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="5fe65-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="5fe65-152">weight</span><span class="sxs-lookup"><span data-stu-id="5fe65-152">weight</span></span>|<span data-ttu-id="5fe65-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5fe65-153">Int32</span></span>| <span data-ttu-id="5fe65-154">O valor a ser usado ao configurar a propriedade *weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="5fe65-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="5fe65-155">Relações</span><span class="sxs-lookup"><span data-stu-id="5fe65-155">Relationships</span></span>
<span data-ttu-id="5fe65-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5fe65-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5fe65-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5fe65-157">JSON representation</span></span>
<span data-ttu-id="5fe65-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5fe65-158">Here is a JSON representation of the resource.</span></span>

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