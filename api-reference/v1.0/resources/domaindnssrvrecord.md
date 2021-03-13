---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 7755779218b7120e24cc25f6e0a5a97d4c42db5d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761195"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="6a1ff-103">Tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="6a1ff-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="6a1ff-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a1ff-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6a1ff-105">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="6a1ff-106">Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="6a1ff-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="6a1ff-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6a1ff-107">Methods</span></span>
<span data-ttu-id="6a1ff-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="6a1ff-109">Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="6a1ff-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a1ff-110">Properties</span></span>
| <span data-ttu-id="6a1ff-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a1ff-111">Property</span></span>     | <span data-ttu-id="6a1ff-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a1ff-112">Type</span></span>   |<span data-ttu-id="6a1ff-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a1ff-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a1ff-114">id</span><span class="sxs-lookup"><span data-stu-id="6a1ff-114">id</span></span>|<span data-ttu-id="6a1ff-115">String</span><span class="sxs-lookup"><span data-stu-id="6a1ff-115">String</span></span>| <span data-ttu-id="6a1ff-116">Identificador exclusivo atribuído a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="6a1ff-117">Não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="6a1ff-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="6a1ff-118">isOptional</span></span>|<span data-ttu-id="6a1ff-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="6a1ff-119">Boolean</span></span>| <span data-ttu-id="6a1ff-120">Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS para Microsoft Online Services funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="6a1ff-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="6a1ff-121">label</span></span>|<span data-ttu-id="6a1ff-122">String</span><span class="sxs-lookup"><span data-stu-id="6a1ff-122">String</span></span>| <span data-ttu-id="6a1ff-123">Valor usado ao configurar a *propriedade name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="6a1ff-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="6a1ff-124">nameTarget</span></span>|<span data-ttu-id="6a1ff-125">String</span><span class="sxs-lookup"><span data-stu-id="6a1ff-125">String</span></span>| <span data-ttu-id="6a1ff-126">Valor a ser usado ao configurar a *propriedade Target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="6a1ff-127">port</span><span class="sxs-lookup"><span data-stu-id="6a1ff-127">port</span></span>|<span data-ttu-id="6a1ff-128">Int32</span><span class="sxs-lookup"><span data-stu-id="6a1ff-128">Int32</span></span>| <span data-ttu-id="6a1ff-129">Valor a ser usado ao configurar a *propriedade de* porta do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="6a1ff-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="6a1ff-130">priority</span></span>|<span data-ttu-id="6a1ff-131">Int32</span><span class="sxs-lookup"><span data-stu-id="6a1ff-131">Int32</span></span>| <span data-ttu-id="6a1ff-132">Valor a ser usado ao configurar a *propriedade priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="6a1ff-133">protocol</span><span class="sxs-lookup"><span data-stu-id="6a1ff-133">protocol</span></span>|<span data-ttu-id="6a1ff-134">String</span><span class="sxs-lookup"><span data-stu-id="6a1ff-134">String</span></span>| <span data-ttu-id="6a1ff-135">Valor a ser usado ao configurar a propriedade *de* protocolo do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="6a1ff-136">recordType</span><span class="sxs-lookup"><span data-stu-id="6a1ff-136">recordType</span></span>|<span data-ttu-id="6a1ff-137">String</span><span class="sxs-lookup"><span data-stu-id="6a1ff-137">String</span></span>|  <span data-ttu-id="6a1ff-138">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-138">Type of DNS record.</span></span> <span data-ttu-id="6a1ff-139">O valor é sempre *Srv*.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-139">The value is always *Srv*.</span></span> <span data-ttu-id="6a1ff-140">Chave</span><span class="sxs-lookup"><span data-stu-id="6a1ff-140">Key</span></span> |
|<span data-ttu-id="6a1ff-141">service</span><span class="sxs-lookup"><span data-stu-id="6a1ff-141">service</span></span>|<span data-ttu-id="6a1ff-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a1ff-142">String</span></span>| <span data-ttu-id="6a1ff-143">Valor a ser usado ao configurar a propriedade *de* serviço do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="6a1ff-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="6a1ff-144">supportedService</span></span>|<span data-ttu-id="6a1ff-145">String</span><span class="sxs-lookup"><span data-stu-id="6a1ff-145">String</span></span>| <span data-ttu-id="6a1ff-146">Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro SRV.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="6a1ff-147">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="6a1ff-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="6a1ff-148">ttl</span><span class="sxs-lookup"><span data-stu-id="6a1ff-148">ttl</span></span>|<span data-ttu-id="6a1ff-149">Int32</span><span class="sxs-lookup"><span data-stu-id="6a1ff-149">Int32</span></span>| <span data-ttu-id="6a1ff-150">Valor a ser usado ao configurar a *propriedade time-to-live (ttl)* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="6a1ff-151">Não anulada</span><span class="sxs-lookup"><span data-stu-id="6a1ff-151">Not nullable</span></span> |
|<span data-ttu-id="6a1ff-152">weight</span><span class="sxs-lookup"><span data-stu-id="6a1ff-152">weight</span></span>|<span data-ttu-id="6a1ff-153">Int32</span><span class="sxs-lookup"><span data-stu-id="6a1ff-153">Int32</span></span>| <span data-ttu-id="6a1ff-154">Valor a ser usado ao configurar a *propriedade weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6a1ff-155">Relações</span><span class="sxs-lookup"><span data-stu-id="6a1ff-155">Relationships</span></span>
<span data-ttu-id="6a1ff-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a1ff-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6a1ff-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a1ff-157">JSON representation</span></span>
<span data-ttu-id="6a1ff-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a1ff-158">Here is a JSON representation of the resource.</span></span>

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

