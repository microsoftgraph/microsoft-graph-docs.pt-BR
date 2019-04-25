---
title: tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f270075556843625d1ec408f06be8ed4a065c831
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543186"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="0c263-104">tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="0c263-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="0c263-105">Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="0c263-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="0c263-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="0c263-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="0c263-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="0c263-107">Methods</span></span>
<span data-ttu-id="0c263-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="0c263-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="0c263-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="0c263-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="0c263-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0c263-110">Properties</span></span>
| <span data-ttu-id="0c263-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0c263-111">Property</span></span>     | <span data-ttu-id="0c263-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="0c263-112">Type</span></span>   |<span data-ttu-id="0c263-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="0c263-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c263-114">canônicaname</span><span class="sxs-lookup"><span data-stu-id="0c263-114">canonicalName</span></span>|<span data-ttu-id="0c263-115">String</span><span class="sxs-lookup"><span data-stu-id="0c263-115">String</span></span>| <span data-ttu-id="0c263-116">O nome canônico do registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="0c263-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="0c263-117">Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="0c263-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="0c263-118">id</span><span class="sxs-lookup"><span data-stu-id="0c263-118">id</span></span>|<span data-ttu-id="0c263-119">String</span><span class="sxs-lookup"><span data-stu-id="0c263-119">String</span></span>| <span data-ttu-id="0c263-120">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="0c263-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="0c263-121">Não anulável, somente leitura</span><span class="sxs-lookup"><span data-stu-id="0c263-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="0c263-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="0c263-122">isOptional</span></span>|<span data-ttu-id="0c263-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="0c263-123">Boolean</span></span>| <span data-ttu-id="0c263-124">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="0c263-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="0c263-125">Não anulável</span><span class="sxs-lookup"><span data-stu-id="0c263-125">Not nullable</span></span> |
|<span data-ttu-id="0c263-126">rótulo</span><span class="sxs-lookup"><span data-stu-id="0c263-126">label</span></span>|<span data-ttu-id="0c263-127">String</span><span class="sxs-lookup"><span data-stu-id="0c263-127">String</span></span>| <span data-ttu-id="0c263-128">O valor usado ao configurar o *alias/host/nome* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="0c263-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="0c263-129">recordType</span><span class="sxs-lookup"><span data-stu-id="0c263-129">recordType</span></span>|<span data-ttu-id="0c263-130">String</span><span class="sxs-lookup"><span data-stu-id="0c263-130">String</span></span>| <span data-ttu-id="0c263-131">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="0c263-131">Type of DNS record.</span></span> <span data-ttu-id="0c263-132">O valor é sempre *CNAME*.</span><span class="sxs-lookup"><span data-stu-id="0c263-132">The value is always *CName*.</span></span> <span data-ttu-id="0c263-133">Chave</span><span class="sxs-lookup"><span data-stu-id="0c263-133">Key</span></span>|
|<span data-ttu-id="0c263-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="0c263-134">supportedService</span></span>|<span data-ttu-id="0c263-135">String</span><span class="sxs-lookup"><span data-stu-id="0c263-135">String</span></span>| <span data-ttu-id="0c263-136">O Microsoft Online Services ou o recurso que tem uma dependência neste registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="0c263-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="0c263-137">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="0c263-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="0c263-138">TTL</span><span class="sxs-lookup"><span data-stu-id="0c263-138">ttl</span></span>|<span data-ttu-id="0c263-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0c263-139">Int32</span></span>| <span data-ttu-id="0c263-140">O valor a ser usado ao configurar a propriedade TTL (time-to-Live) do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="0c263-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="0c263-141">Não anulável</span><span class="sxs-lookup"><span data-stu-id="0c263-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="0c263-142">Relações</span><span class="sxs-lookup"><span data-stu-id="0c263-142">Relationships</span></span>
<span data-ttu-id="0c263-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0c263-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="0c263-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0c263-144">JSON representation</span></span>
<span data-ttu-id="0c263-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0c263-145">Here is a JSON representation of the resource.</span></span>

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
