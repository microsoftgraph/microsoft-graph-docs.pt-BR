---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bdbc2246340d5cd15529dd05101567bc04d1e607
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524475"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="88150-104">Tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="88150-104">domainDnsSrvRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="88150-p102">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="88150-p102">Represents a SRV record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="88150-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="88150-107">Methods</span></span>
<span data-ttu-id="88150-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="88150-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="88150-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="88150-110">Properties</span></span>
| <span data-ttu-id="88150-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="88150-111">Property</span></span>     | <span data-ttu-id="88150-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="88150-112">Type</span></span>   |<span data-ttu-id="88150-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="88150-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="88150-114">id</span><span class="sxs-lookup"><span data-stu-id="88150-114">id</span></span>|<span data-ttu-id="88150-115">String</span><span class="sxs-lookup"><span data-stu-id="88150-115">String</span></span>| <span data-ttu-id="88150-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="88150-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="88150-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="88150-118">isOptional</span></span>|<span data-ttu-id="88150-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="88150-119">Boolean</span></span>| <span data-ttu-id="88150-120">Se for falso, o registro SRV deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="88150-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="88150-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="88150-121">label</span></span>|<span data-ttu-id="88150-122">String</span><span class="sxs-lookup"><span data-stu-id="88150-122">String</span></span>| <span data-ttu-id="88150-123">O valor usado ao configurar a propriedade *name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="88150-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="88150-124">nameTarget</span></span>|<span data-ttu-id="88150-125">String</span><span class="sxs-lookup"><span data-stu-id="88150-125">String</span></span>| <span data-ttu-id="88150-126">O valor a ser usado ao configurar a propriedade *Target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="88150-127">porta</span><span class="sxs-lookup"><span data-stu-id="88150-127">port</span></span>|<span data-ttu-id="88150-128">Int32</span><span class="sxs-lookup"><span data-stu-id="88150-128">Int32</span></span>| <span data-ttu-id="88150-129">O valor a ser usado ao configurar a propriedade *port* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="88150-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="88150-130">priority</span></span>|<span data-ttu-id="88150-131">Int32</span><span class="sxs-lookup"><span data-stu-id="88150-131">Int32</span></span>| <span data-ttu-id="88150-132">O valor a ser usado ao configurar a propriedade *priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="88150-133">protocolo</span><span class="sxs-lookup"><span data-stu-id="88150-133">protocol</span></span>|<span data-ttu-id="88150-134">String</span><span class="sxs-lookup"><span data-stu-id="88150-134">String</span></span>| <span data-ttu-id="88150-135">O valor a ser usado ao configurar a propriedade *protocol* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="88150-136">recordType</span><span class="sxs-lookup"><span data-stu-id="88150-136">recordType</span></span>|<span data-ttu-id="88150-137">String</span><span class="sxs-lookup"><span data-stu-id="88150-137">String</span></span>|  <span data-ttu-id="88150-p105">Tipo do registro DNS. Este valor sempre será *Srv*. Chave</span><span class="sxs-lookup"><span data-stu-id="88150-p105">Type of DNS record. The value is always *Srv*. Key</span></span> |
|<span data-ttu-id="88150-141">service</span><span class="sxs-lookup"><span data-stu-id="88150-141">service</span></span>|<span data-ttu-id="88150-142">String</span><span class="sxs-lookup"><span data-stu-id="88150-142">String</span></span>| <span data-ttu-id="88150-143">O valor a ser usado ao configurar a propriedade *service* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="88150-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="88150-144">supportedService</span></span>|<span data-ttu-id="88150-145">String</span><span class="sxs-lookup"><span data-stu-id="88150-145">String</span></span>| <span data-ttu-id="88150-146">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro SRV.</span><span class="sxs-lookup"><span data-stu-id="88150-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="88150-147">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="88150-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="88150-148">ttl</span><span class="sxs-lookup"><span data-stu-id="88150-148">ttl</span></span>|<span data-ttu-id="88150-149">Int32</span><span class="sxs-lookup"><span data-stu-id="88150-149">Int32</span></span>| <span data-ttu-id="88150-p106">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro SRV no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="88150-p106">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host. Not nullable</span></span> |
|<span data-ttu-id="88150-152">weight</span><span class="sxs-lookup"><span data-stu-id="88150-152">weight</span></span>|<span data-ttu-id="88150-153">Int32</span><span class="sxs-lookup"><span data-stu-id="88150-153">Int32</span></span>| <span data-ttu-id="88150-154">O valor a ser usado ao configurar a propriedade *weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="88150-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="88150-155">Relações</span><span class="sxs-lookup"><span data-stu-id="88150-155">Relationships</span></span>
<span data-ttu-id="88150-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="88150-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="88150-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="88150-157">JSON representation</span></span>
<span data-ttu-id="88150-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="88150-158">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/domaindnssrvrecord.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
