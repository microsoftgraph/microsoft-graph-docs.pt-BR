---
title: tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 1d837ce660ebceda300d63d428b92836b3173fba
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032659"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="e80ba-104">tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="e80ba-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="e80ba-105">Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="e80ba-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="e80ba-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="e80ba-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="e80ba-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e80ba-107">Methods</span></span>
<span data-ttu-id="e80ba-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="e80ba-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="e80ba-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="e80ba-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="e80ba-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e80ba-110">Properties</span></span>
| <span data-ttu-id="e80ba-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e80ba-111">Property</span></span>     | <span data-ttu-id="e80ba-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="e80ba-112">Type</span></span>   |<span data-ttu-id="e80ba-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="e80ba-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e80ba-114">id</span><span class="sxs-lookup"><span data-stu-id="e80ba-114">id</span></span>|<span data-ttu-id="e80ba-115">String</span><span class="sxs-lookup"><span data-stu-id="e80ba-115">String</span></span>| <span data-ttu-id="e80ba-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="e80ba-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="e80ba-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e80ba-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="e80ba-118">IsOptional</span><span class="sxs-lookup"><span data-stu-id="e80ba-118">isOptional</span></span>|<span data-ttu-id="e80ba-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="e80ba-119">Boolean</span></span>| <span data-ttu-id="e80ba-120">Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="e80ba-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="e80ba-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="e80ba-121">label</span></span>|<span data-ttu-id="e80ba-122">String</span><span class="sxs-lookup"><span data-stu-id="e80ba-122">String</span></span>| <span data-ttu-id="e80ba-123">O valor usado ao configurar a propriedade *alias/Host/Name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="e80ba-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="e80ba-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="e80ba-124">mailExchange</span></span>|<span data-ttu-id="e80ba-125">String</span><span class="sxs-lookup"><span data-stu-id="e80ba-125">String</span></span>| <span data-ttu-id="e80ba-126">O valor usado ao configurar a *resposta/destino/valor* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="e80ba-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="e80ba-127">preferência</span><span class="sxs-lookup"><span data-stu-id="e80ba-127">preference</span></span>|<span data-ttu-id="e80ba-128">Int32</span><span class="sxs-lookup"><span data-stu-id="e80ba-128">Int32</span></span>| <span data-ttu-id="e80ba-129">O valor usado ao configurar a propriedade *preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="e80ba-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="e80ba-130">recordType</span><span class="sxs-lookup"><span data-stu-id="e80ba-130">recordType</span></span>|<span data-ttu-id="e80ba-131">String</span><span class="sxs-lookup"><span data-stu-id="e80ba-131">String</span></span>| <span data-ttu-id="e80ba-132">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="e80ba-132">Type of DNS record.</span></span> <span data-ttu-id="e80ba-133">O valor é sempre *MX*.</span><span class="sxs-lookup"><span data-stu-id="e80ba-133">The value is always *Mx*.</span></span> <span data-ttu-id="e80ba-134">Chave</span><span class="sxs-lookup"><span data-stu-id="e80ba-134">Key</span></span> |
|<span data-ttu-id="e80ba-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="e80ba-135">supportedService</span></span>|<span data-ttu-id="e80ba-136">String</span><span class="sxs-lookup"><span data-stu-id="e80ba-136">String</span></span>| <span data-ttu-id="e80ba-137">O Microsoft Online Services ou o recurso que tem uma dependência neste registro MX.</span><span class="sxs-lookup"><span data-stu-id="e80ba-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="e80ba-138">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="e80ba-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="e80ba-139">TTL</span><span class="sxs-lookup"><span data-stu-id="e80ba-139">ttl</span></span>|<span data-ttu-id="e80ba-140">Int32</span><span class="sxs-lookup"><span data-stu-id="e80ba-140">Int32</span></span>| <span data-ttu-id="e80ba-141">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="e80ba-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="e80ba-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="e80ba-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="e80ba-143">Relações</span><span class="sxs-lookup"><span data-stu-id="e80ba-143">Relationships</span></span>
<span data-ttu-id="e80ba-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e80ba-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e80ba-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e80ba-145">JSON representation</span></span>
<span data-ttu-id="e80ba-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e80ba-146">Here is a JSON representation of the resource.</span></span>

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
