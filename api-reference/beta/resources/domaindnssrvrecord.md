---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: c06682753b752980530bf8cfd8f6a32b9bbd569a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810434"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="79148-104">Tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="79148-104">domainDnsSrvRecord resource type</span></span>

> <span data-ttu-id="79148-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="79148-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="79148-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="79148-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="79148-p103">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="79148-p103">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="79148-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="79148-109">Methods</span></span>
<span data-ttu-id="79148-p104">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="79148-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="79148-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="79148-112">Properties</span></span>
| <span data-ttu-id="79148-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="79148-113">Property</span></span>     | <span data-ttu-id="79148-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="79148-114">Type</span></span>   |<span data-ttu-id="79148-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="79148-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="79148-116">id</span><span class="sxs-lookup"><span data-stu-id="79148-116">id</span></span>|<span data-ttu-id="79148-117">String</span><span class="sxs-lookup"><span data-stu-id="79148-117">String</span></span>| <span data-ttu-id="79148-p105">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="79148-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="79148-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="79148-120">isOptional</span></span>|<span data-ttu-id="79148-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="79148-121">Boolean</span></span>| <span data-ttu-id="79148-122">Se for falso, o registro SRV deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="79148-122">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="79148-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="79148-123">label</span></span>|<span data-ttu-id="79148-124">String</span><span class="sxs-lookup"><span data-stu-id="79148-124">String</span></span>| <span data-ttu-id="79148-125">O valor usado ao configurar a propriedade *name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-125">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="79148-126">nameTarget</span><span class="sxs-lookup"><span data-stu-id="79148-126">nameTarget</span></span>|<span data-ttu-id="79148-127">String</span><span class="sxs-lookup"><span data-stu-id="79148-127">String</span></span>| <span data-ttu-id="79148-128">O valor a ser usado ao configurar a propriedade *Target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-128">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="79148-129">porta</span><span class="sxs-lookup"><span data-stu-id="79148-129">port</span></span>|<span data-ttu-id="79148-130">Int32</span><span class="sxs-lookup"><span data-stu-id="79148-130">Int32</span></span>| <span data-ttu-id="79148-131">O valor a ser usado ao configurar a propriedade *port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-131">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="79148-132">prioridade</span><span class="sxs-lookup"><span data-stu-id="79148-132">priority</span></span>|<span data-ttu-id="79148-133">Int32</span><span class="sxs-lookup"><span data-stu-id="79148-133">Int32</span></span>| <span data-ttu-id="79148-134">O valor a ser usado ao configurar a propriedade *priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-134">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="79148-135">protocolo</span><span class="sxs-lookup"><span data-stu-id="79148-135">protocol</span></span>|<span data-ttu-id="79148-136">String</span><span class="sxs-lookup"><span data-stu-id="79148-136">String</span></span>| <span data-ttu-id="79148-137">O valor a ser usado ao configurar a propriedade *protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-137">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="79148-138">recordType</span><span class="sxs-lookup"><span data-stu-id="79148-138">recordType</span></span>|<span data-ttu-id="79148-139">String</span><span class="sxs-lookup"><span data-stu-id="79148-139">String</span></span>|  <span data-ttu-id="79148-p106">Tipo do registro DNS. Este valor sempre será *Srv*. Chave</span><span class="sxs-lookup"><span data-stu-id="79148-p106">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="79148-143">service</span><span class="sxs-lookup"><span data-stu-id="79148-143">service</span></span>|<span data-ttu-id="79148-144">String</span><span class="sxs-lookup"><span data-stu-id="79148-144">String</span></span>| <span data-ttu-id="79148-145">O valor a ser usado ao configurar a propriedade *service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-145">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="79148-146">supportedService</span><span class="sxs-lookup"><span data-stu-id="79148-146">supportedService</span></span>|<span data-ttu-id="79148-147">String</span><span class="sxs-lookup"><span data-stu-id="79148-147">String</span></span>| <span data-ttu-id="79148-148">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="79148-148">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="79148-149">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="79148-149">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="79148-150">ttl</span><span class="sxs-lookup"><span data-stu-id="79148-150">ttl</span></span>|<span data-ttu-id="79148-151">Int32</span><span class="sxs-lookup"><span data-stu-id="79148-151">Int32</span></span>| <span data-ttu-id="79148-p107">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="79148-p107">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="79148-154">weight</span><span class="sxs-lookup"><span data-stu-id="79148-154">weight</span></span>|<span data-ttu-id="79148-155">Int32</span><span class="sxs-lookup"><span data-stu-id="79148-155">Int32</span></span>| <span data-ttu-id="79148-156">O valor a ser usado ao configurar a propriedade *weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="79148-156">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="79148-157">Relações</span><span class="sxs-lookup"><span data-stu-id="79148-157">Relationships</span></span>
<span data-ttu-id="79148-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="79148-158">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="79148-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="79148-159">JSON representation</span></span>
<span data-ttu-id="79148-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="79148-160">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsSrvRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
