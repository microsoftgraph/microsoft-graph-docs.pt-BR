---
title: tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4bdcddc0ec81d8a7fc76e2113155fdc7ee871161
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543137"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="8442c-104">tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="8442c-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="8442c-105">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="8442c-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="8442c-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="8442c-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="8442c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="8442c-107">Methods</span></span>
<span data-ttu-id="8442c-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="8442c-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="8442c-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="8442c-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="8442c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8442c-110">Properties</span></span>
| <span data-ttu-id="8442c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8442c-111">Property</span></span>     | <span data-ttu-id="8442c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="8442c-112">Type</span></span>   |<span data-ttu-id="8442c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="8442c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8442c-114">id</span><span class="sxs-lookup"><span data-stu-id="8442c-114">id</span></span>|<span data-ttu-id="8442c-115">String</span><span class="sxs-lookup"><span data-stu-id="8442c-115">String</span></span>| <span data-ttu-id="8442c-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="8442c-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="8442c-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8442c-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="8442c-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="8442c-118">isOptional</span></span>|<span data-ttu-id="8442c-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="8442c-119">Boolean</span></span>| <span data-ttu-id="8442c-120">Se for falso, o registro TXT deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="8442c-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="8442c-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="8442c-121">label</span></span>|<span data-ttu-id="8442c-122">String</span><span class="sxs-lookup"><span data-stu-id="8442c-122">String</span></span>| <span data-ttu-id="8442c-123">O valor a ser usado ao configurar a propriedade *Name* do registro txt no host DNS.</span><span class="sxs-lookup"><span data-stu-id="8442c-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="8442c-124">recordType</span><span class="sxs-lookup"><span data-stu-id="8442c-124">recordType</span></span>|<span data-ttu-id="8442c-125">String</span><span class="sxs-lookup"><span data-stu-id="8442c-125">String</span></span>| <span data-ttu-id="8442c-126">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="8442c-126">Type of DNS record.</span></span> <span data-ttu-id="8442c-127">O valor é sempre *txt*.</span><span class="sxs-lookup"><span data-stu-id="8442c-127">The value is always *Txt*.</span></span> <span data-ttu-id="8442c-128">Chave</span><span class="sxs-lookup"><span data-stu-id="8442c-128">Key</span></span> |
|<span data-ttu-id="8442c-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="8442c-129">supportedService</span></span>|<span data-ttu-id="8442c-130">String</span><span class="sxs-lookup"><span data-stu-id="8442c-130">String</span></span>| <span data-ttu-id="8442c-131">O Microsoft Online Services ou o recurso que tem uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="8442c-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="8442c-132">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="8442c-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="8442c-133">texto</span><span class="sxs-lookup"><span data-stu-id="8442c-133">text</span></span>|<span data-ttu-id="8442c-134">String</span><span class="sxs-lookup"><span data-stu-id="8442c-134">String</span></span>| <span data-ttu-id="8442c-135">O valor usado ao configurar a propriedade *Text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="8442c-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="8442c-136">TTL</span><span class="sxs-lookup"><span data-stu-id="8442c-136">ttl</span></span>|<span data-ttu-id="8442c-137">Int32</span><span class="sxs-lookup"><span data-stu-id="8442c-137">Int32</span></span>| <span data-ttu-id="8442c-138">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="8442c-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="8442c-139">Não anulável</span><span class="sxs-lookup"><span data-stu-id="8442c-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="8442c-140">Relações</span><span class="sxs-lookup"><span data-stu-id="8442c-140">Relationships</span></span>
<span data-ttu-id="8442c-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8442c-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8442c-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8442c-142">JSON representation</span></span>
<span data-ttu-id="8442c-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8442c-143">Here is a JSON representation of the resource.</span></span>

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
