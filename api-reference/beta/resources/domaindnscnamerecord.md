---
title: Tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade DomainDnsRecord.
ms.openlocfilehash: 9eaa48bb492572d4e5cac57ee07420ed492aac73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040167"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="6e5f1-104">Tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="6e5f1-104">domainDnsCnameRecord resource type</span></span>

> <span data-ttu-id="6e5f1-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6e5f1-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6e5f1-p103">Representa um registro CNAME adicionado ao arquivo de zona DNS de um domínio específico no locatário. Herdado da entidade [DomainDnsRecord](domaindnsrecord.md).</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p103">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant. Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="6e5f1-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="6e5f1-109">Methods</span></span>
<span data-ttu-id="6e5f1-p104">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="6e5f1-112">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6e5f1-112">Properties</span></span>
| <span data-ttu-id="6e5f1-113">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6e5f1-113">Property</span></span>     | <span data-ttu-id="6e5f1-114">Tipo</span><span class="sxs-lookup"><span data-stu-id="6e5f1-114">Type</span></span>   |<span data-ttu-id="6e5f1-115">Descrição</span><span class="sxs-lookup"><span data-stu-id="6e5f1-115">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6e5f1-116">canonicalName</span><span class="sxs-lookup"><span data-stu-id="6e5f1-116">canonicalName</span></span>|<span data-ttu-id="6e5f1-117">String</span><span class="sxs-lookup"><span data-stu-id="6e5f1-117">String</span></span>| <span data-ttu-id="6e5f1-p105">O nome canônico do registro CNAME. Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p105">The canonical name of the CNAME record. Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="6e5f1-120">id</span><span class="sxs-lookup"><span data-stu-id="6e5f1-120">id</span></span>|<span data-ttu-id="6e5f1-121">String</span><span class="sxs-lookup"><span data-stu-id="6e5f1-121">String</span></span>| <span data-ttu-id="6e5f1-p106">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p106">Unique identifier assigned to this entity. Not nullable, Read-only</span></span>|
|<span data-ttu-id="6e5f1-124">isOptional</span><span class="sxs-lookup"><span data-stu-id="6e5f1-124">isOptional</span></span>|<span data-ttu-id="6e5f1-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="6e5f1-125">Boolean</span></span>| <span data-ttu-id="6e5f1-p107">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio. Não anulável</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p107">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain. Not nullable</span></span> |
|<span data-ttu-id="6e5f1-128">rótulo</span><span class="sxs-lookup"><span data-stu-id="6e5f1-128">label</span></span>|<span data-ttu-id="6e5f1-129">String</span><span class="sxs-lookup"><span data-stu-id="6e5f1-129">String</span></span>| <span data-ttu-id="6e5f1-130">O valor usado ao configurar a propriedade *alias/host/name* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-130">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="6e5f1-131">recordType</span><span class="sxs-lookup"><span data-stu-id="6e5f1-131">recordType</span></span>|<span data-ttu-id="6e5f1-132">String</span><span class="sxs-lookup"><span data-stu-id="6e5f1-132">String</span></span>| <span data-ttu-id="6e5f1-p108">Tipo do registro DNS. Este valor sempre será *CName*. Chave</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p108">Type of DNS record. The value is always *CName*. Key</span></span>|
|<span data-ttu-id="6e5f1-136">supportedService</span><span class="sxs-lookup"><span data-stu-id="6e5f1-136">supportedService</span></span>|<span data-ttu-id="6e5f1-137">String</span><span class="sxs-lookup"><span data-stu-id="6e5f1-137">String</span></span>| <span data-ttu-id="6e5f1-138">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-138">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="6e5f1-139">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="6e5f1-139">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="6e5f1-140">ttl</span><span class="sxs-lookup"><span data-stu-id="6e5f1-140">ttl</span></span>|<span data-ttu-id="6e5f1-141">Int32</span><span class="sxs-lookup"><span data-stu-id="6e5f1-141">Int32</span></span>| <span data-ttu-id="6e5f1-p109">O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro CNAME no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="6e5f1-p109">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="6e5f1-144">Relações</span><span class="sxs-lookup"><span data-stu-id="6e5f1-144">Relationships</span></span>
<span data-ttu-id="6e5f1-145">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6e5f1-145">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="6e5f1-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6e5f1-146">JSON representation</span></span>
<span data-ttu-id="6e5f1-147">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6e5f1-147">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "domainDnsCnameRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->