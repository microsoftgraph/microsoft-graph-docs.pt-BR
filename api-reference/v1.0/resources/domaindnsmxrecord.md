---
title: Tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
ms.openlocfilehash: 54a72f8e420d0313303b0787e803933888fb1e57
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27004975"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="4ca63-104">Tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="4ca63-104">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="4ca63-p102">Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="4ca63-p102">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4ca63-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4ca63-107">Methods</span></span>
<span data-ttu-id="4ca63-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="4ca63-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4ca63-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4ca63-110">Properties</span></span>
| <span data-ttu-id="4ca63-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4ca63-111">Property</span></span>     | <span data-ttu-id="4ca63-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="4ca63-112">Type</span></span>   |<span data-ttu-id="4ca63-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4ca63-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4ca63-114">id</span><span class="sxs-lookup"><span data-stu-id="4ca63-114">id</span></span>|<span data-ttu-id="4ca63-115">String</span><span class="sxs-lookup"><span data-stu-id="4ca63-115">String</span></span>| <span data-ttu-id="4ca63-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4ca63-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="4ca63-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="4ca63-118">isOptional</span></span>|<span data-ttu-id="4ca63-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="4ca63-119">Boolean</span></span>| <span data-ttu-id="4ca63-120">Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="4ca63-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4ca63-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="4ca63-121">label</span></span>|<span data-ttu-id="4ca63-122">String</span><span class="sxs-lookup"><span data-stu-id="4ca63-122">String</span></span>| <span data-ttu-id="4ca63-123">O valor usado ao configurar a propriedade *alias/host/name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="4ca63-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="4ca63-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="4ca63-124">mailExchange</span></span>|<span data-ttu-id="4ca63-125">String</span><span class="sxs-lookup"><span data-stu-id="4ca63-125">String</span></span>| <span data-ttu-id="4ca63-126">O valor usado ao configurar a propriedade *answer/destination/value* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="4ca63-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="4ca63-127">preference</span><span class="sxs-lookup"><span data-stu-id="4ca63-127">preference</span></span>|<span data-ttu-id="4ca63-128">Int32</span><span class="sxs-lookup"><span data-stu-id="4ca63-128">Int32</span></span>| <span data-ttu-id="4ca63-129">O valor usado ao configurar a propriedade *Preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="4ca63-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="4ca63-130">recordType</span><span class="sxs-lookup"><span data-stu-id="4ca63-130">recordType</span></span>|<span data-ttu-id="4ca63-131">String</span><span class="sxs-lookup"><span data-stu-id="4ca63-131">String</span></span>| <span data-ttu-id="4ca63-p105">Tipo do registro DNS. Este valor sempre será *Mx*. Chave</span><span class="sxs-lookup"><span data-stu-id="4ca63-p105">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="4ca63-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="4ca63-135">supportedService</span></span>|<span data-ttu-id="4ca63-136">String</span><span class="sxs-lookup"><span data-stu-id="4ca63-136">String</span></span>| <span data-ttu-id="4ca63-137">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro MX.</span><span class="sxs-lookup"><span data-stu-id="4ca63-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="4ca63-138">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="4ca63-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="4ca63-139">ttl</span><span class="sxs-lookup"><span data-stu-id="4ca63-139">ttl</span></span>|<span data-ttu-id="4ca63-140">Int32</span><span class="sxs-lookup"><span data-stu-id="4ca63-140">Int32</span></span>| <span data-ttu-id="4ca63-p106">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="4ca63-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4ca63-143">Relações</span><span class="sxs-lookup"><span data-stu-id="4ca63-143">Relationships</span></span>
<span data-ttu-id="4ca63-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4ca63-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4ca63-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4ca63-145">JSON representation</span></span>
<span data-ttu-id="4ca63-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4ca63-146">Here is a JSON representation of the resource.</span></span>

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