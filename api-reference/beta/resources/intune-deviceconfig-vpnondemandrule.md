---
title: tipo de recurso vpnOnDemandRule
description: Definição de regra VPN sob demanda.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd5724e4c2c1cfb5ca185dd8420011853812305a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412144"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="1d559-103">tipo de recurso vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="1d559-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="1d559-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1d559-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1d559-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d559-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d559-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d559-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d559-107">Definição de regra VPN sob demanda.</span><span class="sxs-lookup"><span data-stu-id="1d559-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="1d559-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1d559-108">Properties</span></span>
|<span data-ttu-id="1d559-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d559-109">Property</span></span>|<span data-ttu-id="1d559-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d559-110">Type</span></span>|<span data-ttu-id="1d559-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d559-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d559-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="1d559-112">ssids</span></span>|<span data-ttu-id="1d559-113">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1d559-113">String collection</span></span>|<span data-ttu-id="1d559-114">Identificadores de conjuntos de serviços de rede (SSIDs).</span><span class="sxs-lookup"><span data-stu-id="1d559-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="1d559-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="1d559-115">dnsSearchDomains</span></span>|<span data-ttu-id="1d559-116">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1d559-116">String collection</span></span>|<span data-ttu-id="1d559-117">Domínios de pesquisa de DNS.</span><span class="sxs-lookup"><span data-stu-id="1d559-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="1d559-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="1d559-118">probeUrl</span></span>|<span data-ttu-id="1d559-119">String</span><span class="sxs-lookup"><span data-stu-id="1d559-119">String</span></span>|<span data-ttu-id="1d559-120">Uma URL para sondar.</span><span class="sxs-lookup"><span data-stu-id="1d559-120">A URL to probe.</span></span> <span data-ttu-id="1d559-121">Se essa URL for obtida com êxito (retornando um código de status HTTP 200) sem redirecionamento, essa regra será correspondente.</span><span class="sxs-lookup"><span data-stu-id="1d559-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="1d559-122">ação</span><span class="sxs-lookup"><span data-stu-id="1d559-122">action</span></span>|[<span data-ttu-id="1d559-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="1d559-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="1d559-124">Ação.</span><span class="sxs-lookup"><span data-stu-id="1d559-124">Action.</span></span> <span data-ttu-id="1d559-125">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="1d559-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="1d559-126">domainaction</span><span class="sxs-lookup"><span data-stu-id="1d559-126">domainAction</span></span>|[<span data-ttu-id="1d559-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="1d559-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="1d559-128">Ação de domínio (aplicável somente quando a ação é avaliar conexão).</span><span class="sxs-lookup"><span data-stu-id="1d559-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="1d559-129">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="1d559-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="1d559-130">domínio</span><span class="sxs-lookup"><span data-stu-id="1d559-130">domains</span></span>|<span data-ttu-id="1d559-131">Coleção String</span><span class="sxs-lookup"><span data-stu-id="1d559-131">String collection</span></span>|<span data-ttu-id="1d559-132">Domains (só é aplicável quando Action é Evaluate Connection).</span><span class="sxs-lookup"><span data-stu-id="1d559-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="1d559-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="1d559-133">probeRequiredUrl</span></span>|<span data-ttu-id="1d559-134">String</span><span class="sxs-lookup"><span data-stu-id="1d559-134">String</span></span>|<span data-ttu-id="1d559-135">A URL obrigatória da sonda (aplicável somente quando Action é Evaluate Connection e domainaction é conectada se necessário).</span><span class="sxs-lookup"><span data-stu-id="1d559-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1d559-136">Relações</span><span class="sxs-lookup"><span data-stu-id="1d559-136">Relationships</span></span>
<span data-ttu-id="1d559-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1d559-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1d559-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1d559-138">JSON Representation</span></span>
<span data-ttu-id="1d559-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1d559-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnOnDemandRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnOnDemandRule",
  "ssids": [
    "String"
  ],
  "dnsSearchDomains": [
    "String"
  ],
  "probeUrl": "String",
  "action": "String",
  "domainAction": "String",
  "domains": [
    "String"
  ],
  "probeRequiredUrl": "String"
}
```



