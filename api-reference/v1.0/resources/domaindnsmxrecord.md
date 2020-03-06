---
title: tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d0c7324f5c0760ff62cb3b835f7e011dd8a0a5a2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531605"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="b6ba6-104">tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="b6ba6-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="b6ba6-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6ba6-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b6ba6-106">Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-106">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="b6ba6-107">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="b6ba6-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b6ba6-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b6ba6-108">Methods</span></span>
<span data-ttu-id="b6ba6-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="b6ba6-110">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b6ba6-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b6ba6-111">Properties</span></span>
| <span data-ttu-id="b6ba6-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b6ba6-112">Property</span></span>     | <span data-ttu-id="b6ba6-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="b6ba6-113">Type</span></span>   |<span data-ttu-id="b6ba6-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="b6ba6-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6ba6-115">id</span><span class="sxs-lookup"><span data-stu-id="b6ba6-115">id</span></span>|<span data-ttu-id="b6ba6-116">String</span><span class="sxs-lookup"><span data-stu-id="b6ba6-116">String</span></span>| <span data-ttu-id="b6ba6-117">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="b6ba6-118">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-118">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="b6ba6-119">IsOptional</span><span class="sxs-lookup"><span data-stu-id="b6ba6-119">isOptional</span></span>|<span data-ttu-id="b6ba6-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="b6ba6-120">Boolean</span></span>| <span data-ttu-id="b6ba6-121">Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-121">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b6ba6-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="b6ba6-122">label</span></span>|<span data-ttu-id="b6ba6-123">String</span><span class="sxs-lookup"><span data-stu-id="b6ba6-123">String</span></span>| <span data-ttu-id="b6ba6-124">O valor usado ao configurar a propriedade *alias/Host/Name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-124">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="b6ba6-125">mailExchange</span><span class="sxs-lookup"><span data-stu-id="b6ba6-125">mailExchange</span></span>|<span data-ttu-id="b6ba6-126">String</span><span class="sxs-lookup"><span data-stu-id="b6ba6-126">String</span></span>| <span data-ttu-id="b6ba6-127">O valor usado ao configurar a *resposta/destino/valor* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-127">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="b6ba6-128">preferência</span><span class="sxs-lookup"><span data-stu-id="b6ba6-128">preference</span></span>|<span data-ttu-id="b6ba6-129">Int32</span><span class="sxs-lookup"><span data-stu-id="b6ba6-129">Int32</span></span>| <span data-ttu-id="b6ba6-130">O valor usado ao configurar a propriedade *preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-130">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="b6ba6-131">recordType</span><span class="sxs-lookup"><span data-stu-id="b6ba6-131">recordType</span></span>|<span data-ttu-id="b6ba6-132">String</span><span class="sxs-lookup"><span data-stu-id="b6ba6-132">String</span></span>| <span data-ttu-id="b6ba6-133">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-133">Type of DNS record.</span></span> <span data-ttu-id="b6ba6-134">O valor é sempre *MX*.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-134">The value is always *Mx*.</span></span> <span data-ttu-id="b6ba6-135">Chave</span><span class="sxs-lookup"><span data-stu-id="b6ba6-135">Key</span></span> |
|<span data-ttu-id="b6ba6-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="b6ba6-136">supportedService</span></span>|<span data-ttu-id="b6ba6-137">String</span><span class="sxs-lookup"><span data-stu-id="b6ba6-137">String</span></span>| <span data-ttu-id="b6ba6-138">O Microsoft Online Services ou o recurso que tem uma dependência neste registro MX.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-138">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="b6ba6-139">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="b6ba6-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b6ba6-140">TTL</span><span class="sxs-lookup"><span data-stu-id="b6ba6-140">ttl</span></span>|<span data-ttu-id="b6ba6-141">Int32</span><span class="sxs-lookup"><span data-stu-id="b6ba6-141">Int32</span></span>| <span data-ttu-id="b6ba6-142">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-142">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="b6ba6-143">Não anulável</span><span class="sxs-lookup"><span data-stu-id="b6ba6-143">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="b6ba6-144">Relações</span><span class="sxs-lookup"><span data-stu-id="b6ba6-144">Relationships</span></span>
<span data-ttu-id="b6ba6-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b6ba6-145">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b6ba6-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b6ba6-146">JSON representation</span></span>
<span data-ttu-id="b6ba6-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b6ba6-147">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "mailExchange": "String",
  "preference": 1024,
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsMxRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
