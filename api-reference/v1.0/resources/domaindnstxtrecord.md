---
title: tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8694a0a64926f545dcc7ab5e8251961e53638c62
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657613"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="1af2f-104">tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="1af2f-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="1af2f-105">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="1af2f-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="1af2f-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="1af2f-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="1af2f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1af2f-107">Methods</span></span>
<span data-ttu-id="1af2f-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="1af2f-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="1af2f-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="1af2f-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="1af2f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1af2f-110">Properties</span></span>
| <span data-ttu-id="1af2f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1af2f-111">Property</span></span>     | <span data-ttu-id="1af2f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="1af2f-112">Type</span></span>   |<span data-ttu-id="1af2f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="1af2f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1af2f-114">id</span><span class="sxs-lookup"><span data-stu-id="1af2f-114">id</span></span>|<span data-ttu-id="1af2f-115">String</span><span class="sxs-lookup"><span data-stu-id="1af2f-115">String</span></span>| <span data-ttu-id="1af2f-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="1af2f-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="1af2f-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="1af2f-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="1af2f-118">IsOptional</span><span class="sxs-lookup"><span data-stu-id="1af2f-118">isOptional</span></span>|<span data-ttu-id="1af2f-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="1af2f-119">Boolean</span></span>| <span data-ttu-id="1af2f-120">Se for falso, o registro TXT deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="1af2f-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="1af2f-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="1af2f-121">label</span></span>|<span data-ttu-id="1af2f-122">String</span><span class="sxs-lookup"><span data-stu-id="1af2f-122">String</span></span>| <span data-ttu-id="1af2f-123">O valor a ser usado ao configurar a propriedade *Name* do registro txt no host DNS.</span><span class="sxs-lookup"><span data-stu-id="1af2f-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="1af2f-124">recordType</span><span class="sxs-lookup"><span data-stu-id="1af2f-124">recordType</span></span>|<span data-ttu-id="1af2f-125">String</span><span class="sxs-lookup"><span data-stu-id="1af2f-125">String</span></span>| <span data-ttu-id="1af2f-126">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="1af2f-126">Type of DNS record.</span></span> <span data-ttu-id="1af2f-127">O valor é sempre *txt*.</span><span class="sxs-lookup"><span data-stu-id="1af2f-127">The value is always *Txt*.</span></span> <span data-ttu-id="1af2f-128">Chave</span><span class="sxs-lookup"><span data-stu-id="1af2f-128">Key</span></span> |
|<span data-ttu-id="1af2f-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="1af2f-129">supportedService</span></span>|<span data-ttu-id="1af2f-130">String</span><span class="sxs-lookup"><span data-stu-id="1af2f-130">String</span></span>| <span data-ttu-id="1af2f-131">O Microsoft Online Services ou o recurso que tem uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="1af2f-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="1af2f-132">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="1af2f-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="1af2f-133">texto</span><span class="sxs-lookup"><span data-stu-id="1af2f-133">text</span></span>|<span data-ttu-id="1af2f-134">String</span><span class="sxs-lookup"><span data-stu-id="1af2f-134">String</span></span>| <span data-ttu-id="1af2f-135">O valor usado ao configurar a propriedade *Text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="1af2f-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="1af2f-136">TTL</span><span class="sxs-lookup"><span data-stu-id="1af2f-136">ttl</span></span>|<span data-ttu-id="1af2f-137">Int32</span><span class="sxs-lookup"><span data-stu-id="1af2f-137">Int32</span></span>| <span data-ttu-id="1af2f-138">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="1af2f-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="1af2f-139">Não anulável</span><span class="sxs-lookup"><span data-stu-id="1af2f-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="1af2f-140">Relações</span><span class="sxs-lookup"><span data-stu-id="1af2f-140">Relationships</span></span>
<span data-ttu-id="1af2f-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1af2f-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="1af2f-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1af2f-142">JSON representation</span></span>
<span data-ttu-id="1af2f-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1af2f-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "id": "String (identifier)",
  "isOptional": true,
  "label": "String",
  "recordType": "String",
  "supportedService": "String",
  "text": "String",
  "ttl": 1024
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
