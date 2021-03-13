---
title: Tipo de recurso domainDnsSrvRecord
description: Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 5b3355115f11937584879725073cd4a4c279c62d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761671"
---
# <a name="domaindnssrvrecord-resource-type"></a><span data-ttu-id="ead12-103">Tipo de recurso domainDnsSrvRecord</span><span class="sxs-lookup"><span data-stu-id="ead12-103">domainDnsSrvRecord resource type</span></span>

<span data-ttu-id="ead12-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ead12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ead12-105">Representa um registro SRV adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="ead12-105">Represents a SRV record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="ead12-106">Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="ead12-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="ead12-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="ead12-107">Methods</span></span>
<span data-ttu-id="ead12-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="ead12-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="ead12-109">Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="ead12-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="ead12-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ead12-110">Properties</span></span>
| <span data-ttu-id="ead12-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ead12-111">Property</span></span>     | <span data-ttu-id="ead12-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="ead12-112">Type</span></span>   |<span data-ttu-id="ead12-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="ead12-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ead12-114">id</span><span class="sxs-lookup"><span data-stu-id="ead12-114">id</span></span>|<span data-ttu-id="ead12-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-115">String</span></span>| <span data-ttu-id="ead12-116">Identificador exclusivo atribuído a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="ead12-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="ead12-117">Não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="ead12-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="ead12-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="ead12-118">isOptional</span></span>|<span data-ttu-id="ead12-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="ead12-119">Boolean</span></span>| <span data-ttu-id="ead12-120">Se for falso, o registro SRV deverá ser configurado pelo cliente no host DNS para Microsoft Online Services funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="ead12-120">If false, the SRV record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="ead12-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="ead12-121">label</span></span>|<span data-ttu-id="ead12-122">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-122">String</span></span>| <span data-ttu-id="ead12-123">Valor usado ao configurar a *propriedade name* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-123">Value used when configuring the *name* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="ead12-124">nameTarget</span><span class="sxs-lookup"><span data-stu-id="ead12-124">nameTarget</span></span>|<span data-ttu-id="ead12-125">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-125">String</span></span>| <span data-ttu-id="ead12-126">Valor a ser usado ao configurar a *propriedade Target* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-126">Value to use when configuring the *Target* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="ead12-127">port</span><span class="sxs-lookup"><span data-stu-id="ead12-127">port</span></span>|<span data-ttu-id="ead12-128">Int32</span><span class="sxs-lookup"><span data-stu-id="ead12-128">Int32</span></span>| <span data-ttu-id="ead12-129">Valor a ser usado ao configurar a *propriedade de* porta do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-129">Value to use when configuring the *port* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="ead12-130">prioridade</span><span class="sxs-lookup"><span data-stu-id="ead12-130">priority</span></span>|<span data-ttu-id="ead12-131">Int32</span><span class="sxs-lookup"><span data-stu-id="ead12-131">Int32</span></span>| <span data-ttu-id="ead12-132">Valor a ser usado ao configurar a *propriedade priority* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-132">Value to use when configuring the *priority* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="ead12-133">protocol</span><span class="sxs-lookup"><span data-stu-id="ead12-133">protocol</span></span>|<span data-ttu-id="ead12-134">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-134">String</span></span>| <span data-ttu-id="ead12-135">Valor a ser usado ao configurar a propriedade *de* protocolo do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-135">Value to use when configuring the *protocol* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="ead12-136">recordType</span><span class="sxs-lookup"><span data-stu-id="ead12-136">recordType</span></span>|<span data-ttu-id="ead12-137">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-137">String</span></span>|  <span data-ttu-id="ead12-138">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-138">Type of DNS record.</span></span> <span data-ttu-id="ead12-139">O valor é sempre *Srv*.</span><span class="sxs-lookup"><span data-stu-id="ead12-139">The value is always *Srv*.</span></span> <span data-ttu-id="ead12-140">Chave</span><span class="sxs-lookup"><span data-stu-id="ead12-140">Key</span></span> |
|<span data-ttu-id="ead12-141">service</span><span class="sxs-lookup"><span data-stu-id="ead12-141">service</span></span>|<span data-ttu-id="ead12-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-142">String</span></span>| <span data-ttu-id="ead12-143">Valor a ser usado ao configurar a propriedade *de* serviço do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-143">Value to use when configuring the *service* property of the SRV record at the DNS host.</span></span> |
|<span data-ttu-id="ead12-144">supportedService</span><span class="sxs-lookup"><span data-stu-id="ead12-144">supportedService</span></span>|<span data-ttu-id="ead12-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="ead12-145">String</span></span>| <span data-ttu-id="ead12-146">Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro SRV.</span><span class="sxs-lookup"><span data-stu-id="ead12-146">Microsoft Online Service or feature that has a dependency on this SRV record.</span></span></br></br><span data-ttu-id="ead12-147">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="ead12-147">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="ead12-148">ttl</span><span class="sxs-lookup"><span data-stu-id="ead12-148">ttl</span></span>|<span data-ttu-id="ead12-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ead12-149">Int32</span></span>| <span data-ttu-id="ead12-150">Valor a ser usado ao configurar a *propriedade time-to-live (ttl)* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-150">Value to use when configuring the *time-to-live (ttl)* property of the SRV record at the DNS host.</span></span> <span data-ttu-id="ead12-151">Não anulada</span><span class="sxs-lookup"><span data-stu-id="ead12-151">Not nullable</span></span> |
|<span data-ttu-id="ead12-152">weight</span><span class="sxs-lookup"><span data-stu-id="ead12-152">weight</span></span>|<span data-ttu-id="ead12-153">Int32</span><span class="sxs-lookup"><span data-stu-id="ead12-153">Int32</span></span>| <span data-ttu-id="ead12-154">Valor a ser usado ao configurar a *propriedade weight* do registro SRV no host DNS.</span><span class="sxs-lookup"><span data-stu-id="ead12-154">Value to use when configuring the *weight* property of the SRV record at the DNS host.</span></span> |

## <a name="relationships"></a><span data-ttu-id="ead12-155">Relações</span><span class="sxs-lookup"><span data-stu-id="ead12-155">Relationships</span></span>
<span data-ttu-id="ead12-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ead12-156">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="ead12-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ead12-157">JSON representation</span></span>
<span data-ttu-id="ead12-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ead12-158">Here is a JSON representation of the resource.</span></span>

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


