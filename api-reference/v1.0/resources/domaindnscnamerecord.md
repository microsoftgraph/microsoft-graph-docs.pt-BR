---
title: Tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
author: lleonard-msft
ms.openlocfilehash: bd1701e0757dc2facecb066beb7fe9108345a7f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330832"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="6e74c-104">Tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="6e74c-104">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="6e74c-p102">Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="6e74c-p102">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="6e74c-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e74c-107">Methods</span></span>
<span data-ttu-id="6e74c-p103">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="6e74c-p103">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="6e74c-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e74c-110">Properties</span></span>
| <span data-ttu-id="6e74c-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e74c-111">Property</span></span>     | <span data-ttu-id="6e74c-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e74c-112">Type</span></span>   |<span data-ttu-id="6e74c-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e74c-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e74c-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="6e74c-114">canonicalName</span></span>|<span data-ttu-id="6e74c-115">String</span><span class="sxs-lookup"><span data-stu-id="6e74c-115">String</span></span>| <span data-ttu-id="6e74c-p104">O nome canônico do registro CNAME. Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6e74c-p104">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="6e74c-118">id</span><span class="sxs-lookup"><span data-stu-id="6e74c-118">id</span></span>|<span data-ttu-id="6e74c-119">String</span><span class="sxs-lookup"><span data-stu-id="6e74c-119">String</span></span>| <span data-ttu-id="6e74c-p105">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura</span><span class="sxs-lookup"><span data-stu-id="6e74c-p105">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="6e74c-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="6e74c-122">isOptional</span></span>|<span data-ttu-id="6e74c-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e74c-123">Boolean</span></span>| <span data-ttu-id="6e74c-p106">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. Não anulável</span><span class="sxs-lookup"><span data-stu-id="6e74c-p106">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="6e74c-126">rótulo</span><span class="sxs-lookup"><span data-stu-id="6e74c-126">label</span></span>|<span data-ttu-id="6e74c-127">String</span><span class="sxs-lookup"><span data-stu-id="6e74c-127">String</span></span>| <span data-ttu-id="6e74c-128">O valor usado ao configurar a propriedade *alias/host/name* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6e74c-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="6e74c-129">recordType</span><span class="sxs-lookup"><span data-stu-id="6e74c-129">recordType</span></span>|<span data-ttu-id="6e74c-130">String</span><span class="sxs-lookup"><span data-stu-id="6e74c-130">String</span></span>| <span data-ttu-id="6e74c-p107">Tipo do registro DNS. Este valor sempre será *CName*. Chave</span><span class="sxs-lookup"><span data-stu-id="6e74c-p107">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="6e74c-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="6e74c-134">supportedService</span></span>|<span data-ttu-id="6e74c-135">String</span><span class="sxs-lookup"><span data-stu-id="6e74c-135">String</span></span>| <span data-ttu-id="6e74c-136">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="6e74c-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="6e74c-137">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="6e74c-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="6e74c-138">ttl</span><span class="sxs-lookup"><span data-stu-id="6e74c-138">ttl</span></span>|<span data-ttu-id="6e74c-139">Int32</span><span class="sxs-lookup"><span data-stu-id="6e74c-139">Int32</span></span>| <span data-ttu-id="6e74c-p108">O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro CNAME no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="6e74c-p108">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="6e74c-142">Relações</span><span class="sxs-lookup"><span data-stu-id="6e74c-142">Relationships</span></span>
<span data-ttu-id="6e74c-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e74c-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e74c-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e74c-144">JSON representation</span></span>
<span data-ttu-id="6e74c-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e74c-145">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.domainDnsRecord",
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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->