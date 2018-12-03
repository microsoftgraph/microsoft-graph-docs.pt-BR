---
title: Tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
ms.openlocfilehash: ed60c15463bd4182049fe3ae8fa32963f8574456
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003644"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="4f203-104">Tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="4f203-104">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="4f203-p102">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="4f203-p102">Represents a TXT record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="4f203-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="4f203-107">Methods</span></span>
<span data-ttu-id="4f203-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="4f203-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="4f203-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4f203-110">Properties</span></span>
| <span data-ttu-id="4f203-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4f203-111">Property</span></span>     | <span data-ttu-id="4f203-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="4f203-112">Type</span></span>   |<span data-ttu-id="4f203-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="4f203-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4f203-114">id</span><span class="sxs-lookup"><span data-stu-id="4f203-114">id</span></span>|<span data-ttu-id="4f203-115">String</span><span class="sxs-lookup"><span data-stu-id="4f203-115">String</span></span>| <span data-ttu-id="4f203-p104">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="4f203-p104">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span> |
|<span data-ttu-id="4f203-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="4f203-118">isOptional</span></span>|<span data-ttu-id="4f203-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="4f203-119">Boolean</span></span>| <span data-ttu-id="4f203-120">Se for falso, o registro TXT deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="4f203-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="4f203-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="4f203-121">label</span></span>|<span data-ttu-id="4f203-122">String</span><span class="sxs-lookup"><span data-stu-id="4f203-122">String</span></span>| <span data-ttu-id="4f203-123">O valor a ser usado ao configurar a propriedade *name* do registro TXT no host DNS.</span><span class="sxs-lookup"><span data-stu-id="4f203-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="4f203-124">recordType</span><span class="sxs-lookup"><span data-stu-id="4f203-124">recordType</span></span>|<span data-ttu-id="4f203-125">String</span><span class="sxs-lookup"><span data-stu-id="4f203-125">String</span></span>| <span data-ttu-id="4f203-p105">Tipo do registro DNS. Este valor sempre será *Txt*. Chave</span><span class="sxs-lookup"><span data-stu-id="4f203-p105">Type of DNS record. The value is always *Txt*. Key</span></span> |
|<span data-ttu-id="4f203-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="4f203-129">supportedService</span></span>|<span data-ttu-id="4f203-130">String</span><span class="sxs-lookup"><span data-stu-id="4f203-130">String</span></span>| <span data-ttu-id="4f203-131">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro TXT.</span><span class="sxs-lookup"><span data-stu-id="4f203-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="4f203-132">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="4f203-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="4f203-133">text</span><span class="sxs-lookup"><span data-stu-id="4f203-133">text</span></span>|<span data-ttu-id="4f203-134">String</span><span class="sxs-lookup"><span data-stu-id="4f203-134">String</span></span>| <span data-ttu-id="4f203-135">O valor usado ao configurar a propriedade *text* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="4f203-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="4f203-136">ttl</span><span class="sxs-lookup"><span data-stu-id="4f203-136">ttl</span></span>|<span data-ttu-id="4f203-137">Int32</span><span class="sxs-lookup"><span data-stu-id="4f203-137">Int32</span></span>| <span data-ttu-id="4f203-p106">O valor a ser usado ao configurar a propriedade *time-to-live (ttl)* do registro MX no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="4f203-p106">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="4f203-140">Relações</span><span class="sxs-lookup"><span data-stu-id="4f203-140">Relationships</span></span>
<span data-ttu-id="4f203-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4f203-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4f203-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4f203-142">JSON representation</span></span>
<span data-ttu-id="4f203-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4f203-143">Here is a JSON representation of the resource.</span></span>

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