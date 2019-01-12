---
title: Tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 23d36114472073aedf38ca601380bb9ba38adc7d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967550"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="d9924-104">Tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="d9924-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="d9924-p102">Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="d9924-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="d9924-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="d9924-107">Methods</span></span>
<span data-ttu-id="d9924-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="d9924-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="d9924-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d9924-110">Properties</span></span>
| <span data-ttu-id="d9924-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9924-111">Property</span></span>     | <span data-ttu-id="d9924-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9924-112">Type</span></span>   |<span data-ttu-id="d9924-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9924-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d9924-114">id</span><span class="sxs-lookup"><span data-stu-id="d9924-114">id</span></span>|<span data-ttu-id="d9924-115">String</span><span class="sxs-lookup"><span data-stu-id="d9924-115">String</span></span>| <span data-ttu-id="d9924-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="d9924-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="d9924-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="d9924-118">isOptional</span></span>|<span data-ttu-id="d9924-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9924-119">Boolean</span></span>| <span data-ttu-id="d9924-120">Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="d9924-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="d9924-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="d9924-121">label</span></span>|<span data-ttu-id="d9924-122">String</span><span class="sxs-lookup"><span data-stu-id="d9924-122">String</span></span>| <span data-ttu-id="d9924-123">O valor usado ao configurar a propriedade *alias/host/name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="d9924-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="d9924-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="d9924-124">mailExchange</span></span>|<span data-ttu-id="d9924-125">String</span><span class="sxs-lookup"><span data-stu-id="d9924-125">String</span></span>| <span data-ttu-id="d9924-126">O valor usado ao configurar a propriedade *answer/destination/value* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="d9924-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="d9924-127">preference</span><span class="sxs-lookup"><span data-stu-id="d9924-127">preference</span></span>|<span data-ttu-id="d9924-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d9924-128">Int32</span></span>| <span data-ttu-id="d9924-129">O valor usado ao configurar a propriedade *Preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="d9924-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="d9924-130">recordType</span><span class="sxs-lookup"><span data-stu-id="d9924-130">recordType</span></span>|<span data-ttu-id="d9924-131">String</span><span class="sxs-lookup"><span data-stu-id="d9924-131">String</span></span>| <span data-ttu-id="d9924-p105">Tipo do registro DNS. Este valor sempre será *Mx*. Chave</span><span class="sxs-lookup"><span data-stu-id="d9924-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="d9924-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="d9924-135">supportedService</span></span>|<span data-ttu-id="d9924-136">String</span><span class="sxs-lookup"><span data-stu-id="d9924-136">String</span></span>| <span data-ttu-id="d9924-137">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro MX.</span><span class="sxs-lookup"><span data-stu-id="d9924-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="d9924-138">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="d9924-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="d9924-139">ttl</span><span class="sxs-lookup"><span data-stu-id="d9924-139">ttl</span></span>|<span data-ttu-id="d9924-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d9924-140">Int32</span></span>| <span data-ttu-id="d9924-p106">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="d9924-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="d9924-143">Relações</span><span class="sxs-lookup"><span data-stu-id="d9924-143">Relationships</span></span>
<span data-ttu-id="d9924-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d9924-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d9924-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d9924-145">JSON representation</span></span>
<span data-ttu-id="d9924-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d9924-146">Here is a JSON representation of the resource.</span></span>

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
