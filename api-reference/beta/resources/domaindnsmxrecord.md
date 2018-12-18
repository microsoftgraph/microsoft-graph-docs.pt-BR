---
title: Tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: 562afbd6998ad1678f4f055dacf89af9b1ed4446
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320647"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="df8a7-104">Tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="df8a7-104">domainDnsMxRecord resource type</span></span>

> <span data-ttu-id="df8a7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="df8a7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df8a7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="df8a7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="df8a7-p103">Representa um registro MX adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="df8a7-p103">Represents a MX record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="df8a7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="df8a7-109">Methods</span></span>
<span data-ttu-id="df8a7-p104">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="df8a7-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="df8a7-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="df8a7-112">Properties</span></span>
| <span data-ttu-id="df8a7-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="df8a7-113">Property</span></span>     | <span data-ttu-id="df8a7-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="df8a7-114">Type</span></span>   |<span data-ttu-id="df8a7-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="df8a7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df8a7-116">id</span><span class="sxs-lookup"><span data-stu-id="df8a7-116">id</span></span>|<span data-ttu-id="df8a7-117">String</span><span class="sxs-lookup"><span data-stu-id="df8a7-117">String</span></span>| <span data-ttu-id="df8a7-p105">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="df8a7-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="df8a7-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="df8a7-120">isOptional</span></span>|<span data-ttu-id="df8a7-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="df8a7-121">Boolean</span></span>| <span data-ttu-id="df8a7-122">Se for falso, o registro MX deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="df8a7-122">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="df8a7-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="df8a7-123">label</span></span>|<span data-ttu-id="df8a7-124">String</span><span class="sxs-lookup"><span data-stu-id="df8a7-124">String</span></span>| <span data-ttu-id="df8a7-125">O valor usado ao configurar a propriedade *alias/host/name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="df8a7-125">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="df8a7-126">mailExchange</span><span class="sxs-lookup"><span data-stu-id="df8a7-126">mailExchange</span></span>|<span data-ttu-id="df8a7-127">String</span><span class="sxs-lookup"><span data-stu-id="df8a7-127">String</span></span>| <span data-ttu-id="df8a7-128">O valor usado ao configurar a propriedade *answer/destination/value* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="df8a7-128">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="df8a7-129">preference</span><span class="sxs-lookup"><span data-stu-id="df8a7-129">preference</span></span>|<span data-ttu-id="df8a7-130">Int32</span><span class="sxs-lookup"><span data-stu-id="df8a7-130">Int32</span></span>| <span data-ttu-id="df8a7-131">O valor usado ao configurar a propriedade *Preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="df8a7-131">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="df8a7-132">recordType</span><span class="sxs-lookup"><span data-stu-id="df8a7-132">recordType</span></span>|<span data-ttu-id="df8a7-133">String</span><span class="sxs-lookup"><span data-stu-id="df8a7-133">String</span></span>| <span data-ttu-id="df8a7-p106">Tipo do registro DNS. Este valor sempre será *Mx*. Chave</span><span class="sxs-lookup"><span data-stu-id="df8a7-p106">Type of DNS record. The value is always *Mx*. Key</span></span> |
|<span data-ttu-id="df8a7-137">supportedService</span><span class="sxs-lookup"><span data-stu-id="df8a7-137">supportedService</span></span>|<span data-ttu-id="df8a7-138">String</span><span class="sxs-lookup"><span data-stu-id="df8a7-138">String</span></span>| <span data-ttu-id="df8a7-139">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro MX.</span><span class="sxs-lookup"><span data-stu-id="df8a7-139">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="df8a7-140">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="df8a7-140">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="df8a7-141">ttl</span><span class="sxs-lookup"><span data-stu-id="df8a7-141">ttl</span></span>|<span data-ttu-id="df8a7-142">Int32</span><span class="sxs-lookup"><span data-stu-id="df8a7-142">Int32</span></span>| <span data-ttu-id="df8a7-p107">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="df8a7-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="df8a7-145">Relações</span><span class="sxs-lookup"><span data-stu-id="df8a7-145">Relationships</span></span>
<span data-ttu-id="df8a7-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="df8a7-146">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="df8a7-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="df8a7-147">JSON representation</span></span>
<span data-ttu-id="df8a7-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="df8a7-148">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsMxRecord"
}-->

```json
{
  "canonicalName": "String",
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