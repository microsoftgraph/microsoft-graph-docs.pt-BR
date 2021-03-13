---
title: Tipo de recurso domainDnsMxRecord
description: Representa um registro MX adicionado ao arquivo de zona DNS de um determinado domínio no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 017fe2ef132ce78a392a2f6fe83895b365002048
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761174"
---
# <a name="domaindnsmxrecord-resource-type"></a><span data-ttu-id="f5e68-103">Tipo de recurso domainDnsMxRecord</span><span class="sxs-lookup"><span data-stu-id="f5e68-103">domainDnsMxRecord resource type</span></span>

<span data-ttu-id="f5e68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f5e68-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f5e68-105">Representa um registro MX adicionado ao arquivo de zona DNS de um determinado domínio no locatário.</span><span class="sxs-lookup"><span data-stu-id="f5e68-105">Represents a MX record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="f5e68-106">Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="f5e68-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="f5e68-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="f5e68-107">Methods</span></span>
<span data-ttu-id="f5e68-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="f5e68-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="f5e68-109">Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="f5e68-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="f5e68-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f5e68-110">Properties</span></span>
| <span data-ttu-id="f5e68-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f5e68-111">Property</span></span>     | <span data-ttu-id="f5e68-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="f5e68-112">Type</span></span>   |<span data-ttu-id="f5e68-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5e68-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5e68-114">id</span><span class="sxs-lookup"><span data-stu-id="f5e68-114">id</span></span>|<span data-ttu-id="f5e68-115">String</span><span class="sxs-lookup"><span data-stu-id="f5e68-115">String</span></span>| <span data-ttu-id="f5e68-116">Identificador exclusivo atribuído a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="f5e68-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="f5e68-117">Não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f5e68-117">Not nullable, Read-only.</span></span>|
|<span data-ttu-id="f5e68-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="f5e68-118">isOptional</span></span>|<span data-ttu-id="f5e68-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="f5e68-119">Boolean</span></span>| <span data-ttu-id="f5e68-120">Se for false, o registro MX deve ser configurado pelo cliente no host DNS para Microsoft Online Services operar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="f5e68-120">If false, the MX record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="f5e68-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="f5e68-121">label</span></span>|<span data-ttu-id="f5e68-122">String</span><span class="sxs-lookup"><span data-stu-id="f5e68-122">String</span></span>| <span data-ttu-id="f5e68-123">Valor usado ao configurar a *propriedade alias/host/name* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f5e68-123">Value used when configuring the *alias/host/name* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="f5e68-124">mailExchange</span><span class="sxs-lookup"><span data-stu-id="f5e68-124">mailExchange</span></span>|<span data-ttu-id="f5e68-125">String</span><span class="sxs-lookup"><span data-stu-id="f5e68-125">String</span></span>| <span data-ttu-id="f5e68-126">Valor usado ao configurar *a resposta/destino/valor* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f5e68-126">Value used when configuring the *answer/destination/value* of the MX record at the DNS host.</span></span>|
|<span data-ttu-id="f5e68-127">preference</span><span class="sxs-lookup"><span data-stu-id="f5e68-127">preference</span></span>|<span data-ttu-id="f5e68-128">Int32</span><span class="sxs-lookup"><span data-stu-id="f5e68-128">Int32</span></span>| <span data-ttu-id="f5e68-129">Valor usado ao configurar a *propriedade Preference/Priority* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f5e68-129">Value used when configuring the *Preference/Priority* property of the MX record at the DNS host.</span></span> |
|<span data-ttu-id="f5e68-130">recordType</span><span class="sxs-lookup"><span data-stu-id="f5e68-130">recordType</span></span>|<span data-ttu-id="f5e68-131">String</span><span class="sxs-lookup"><span data-stu-id="f5e68-131">String</span></span>| <span data-ttu-id="f5e68-132">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="f5e68-132">Type of DNS record.</span></span> <span data-ttu-id="f5e68-133">O valor é sempre *Mx*.</span><span class="sxs-lookup"><span data-stu-id="f5e68-133">The value is always *Mx*.</span></span> <span data-ttu-id="f5e68-134">Chave</span><span class="sxs-lookup"><span data-stu-id="f5e68-134">Key</span></span> |
|<span data-ttu-id="f5e68-135">supportedService</span><span class="sxs-lookup"><span data-stu-id="f5e68-135">supportedService</span></span>|<span data-ttu-id="f5e68-136">String</span><span class="sxs-lookup"><span data-stu-id="f5e68-136">String</span></span>| <span data-ttu-id="f5e68-137">Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro MX.</span><span class="sxs-lookup"><span data-stu-id="f5e68-137">Microsoft Online Service or feature that has a dependency on this MX record.</span></span></br></br><span data-ttu-id="f5e68-138">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="f5e68-138">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="f5e68-139">ttl</span><span class="sxs-lookup"><span data-stu-id="f5e68-139">ttl</span></span>|<span data-ttu-id="f5e68-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f5e68-140">Int32</span></span>| <span data-ttu-id="f5e68-141">Valor a ser usado ao configurar a *propriedade time-to-live (ttl)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="f5e68-141">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="f5e68-142">Não anulada</span><span class="sxs-lookup"><span data-stu-id="f5e68-142">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="f5e68-143">Relações</span><span class="sxs-lookup"><span data-stu-id="f5e68-143">Relationships</span></span>
<span data-ttu-id="f5e68-144">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f5e68-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5e68-145">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f5e68-145">JSON representation</span></span>
<span data-ttu-id="f5e68-146">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f5e68-146">Here is a JSON representation of the resource.</span></span>

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

