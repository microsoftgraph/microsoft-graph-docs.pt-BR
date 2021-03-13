---
title: Tipo de recurso domainDnsTxtRecord
description: Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.
author: adimitui
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 9f63b671135edceb715aa4b3641b4bf189b74a33
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761378"
---
# <a name="domaindnstxtrecord-resource-type"></a><span data-ttu-id="93b08-103">Tipo de recurso domainDnsTxtRecord</span><span class="sxs-lookup"><span data-stu-id="93b08-103">domainDnsTxtRecord resource type</span></span>

<span data-ttu-id="93b08-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93b08-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="93b08-105">Representa um registro TXT adicionado ao arquivo de zona DNS de um domínio específico no locatário.</span><span class="sxs-lookup"><span data-stu-id="93b08-105">Represents a TXT record added to the DNS zone file of a particular domain in the tenant.</span></span> <span data-ttu-id="93b08-106">Herdada [da entidade DomainDnsRecord.](domaindnsrecord.md)</span><span class="sxs-lookup"><span data-stu-id="93b08-106">Inherited from [DomainDnsRecord](domaindnsrecord.md) entity.</span></span>

## <a name="methods"></a><span data-ttu-id="93b08-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="93b08-107">Methods</span></span>
<span data-ttu-id="93b08-108">Não há suporte para consultas diretas a esse recurso.</span><span class="sxs-lookup"><span data-stu-id="93b08-108">Direct queries to this resource are not supported.</span></span> <span data-ttu-id="93b08-109">Consulte o tópico [de domínio](domain.md) para obter informações sobre como consultar registros de serviço de domínio.</span><span class="sxs-lookup"><span data-stu-id="93b08-109">Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="93b08-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="93b08-110">Properties</span></span>
| <span data-ttu-id="93b08-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="93b08-111">Property</span></span>     | <span data-ttu-id="93b08-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="93b08-112">Type</span></span>   |<span data-ttu-id="93b08-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="93b08-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="93b08-114">id</span><span class="sxs-lookup"><span data-stu-id="93b08-114">id</span></span>|<span data-ttu-id="93b08-115">String</span><span class="sxs-lookup"><span data-stu-id="93b08-115">String</span></span>| <span data-ttu-id="93b08-116">Identificador exclusivo atribuído a essa entidade.</span><span class="sxs-lookup"><span data-stu-id="93b08-116">Unique identifier assigned to this entity.</span></span> <span data-ttu-id="93b08-117">Não anulada, somente leitura.</span><span class="sxs-lookup"><span data-stu-id="93b08-117">Not nullable, Read-only.</span></span> |
|<span data-ttu-id="93b08-118">isOptional</span><span class="sxs-lookup"><span data-stu-id="93b08-118">isOptional</span></span>|<span data-ttu-id="93b08-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="93b08-119">Boolean</span></span>| <span data-ttu-id="93b08-120">Se for false, o registro TXT deverá ser configurado pelo cliente no host DNS para Microsoft Online Services operar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="93b08-120">If false, the TXT record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="93b08-121">rótulo</span><span class="sxs-lookup"><span data-stu-id="93b08-121">label</span></span>|<span data-ttu-id="93b08-122">String</span><span class="sxs-lookup"><span data-stu-id="93b08-122">String</span></span>| <span data-ttu-id="93b08-123">Valor a ser usado ao configurar a propriedade *name* do registro TXT no host DNS.</span><span class="sxs-lookup"><span data-stu-id="93b08-123">Value to use when configuring the *name* property of the TXT record at the DNS host.</span></span>|
|<span data-ttu-id="93b08-124">recordType</span><span class="sxs-lookup"><span data-stu-id="93b08-124">recordType</span></span>|<span data-ttu-id="93b08-125">String</span><span class="sxs-lookup"><span data-stu-id="93b08-125">String</span></span>| <span data-ttu-id="93b08-126">Tipo de registro DNS.</span><span class="sxs-lookup"><span data-stu-id="93b08-126">Type of DNS record.</span></span> <span data-ttu-id="93b08-127">O valor é sempre *Txt*.</span><span class="sxs-lookup"><span data-stu-id="93b08-127">The value is always *Txt*.</span></span> <span data-ttu-id="93b08-128">Chave</span><span class="sxs-lookup"><span data-stu-id="93b08-128">Key</span></span> |
|<span data-ttu-id="93b08-129">supportedService</span><span class="sxs-lookup"><span data-stu-id="93b08-129">supportedService</span></span>|<span data-ttu-id="93b08-130">String</span><span class="sxs-lookup"><span data-stu-id="93b08-130">String</span></span>| <span data-ttu-id="93b08-131">Serviço ou recurso do Microsoft Online que tem uma dependência nesse registro TXT.</span><span class="sxs-lookup"><span data-stu-id="93b08-131">Microsoft Online Service or feature that has a dependency on this TXT record.</span></span></br></br><span data-ttu-id="93b08-132">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="93b08-132">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span> |
|<span data-ttu-id="93b08-133">texto</span><span class="sxs-lookup"><span data-stu-id="93b08-133">text</span></span>|<span data-ttu-id="93b08-134">String</span><span class="sxs-lookup"><span data-stu-id="93b08-134">String</span></span>| <span data-ttu-id="93b08-135">Valor usado ao configurar a *propriedade de texto* no host DNS.</span><span class="sxs-lookup"><span data-stu-id="93b08-135">Value used when configuring the *text* property at the DNS host.</span></span> |
|<span data-ttu-id="93b08-136">ttl</span><span class="sxs-lookup"><span data-stu-id="93b08-136">ttl</span></span>|<span data-ttu-id="93b08-137">Int32</span><span class="sxs-lookup"><span data-stu-id="93b08-137">Int32</span></span>| <span data-ttu-id="93b08-138">Valor a ser usado ao configurar a *propriedade time-to-live (ttl)* do registro MX no host DNS.</span><span class="sxs-lookup"><span data-stu-id="93b08-138">Value to use when configuring the *time-to-live (ttl)* property of the MX record at the DNS host.</span></span> <span data-ttu-id="93b08-139">Não anulada</span><span class="sxs-lookup"><span data-stu-id="93b08-139">Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="93b08-140">Relações</span><span class="sxs-lookup"><span data-stu-id="93b08-140">Relationships</span></span>
<span data-ttu-id="93b08-141">Nenhum</span><span class="sxs-lookup"><span data-stu-id="93b08-141">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="93b08-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="93b08-142">JSON representation</span></span>
<span data-ttu-id="93b08-143">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="93b08-143">Here is a JSON representation of the resource.</span></span>

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

