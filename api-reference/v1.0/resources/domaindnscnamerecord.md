---
title: tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9d2182ed121dbf303e3f9982c53655cecb6f4c10
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48091716"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="3f324-103">tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="3f324-103">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="3f324-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f324-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f324-105">Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="3f324-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="3f324-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="3f324-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="3f324-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3f324-107">Methods</span></span>
<span data-ttu-id="3f324-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="3f324-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="3f324-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="3f324-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="3f324-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f324-110">Properties</span></span>
| <span data-ttu-id="3f324-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f324-111">Property</span></span>     | <span data-ttu-id="3f324-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f324-112">Type</span></span>   |<span data-ttu-id="3f324-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f324-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3f324-114">canônicaname</span><span class="sxs-lookup"><span data-stu-id="3f324-114">canonicalName</span></span>|<span data-ttu-id="3f324-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f324-115">String</span></span>| <span data-ttu-id="3f324-116">O nome canônico do registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="3f324-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="3f324-117">Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="3f324-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3f324-118">id</span><span class="sxs-lookup"><span data-stu-id="3f324-118">id</span></span>|<span data-ttu-id="3f324-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f324-119">String</span></span>| <span data-ttu-id="3f324-120">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="3f324-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="3f324-121">Não anulável, somente leitura</span><span class="sxs-lookup"><span data-stu-id="3f324-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="3f324-122">IsOptional</span><span class="sxs-lookup"><span data-stu-id="3f324-122">isOptional</span></span>|<span data-ttu-id="3f324-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="3f324-123">Boolean</span></span>| <span data-ttu-id="3f324-124">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="3f324-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="3f324-125">Não anulável</span><span class="sxs-lookup"><span data-stu-id="3f324-125">Not nullable</span></span> |
|<span data-ttu-id="3f324-126">rótulo</span><span class="sxs-lookup"><span data-stu-id="3f324-126">label</span></span>|<span data-ttu-id="3f324-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f324-127">String</span></span>| <span data-ttu-id="3f324-128">O valor usado ao configurar o *alias/host/nome* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="3f324-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3f324-129">recordType</span><span class="sxs-lookup"><span data-stu-id="3f324-129">recordType</span></span>|<span data-ttu-id="3f324-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f324-130">String</span></span>| <span data-ttu-id="3f324-131">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="3f324-131">Type of DNS record.</span></span> <span data-ttu-id="3f324-132">O valor é sempre *CNAME*.</span><span class="sxs-lookup"><span data-stu-id="3f324-132">The value is always *CName*.</span></span> <span data-ttu-id="3f324-133">Chave</span><span class="sxs-lookup"><span data-stu-id="3f324-133">Key</span></span>|
|<span data-ttu-id="3f324-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="3f324-134">supportedService</span></span>|<span data-ttu-id="3f324-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3f324-135">String</span></span>| <span data-ttu-id="3f324-136">O Microsoft Online Services ou o recurso que tem uma dependência neste registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="3f324-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="3f324-137">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="3f324-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="3f324-138">TTL</span><span class="sxs-lookup"><span data-stu-id="3f324-138">ttl</span></span>|<span data-ttu-id="3f324-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3f324-139">Int32</span></span>| <span data-ttu-id="3f324-140">O valor a ser usado ao configurar a propriedade TTL (time-to-Live) do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="3f324-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="3f324-141">Não anulável</span><span class="sxs-lookup"><span data-stu-id="3f324-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="3f324-142">Relações</span><span class="sxs-lookup"><span data-stu-id="3f324-142">Relationships</span></span>
<span data-ttu-id="3f324-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f324-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3f324-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f324-144">JSON representation</span></span>
<span data-ttu-id="3f324-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f324-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsCnameRecord"
}-->

```json
{
  "canonicalName": "String",
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

