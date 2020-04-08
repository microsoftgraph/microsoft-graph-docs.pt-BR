---
title: tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: bd5bbe5f4167142821eea4bc72b53f6c0202fcd4
ms.sourcegitcommit: 11503211a31ea17f4e577c21ec36d364184c0580
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/08/2020
ms.locfileid: "43181885"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="b93e8-103">tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="b93e8-103">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="b93e8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b93e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b93e8-105">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="b93e8-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="b93e8-106">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="b93e8-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="b93e8-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="b93e8-107">Methods</span></span>
<span data-ttu-id="b93e8-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="b93e8-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="b93e8-109">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="b93e8-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="b93e8-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b93e8-110">Properties</span></span>
| <span data-ttu-id="b93e8-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b93e8-111">Property</span></span>     | <span data-ttu-id="b93e8-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="b93e8-112">Type</span></span>   |<span data-ttu-id="b93e8-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="b93e8-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b93e8-114">id</span><span class="sxs-lookup"><span data-stu-id="b93e8-114">id</span></span>|<span data-ttu-id="b93e8-115">String</span><span class="sxs-lookup"><span data-stu-id="b93e8-115">String</span></span>| <span data-ttu-id="b93e8-116">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="b93e8-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="b93e8-117">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b93e8-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="b93e8-118">IsOptional</span><span class="sxs-lookup"><span data-stu-id="b93e8-118">isOptional</span></span>|<span data-ttu-id="b93e8-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="b93e8-119">Boolean</span></span>| <span data-ttu-id="b93e8-120">Se for falso, o registro TXT deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="b93e8-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="b93e8-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="b93e8-121">label</span></span>|<span data-ttu-id="b93e8-122">String</span><span class="sxs-lookup"><span data-stu-id="b93e8-122">String</span></span>| <span data-ttu-id="b93e8-123">O valor a ser usado ao configurar a propriedade *Name* do registro txt no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b93e8-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="b93e8-124">recordType</span><span class="sxs-lookup"><span data-stu-id="b93e8-124">recordType</span></span>|<span data-ttu-id="b93e8-125">String</span><span class="sxs-lookup"><span data-stu-id="b93e8-125">String</span></span>| <span data-ttu-id="b93e8-126">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="b93e8-126">Type of DNS record.</span></span> <span data-ttu-id="b93e8-127">O valor é sempre *txt*.</span><span class="sxs-lookup"><span data-stu-id="b93e8-127">The value is always *Txt*.</span></span> <span data-ttu-id="b93e8-128">Chave</span><span class="sxs-lookup"><span data-stu-id="b93e8-128">Key</span></span> |
|<span data-ttu-id="b93e8-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="b93e8-129">supportedService</span></span>|<span data-ttu-id="b93e8-130">String</span><span class="sxs-lookup"><span data-stu-id="b93e8-130">String</span></span>| <span data-ttu-id="b93e8-131">O Microsoft Online Services ou o recurso que tem uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="b93e8-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="b93e8-132">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="b93e8-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="b93e8-133">texto</span><span class="sxs-lookup"><span data-stu-id="b93e8-133">text</span></span>|<span data-ttu-id="b93e8-134">String</span><span class="sxs-lookup"><span data-stu-id="b93e8-134">String</span></span>| <span data-ttu-id="b93e8-135">O valor usado ao configurar a propriedade *Text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b93e8-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="b93e8-136">TTL</span><span class="sxs-lookup"><span data-stu-id="b93e8-136">ttl</span></span>|<span data-ttu-id="b93e8-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b93e8-137">Int32</span></span>| <span data-ttu-id="b93e8-138">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="b93e8-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="b93e8-139">Não anulável</span><span class="sxs-lookup"><span data-stu-id="b93e8-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="b93e8-140">Relações</span><span class="sxs-lookup"><span data-stu-id="b93e8-140">Relationships</span></span>
<span data-ttu-id="b93e8-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b93e8-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b93e8-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b93e8-142">JSON representation</span></span>
<span data-ttu-id="b93e8-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b93e8-143">Here is a JSON representation of the resource.</span></span>

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
