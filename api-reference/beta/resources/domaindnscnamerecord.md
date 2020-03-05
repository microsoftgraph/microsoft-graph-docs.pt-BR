---
title: tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 9b3a957197821bfb010aed5de071ec1e89192828
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42506362"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="f2c76-104">tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="f2c76-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="f2c76-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f2c76-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2c76-106">Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="f2c76-106">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="f2c76-107">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="f2c76-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="f2c76-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="f2c76-108">Methods</span></span>
<span data-ttu-id="f2c76-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="f2c76-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="f2c76-110">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="f2c76-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f2c76-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f2c76-111">Properties</span></span>
| <span data-ttu-id="f2c76-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f2c76-112">Property</span></span>     | <span data-ttu-id="f2c76-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="f2c76-113">Type</span></span>   |<span data-ttu-id="f2c76-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f2c76-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f2c76-115">canônicaname</span><span class="sxs-lookup"><span data-stu-id="f2c76-115">canonicalName</span></span>|<span data-ttu-id="f2c76-116">String</span><span class="sxs-lookup"><span data-stu-id="f2c76-116">String</span></span>| <span data-ttu-id="f2c76-117">O nome canônico do registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="f2c76-117">The canonical name of the CNAME record.</span></span> <span data-ttu-id="f2c76-118">Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f2c76-118">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="f2c76-119">id</span><span class="sxs-lookup"><span data-stu-id="f2c76-119">id</span></span>|<span data-ttu-id="f2c76-120">String</span><span class="sxs-lookup"><span data-stu-id="f2c76-120">String</span></span>| <span data-ttu-id="f2c76-121">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="f2c76-121">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="f2c76-122">Não anulável, somente leitura</span><span class="sxs-lookup"><span data-stu-id="f2c76-122">Not nullable, Read-only</span></span>|
|<span data-ttu-id="f2c76-123">IsOptional</span><span class="sxs-lookup"><span data-stu-id="f2c76-123">isOptional</span></span>|<span data-ttu-id="f2c76-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2c76-124">Boolean</span></span>| <span data-ttu-id="f2c76-125">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="f2c76-125">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="f2c76-126">Não anulável</span><span class="sxs-lookup"><span data-stu-id="f2c76-126">Not nullable</span></span> |
|<span data-ttu-id="f2c76-127">rótulo</span><span class="sxs-lookup"><span data-stu-id="f2c76-127">label</span></span>|<span data-ttu-id="f2c76-128">String</span><span class="sxs-lookup"><span data-stu-id="f2c76-128">String</span></span>| <span data-ttu-id="f2c76-129">O valor usado ao configurar o *alias/host/nome* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f2c76-129">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="f2c76-130">recordType</span><span class="sxs-lookup"><span data-stu-id="f2c76-130">recordType</span></span>|<span data-ttu-id="f2c76-131">String</span><span class="sxs-lookup"><span data-stu-id="f2c76-131">String</span></span>| <span data-ttu-id="f2c76-132">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="f2c76-132">Type of DNS record.</span></span> <span data-ttu-id="f2c76-133">O valor é sempre *CNAME*.</span><span class="sxs-lookup"><span data-stu-id="f2c76-133">The value is always *CName*.</span></span> <span data-ttu-id="f2c76-134">Chave</span><span class="sxs-lookup"><span data-stu-id="f2c76-134">Key</span></span>|
|<span data-ttu-id="f2c76-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="f2c76-135">supportedService</span></span>|<span data-ttu-id="f2c76-136">String</span><span class="sxs-lookup"><span data-stu-id="f2c76-136">String</span></span>| <span data-ttu-id="f2c76-137">O Microsoft Online Services ou o recurso que tem uma dependência neste registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="f2c76-137">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="f2c76-138">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="f2c76-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="f2c76-139">TTL</span><span class="sxs-lookup"><span data-stu-id="f2c76-139">ttl</span></span>|<span data-ttu-id="f2c76-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f2c76-140">Int32</span></span>| <span data-ttu-id="f2c76-141">O valor a ser usado ao configurar a propriedade TTL (time-to-Live) do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f2c76-141">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="f2c76-142">Não anulável</span><span class="sxs-lookup"><span data-stu-id="f2c76-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="f2c76-143">Relações</span><span class="sxs-lookup"><span data-stu-id="f2c76-143">Relationships</span></span>
<span data-ttu-id="f2c76-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f2c76-144">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f2c76-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f2c76-145">JSON representation</span></span>
<span data-ttu-id="f2c76-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f2c76-146">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!--
{
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
