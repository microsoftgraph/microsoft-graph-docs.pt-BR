---
title: tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 14280f7ddaa172960a269a22255db4ea3e44dc61
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334503"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="853fb-104">tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="853fb-104">domainDnsTxtRecord resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="853fb-105">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="853fb-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="853fb-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="853fb-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="853fb-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="853fb-107">Methods</span></span>
<span data-ttu-id="853fb-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="853fb-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="853fb-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="853fb-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="853fb-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="853fb-110">Properties</span></span>
| <span data-ttu-id="853fb-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="853fb-111">Property</span></span>     | <span data-ttu-id="853fb-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="853fb-112">Type</span></span>   |<span data-ttu-id="853fb-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="853fb-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="853fb-114">id</span><span class="sxs-lookup"><span data-stu-id="853fb-114">id</span></span>|<span data-ttu-id="853fb-115">String</span><span class="sxs-lookup"><span data-stu-id="853fb-115">String</span></span>| <span data-ttu-id="853fb-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="853fb-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="853fb-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="853fb-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="853fb-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="853fb-118">isOptional</span></span>|<span data-ttu-id="853fb-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="853fb-119">Boolean</span></span>| <span data-ttu-id="853fb-120">Se for falso, o registro TXT deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="853fb-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="853fb-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="853fb-121">label</span></span>|<span data-ttu-id="853fb-122">String</span><span class="sxs-lookup"><span data-stu-id="853fb-122">String</span></span>| <span data-ttu-id="853fb-123">O valor a ser usado ao configurar a propriedade *Name* do registro txt no host DNS.</span><span class="sxs-lookup"><span data-stu-id="853fb-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="853fb-124">recordType</span><span class="sxs-lookup"><span data-stu-id="853fb-124">recordType</span></span>|<span data-ttu-id="853fb-125">String</span><span class="sxs-lookup"><span data-stu-id="853fb-125">String</span></span>| <span data-ttu-id="853fb-126">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="853fb-126">Type of DNS record.</span></span> <span data-ttu-id="853fb-127">O valor é sempre *txt*.</span><span class="sxs-lookup"><span data-stu-id="853fb-127">The value is always *Txt*.</span></span> <span data-ttu-id="853fb-128">Chave</span><span class="sxs-lookup"><span data-stu-id="853fb-128">Key</span></span> |
|<span data-ttu-id="853fb-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="853fb-129">supportedService</span></span>|<span data-ttu-id="853fb-130">String</span><span class="sxs-lookup"><span data-stu-id="853fb-130">String</span></span>| <span data-ttu-id="853fb-131">O Microsoft Online Services ou o recurso que tem uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="853fb-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="853fb-132">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, \*SharePointPublic \*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="853fb-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="853fb-133">texto</span><span class="sxs-lookup"><span data-stu-id="853fb-133">text</span></span>|<span data-ttu-id="853fb-134">String</span><span class="sxs-lookup"><span data-stu-id="853fb-134">String</span></span>| <span data-ttu-id="853fb-135">O valor usado ao configurar a propriedade *Text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="853fb-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="853fb-136">TTL</span><span class="sxs-lookup"><span data-stu-id="853fb-136">ttl</span></span>|<span data-ttu-id="853fb-137">Int32</span><span class="sxs-lookup"><span data-stu-id="853fb-137">Int32</span></span>| <span data-ttu-id="853fb-138">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="853fb-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="853fb-139">Não anulável</span><span class="sxs-lookup"><span data-stu-id="853fb-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="853fb-140">Relações</span><span class="sxs-lookup"><span data-stu-id="853fb-140">Relationships</span></span>
<span data-ttu-id="853fb-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="853fb-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="853fb-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="853fb-142">JSON representation</span></span>
<span data-ttu-id="853fb-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="853fb-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsTxtRecord"
}-->

```json
{
  "canonicalName": "String",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
