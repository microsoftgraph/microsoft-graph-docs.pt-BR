---
title: Tipo de recurso domainDnsCnameRecord
description: Representa um registro CNAME adicionado ao arquivo de zona DNS de um determinado domínio no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: ecbe5c0dd1d547a6abb116c5152a8d21f0ee3fd8
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760880"
---
# <a name="domaindnscnamerecord-resource-type"></a><span data-ttu-id="3c0e3-103">Tipo de recurso domainDnsCnameRecord</span><span class="sxs-lookup"><span data-stu-id="3c0e3-103">domainDnsCnameRecord resource type</span></span>

<span data-ttu-id="3c0e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c0e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3c0e3-105">Representa um registro CNAME adicionado ao arquivo de zona DNS de um determinado domínio no locatário.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-105">Represents a CNAME record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="3c0e3-106">Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="3c0e3-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>


## <a name="methods"></a><span data-ttu-id="3c0e3-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="3c0e3-107">Methods</span></span>
<span data-ttu-id="3c0e3-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="3c0e3-109">Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="3c0e3-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3c0e3-110">Properties</span></span>
| <span data-ttu-id="3c0e3-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3c0e3-111">Property</span></span>     | <span data-ttu-id="3c0e3-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="3c0e3-112">Type</span></span>   |<span data-ttu-id="3c0e3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="3c0e3-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3c0e3-114">canonicalName</span><span class="sxs-lookup"><span data-stu-id="3c0e3-114">canonicalName</span></span>|<span data-ttu-id="3c0e3-115">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3c0e3-115">String</span></span>| <span data-ttu-id="3c0e3-116">O nome canônico do registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-116">The canonical name of the CNAME record.</span></span> <span data-ttu-id="3c0e3-117">Usado para configurar o registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-117">Used to configure the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3c0e3-118">id</span><span class="sxs-lookup"><span data-stu-id="3c0e3-118">id</span></span>|<span data-ttu-id="3c0e3-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3c0e3-119">String</span></span>| <span data-ttu-id="3c0e3-120">Identificador exclusivo atribuído a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-120">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="3c0e3-121">Não anulada, somente leitura</span><span class="sxs-lookup"><span data-stu-id="3c0e3-121">Not nullable, Read-only</span></span>|
|<span data-ttu-id="3c0e3-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="3c0e3-122">isOptional</span></span>|<span data-ttu-id="3c0e3-123">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c0e3-123">Boolean</span></span>| <span data-ttu-id="3c0e3-124">Se for falso, o registro CNAME deverá ser configurado pelo cliente no host DNS para que Microsoft Online Services funcione corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-124">If false, the CNAME record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> <span data-ttu-id="3c0e3-125">Não anulada</span><span class="sxs-lookup"><span data-stu-id="3c0e3-125">Not nullable</span></span> |
|<span data-ttu-id="3c0e3-126">rótulo</span><span class="sxs-lookup"><span data-stu-id="3c0e3-126">label</span></span>|<span data-ttu-id="3c0e3-127">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3c0e3-127">String</span></span>| <span data-ttu-id="3c0e3-128">Valor usado ao configurar *o alias/host/nome* do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-128">Value used when configuring the *alias/host/name* of the CNAME record at the DNS host.</span></span> |
|<span data-ttu-id="3c0e3-129">recordType</span><span class="sxs-lookup"><span data-stu-id="3c0e3-129">recordType</span></span>|<span data-ttu-id="3c0e3-130">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3c0e3-130">String</span></span>| <span data-ttu-id="3c0e3-131">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-131">Type of DNS record.</span></span> <span data-ttu-id="3c0e3-132">O valor é sempre *CName*.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-132">The value is always *CName*.</span></span> <span data-ttu-id="3c0e3-133">Chave</span><span class="sxs-lookup"><span data-stu-id="3c0e3-133">Key</span></span>|
|<span data-ttu-id="3c0e3-134">supportedService</span><span class="sxs-lookup"><span data-stu-id="3c0e3-134">supportedService</span></span>|<span data-ttu-id="3c0e3-135">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="3c0e3-135">String</span></span>| <span data-ttu-id="3c0e3-136">Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro CNAME.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-136">Microsoft Online Service or feature that has a dependency on this CNAME record.</span></span></br></br><span data-ttu-id="3c0e3-137">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="3c0e3-137">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="3c0e3-138">ttl</span><span class="sxs-lookup"><span data-stu-id="3c0e3-138">ttl</span></span>|<span data-ttu-id="3c0e3-139">Int32</span><span class="sxs-lookup"><span data-stu-id="3c0e3-139">Int32</span></span>| <span data-ttu-id="3c0e3-140">Valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro CNAME no host DNS.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-140">Value to use when configuring the time-to-live (ttl) property of the CNAME record at the DNS host.</span></span> <span data-ttu-id="3c0e3-141">Não anulada</span><span class="sxs-lookup"><span data-stu-id="3c0e3-141">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="3c0e3-142">Relações</span><span class="sxs-lookup"><span data-stu-id="3c0e3-142">Relationships</span></span>
<span data-ttu-id="3c0e3-143">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3c0e3-143">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="3c0e3-144">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3c0e3-144">JSON representation</span></span>
<span data-ttu-id="3c0e3-145">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3c0e3-145">Here is a JSON representation of the resource.</span></span>

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


