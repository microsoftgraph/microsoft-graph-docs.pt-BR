---
title: tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado de entidade DomainDnsRecord.
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 5555fa6f02e0639f1e126112918c39168b445945
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42505844"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="31922-104">tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="31922-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="31922-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="31922-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="31922-106">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="31922-106">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="31922-107">Herdado de entidade [DomainDnsRecord](domaindnsrecord.md) .</span><span class="sxs-lookup"><span data-stu-id="31922-107">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="31922-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="31922-108">Methods</span></span>
<span data-ttu-id="31922-109">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="31922-109">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="31922-110">Confira o tópico de [domínio](domain.md) para obter informações sobre como consultar os registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="31922-110">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="31922-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="31922-111">Properties</span></span>
| <span data-ttu-id="31922-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="31922-112">Property</span></span>     | <span data-ttu-id="31922-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="31922-113">Type</span></span>   |<span data-ttu-id="31922-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="31922-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="31922-115">id</span><span class="sxs-lookup"><span data-stu-id="31922-115">id</span></span>|<span data-ttu-id="31922-116">String</span><span class="sxs-lookup"><span data-stu-id="31922-116">String</span></span>| <span data-ttu-id="31922-117">Identificador exclusivo atribuído a esta entidade.</span><span class="sxs-lookup"><span data-stu-id="31922-117">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="31922-118">Não anulável, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="31922-118">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="31922-119">IsOptional</span><span class="sxs-lookup"><span data-stu-id="31922-119">isOptional</span></span>|<span data-ttu-id="31922-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="31922-120">Boolean</span></span>| <span data-ttu-id="31922-121">Se for falso, o registro TXT deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="31922-121">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="31922-122">rótulo</span><span class="sxs-lookup"><span data-stu-id="31922-122">label</span></span>|<span data-ttu-id="31922-123">String</span><span class="sxs-lookup"><span data-stu-id="31922-123">String</span></span>| <span data-ttu-id="31922-124">O valor a ser usado ao configurar a propriedade *Name* do registro txt no host DNS.</span><span class="sxs-lookup"><span data-stu-id="31922-124">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="31922-125">recordType</span><span class="sxs-lookup"><span data-stu-id="31922-125">recordType</span></span>|<span data-ttu-id="31922-126">String</span><span class="sxs-lookup"><span data-stu-id="31922-126">String</span></span>| <span data-ttu-id="31922-127">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="31922-127">Type of DNS record.</span></span> <span data-ttu-id="31922-128">O valor é sempre *txt*.</span><span class="sxs-lookup"><span data-stu-id="31922-128">The value is always *Txt*.</span></span> <span data-ttu-id="31922-129">Chave</span><span class="sxs-lookup"><span data-stu-id="31922-129">Key</span></span> |
|<span data-ttu-id="31922-130">supportedService</span><span class="sxs-lookup"><span data-stu-id="31922-130">supportedService</span></span>|<span data-ttu-id="31922-131">String</span><span class="sxs-lookup"><span data-stu-id="31922-131">String</span></span>| <span data-ttu-id="31922-132">O Microsoft Online Services ou o recurso que tem uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="31922-132">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="31922-133">Pode ser um dos seguintes valores: **NULL**, *email*, *SharePoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="31922-133">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="31922-134">texto</span><span class="sxs-lookup"><span data-stu-id="31922-134">text</span></span>|<span data-ttu-id="31922-135">String</span><span class="sxs-lookup"><span data-stu-id="31922-135">String</span></span>| <span data-ttu-id="31922-136">O valor usado ao configurar a propriedade *Text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="31922-136">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="31922-137">TTL</span><span class="sxs-lookup"><span data-stu-id="31922-137">ttl</span></span>|<span data-ttu-id="31922-138">Int32</span><span class="sxs-lookup"><span data-stu-id="31922-138">Int32</span></span>| <span data-ttu-id="31922-139">O valor a ser usado ao configurar a propriedade *TTL (time-to-Live)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="31922-139">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="31922-140">Não anulável</span><span class="sxs-lookup"><span data-stu-id="31922-140">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="31922-141">Relações</span><span class="sxs-lookup"><span data-stu-id="31922-141">Relationships</span></span>
<span data-ttu-id="31922-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="31922-142">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="31922-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="31922-143">JSON representation</span></span>
<span data-ttu-id="31922-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="31922-144">Here is a JSON representation of the resource.</span></span>

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
