---
title: Tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: 045e18b67f3a5fae93651cc59c3d2a16ee9e63f1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811519"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="94bc7-104">Tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="94bc7-104">domainDnsTxtRecord resource type</span></span>

> <span data-ttu-id="94bc7-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="94bc7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94bc7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="94bc7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="94bc7-p103">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="94bc7-p103">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="94bc7-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="94bc7-109">Methods</span></span>
<span data-ttu-id="94bc7-p104">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="94bc7-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="94bc7-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="94bc7-112">Properties</span></span>
| <span data-ttu-id="94bc7-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94bc7-113">Property</span></span>     | <span data-ttu-id="94bc7-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="94bc7-114">Type</span></span>   |<span data-ttu-id="94bc7-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="94bc7-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94bc7-116">id</span><span class="sxs-lookup"><span data-stu-id="94bc7-116">id</span></span>|<span data-ttu-id="94bc7-117">String</span><span class="sxs-lookup"><span data-stu-id="94bc7-117">String</span></span>| <span data-ttu-id="94bc7-p105">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="94bc7-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="94bc7-120">isOptional</span><span class="sxs-lookup"><span data-stu-id="94bc7-120">isOptional</span></span>|<span data-ttu-id="94bc7-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="94bc7-121">Boolean</span></span>| <span data-ttu-id="94bc7-122">Se for falso, o registro TXT deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="94bc7-122">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="94bc7-123">rótulo</span><span class="sxs-lookup"><span data-stu-id="94bc7-123">label</span></span>|<span data-ttu-id="94bc7-124">String</span><span class="sxs-lookup"><span data-stu-id="94bc7-124">String</span></span>| <span data-ttu-id="94bc7-125">O valor a ser usado ao configurar a propriedade *name* do registro TXT no host DNS.</span><span class="sxs-lookup"><span data-stu-id="94bc7-125">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="94bc7-126">recordType</span><span class="sxs-lookup"><span data-stu-id="94bc7-126">recordType</span></span>|<span data-ttu-id="94bc7-127">String</span><span class="sxs-lookup"><span data-stu-id="94bc7-127">String</span></span>| <span data-ttu-id="94bc7-p106">Tipo do registro DNS. Este valor sempre será *Txt*. Chave</span><span class="sxs-lookup"><span data-stu-id="94bc7-p106">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="94bc7-131">supportedService</span><span class="sxs-lookup"><span data-stu-id="94bc7-131">supportedService</span></span>|<span data-ttu-id="94bc7-132">String</span><span class="sxs-lookup"><span data-stu-id="94bc7-132">String</span></span>| <span data-ttu-id="94bc7-133">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="94bc7-133">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="94bc7-134">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="94bc7-134">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="94bc7-135">text</span><span class="sxs-lookup"><span data-stu-id="94bc7-135">text</span></span>|<span data-ttu-id="94bc7-136">String</span><span class="sxs-lookup"><span data-stu-id="94bc7-136">String</span></span>| <span data-ttu-id="94bc7-137">O valor usado ao configurar a propriedade *text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="94bc7-137">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="94bc7-138">ttl</span><span class="sxs-lookup"><span data-stu-id="94bc7-138">ttl</span></span>|<span data-ttu-id="94bc7-139">Int32</span><span class="sxs-lookup"><span data-stu-id="94bc7-139">Int32</span></span>| <span data-ttu-id="94bc7-p107">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="94bc7-p107">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="94bc7-142">Relações</span><span class="sxs-lookup"><span data-stu-id="94bc7-142">Relationships</span></span>
<span data-ttu-id="94bc7-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="94bc7-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="94bc7-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="94bc7-144">JSON representation</span></span>
<span data-ttu-id="94bc7-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="94bc7-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsTxtRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
