---
title: Tipo de recurso domainDnsRecord
description: Para cada domínio no locatário, talvez seja necessário adicionar registro (s) DNS para o arquivo de zona DNS do domínio para que o domínio que possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. Entidade base para entidades DomainDnsCnameRecord, DomainDnsMxRecord, DomainDnsSrvRecord e DomainDnsSrvRecord.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: f5c760ba9a2100bbefd0353c2c02019e7a04354b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912957"
---
# <a name="domaindnsrecord-resource-type"></a><span data-ttu-id="fa902-105">Tipo de recurso domainDnsRecord</span><span class="sxs-lookup"><span data-stu-id="fa902-105">domainDnsRecord resource type</span></span>

> <span data-ttu-id="fa902-106">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="fa902-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa902-107">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fa902-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fa902-p103">Para cada domínio no locatário, talvez seja necessário adicionar os registros DNS ao arquivo de zona DNS do domínio para que ele possa ser usado pelo Microsoft Online Services. A entidade **DomainDnsRecord** é usada para apresentar esses registros DNS. A entidade base das entidades [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) e [DomainDnsSrvRecord](domaindnssrvrecord.md).</span><span class="sxs-lookup"><span data-stu-id="fa902-p103">For each domain in the tenant, you may be required to add DNS record(s) to the DNS zone file of the domain before the domain can be used by Microsoft Online Services. The **DomainDnsRecord** entity is used to present such DNS records. Base entity for [DomainDnsCnameRecord](domaindnscnamerecord.md), [DomainDnsMxRecord](domaindnsmxrecord.md), [DomainDnsSrvRecord](domaindnssrvrecord.md) and [DomainDnsSrvRecord](domaindnssrvrecord.md) entities.</span></span>

## <a name="methods"></a><span data-ttu-id="fa902-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="fa902-111">Methods</span></span>
<span data-ttu-id="fa902-p104">Não há suporte a consultas diretas para este recurso. Confira o tópico do [domínio](domain.md) para obter informações sobre como consultar registros de serviços do domínio.</span><span class="sxs-lookup"><span data-stu-id="fa902-p104">Direct queries to this resource are not supported. Please see the [domain](domain.md) topic for information on how to query for domain service records.</span></span>

## <a name="properties"></a><span data-ttu-id="fa902-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="fa902-114">Properties</span></span>
| <span data-ttu-id="fa902-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fa902-115">Property</span></span>     | <span data-ttu-id="fa902-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="fa902-116">Type</span></span>   |<span data-ttu-id="fa902-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="fa902-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fa902-118">id</span><span class="sxs-lookup"><span data-stu-id="fa902-118">id</span></span>|<span data-ttu-id="fa902-119">String</span><span class="sxs-lookup"><span data-stu-id="fa902-119">String</span></span>| <span data-ttu-id="fa902-p105">Identificador exclusivo atribuído a esta entidade. Não anulável, Somente Leitura.</span><span class="sxs-lookup"><span data-stu-id="fa902-p105">Unique identifier assigned to this entity. Not nullable, Read-only.</span></span>|
|<span data-ttu-id="fa902-122">isOptional</span><span class="sxs-lookup"><span data-stu-id="fa902-122">isOptional</span></span>|<span data-ttu-id="fa902-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="fa902-123">Boolean</span></span>| <span data-ttu-id="fa902-124">Se for falso, o registro deve ser configurado pelo cliente no host DNS do Microsoft Online Services para funcionar corretamente com o domínio.</span><span class="sxs-lookup"><span data-stu-id="fa902-124">If false, this record must be configured by the customer at the DNS host for Microsoft Online Services to operate correctly with the domain.</span></span> |
|<span data-ttu-id="fa902-125">rótulo</span><span class="sxs-lookup"><span data-stu-id="fa902-125">label</span></span>|<span data-ttu-id="fa902-126">String</span><span class="sxs-lookup"><span data-stu-id="fa902-126">String</span></span>| <span data-ttu-id="fa902-127">O valor usado ao configurar o nome da propriedade do registro DNS no host DNS.</span><span class="sxs-lookup"><span data-stu-id="fa902-127">Value used when configuring the name of the DNS record at the DNS host.</span></span> |
|<span data-ttu-id="fa902-128">recordType</span><span class="sxs-lookup"><span data-stu-id="fa902-128">recordType</span></span>|<span data-ttu-id="fa902-129">String</span><span class="sxs-lookup"><span data-stu-id="fa902-129">String</span></span>| <span data-ttu-id="fa902-130">Indica que tipo de registro DNS a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="fa902-130">Indicates what type of DNS record this entity represents.</span></span></br></br><span data-ttu-id="fa902-131">O valor pode ser um dos seguintes: *CName*, *Mx*, *Srv* e *Txt*</span><span class="sxs-lookup"><span data-stu-id="fa902-131">The value can be one of the following: *CName*, *Mx*, *Srv*, *Txt*</span></span></br></br><span data-ttu-id="fa902-132">Chave</span><span class="sxs-lookup"><span data-stu-id="fa902-132">Key</span></span> |
|<span data-ttu-id="fa902-133">supportedService</span><span class="sxs-lookup"><span data-stu-id="fa902-133">supportedService</span></span>|<span data-ttu-id="fa902-134">String</span><span class="sxs-lookup"><span data-stu-id="fa902-134">String</span></span>| <span data-ttu-id="fa902-135">O Microsoft Online Services ou o recurso que tiver uma dependência neste registro DNS.</span><span class="sxs-lookup"><span data-stu-id="fa902-135">Microsoft Online Service or feature that has a dependency on this DNS record.</span></span></br></br><span data-ttu-id="fa902-136">Pode ser um dos seguintes valores: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span><span class="sxs-lookup"><span data-stu-id="fa902-136">Can be one of the following values: **null**, *Email*, *Sharepoint*, *EmailInternalRelayOnly*, *OfficeCommunicationsOnline*, *SharePointDefaultDomain*, *FullRedelegation*, *SharePointPublic*, *OrgIdAuthentication*, *Yammer*, *Intune*</span></span>|
|<span data-ttu-id="fa902-137">ttl</span><span class="sxs-lookup"><span data-stu-id="fa902-137">ttl</span></span>|<span data-ttu-id="fa902-138">Int32</span><span class="sxs-lookup"><span data-stu-id="fa902-138">Int32</span></span>| <span data-ttu-id="fa902-p106">O valor a ser usado ao configurar a propriedade time-to-live (ttl) do registro DNS no host DNS. Não anulável</span><span class="sxs-lookup"><span data-stu-id="fa902-p106">Value to use when configuring the time-to-live (ttl) property of the DNS record at the DNS host. Not nullable</span></span> |

## <a name="relationships"></a><span data-ttu-id="fa902-141">Relações</span><span class="sxs-lookup"><span data-stu-id="fa902-141">Relationships</span></span>
<span data-ttu-id="fa902-142">Nenhum</span><span class="sxs-lookup"><span data-stu-id="fa902-142">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="fa902-143">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="fa902-143">JSON representation</span></span>
<span data-ttu-id="fa902-144">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="fa902-144">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainDnsRecord"
}-->

```json
{
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
  "description": "domainDnsRecord resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
