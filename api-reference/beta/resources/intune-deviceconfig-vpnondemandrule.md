---
title: tipo de recurso vpnOnDemandRule
description: Definição de regra VPN sob demanda.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c75a8b725c95449868767ce6a08a43876c16ab62
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525765"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="517cd-103">tipo de recurso vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="517cd-103">vpnOnDemandRule resource type</span></span>

<span data-ttu-id="517cd-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="517cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="517cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="517cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="517cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="517cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="517cd-107">Definição de regra VPN sob demanda.</span><span class="sxs-lookup"><span data-stu-id="517cd-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="517cd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="517cd-108">Properties</span></span>
|<span data-ttu-id="517cd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="517cd-109">Property</span></span>|<span data-ttu-id="517cd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="517cd-110">Type</span></span>|<span data-ttu-id="517cd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="517cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="517cd-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="517cd-112">ssids</span></span>|<span data-ttu-id="517cd-113">String collection</span><span class="sxs-lookup"><span data-stu-id="517cd-113">String collection</span></span>|<span data-ttu-id="517cd-114">Identificadores de conjuntos de serviços de rede (SSIDs).</span><span class="sxs-lookup"><span data-stu-id="517cd-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="517cd-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="517cd-115">dnsSearchDomains</span></span>|<span data-ttu-id="517cd-116">String collection</span><span class="sxs-lookup"><span data-stu-id="517cd-116">String collection</span></span>|<span data-ttu-id="517cd-117">Domínios de pesquisa de DNS.</span><span class="sxs-lookup"><span data-stu-id="517cd-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="517cd-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="517cd-118">probeUrl</span></span>|<span data-ttu-id="517cd-119">String</span><span class="sxs-lookup"><span data-stu-id="517cd-119">String</span></span>|<span data-ttu-id="517cd-120">Uma URL para sondar.</span><span class="sxs-lookup"><span data-stu-id="517cd-120">A URL to probe.</span></span> <span data-ttu-id="517cd-121">Se essa URL for obtida com êxito (retornando um código de status HTTP 200) sem redirecionamento, essa regra será correspondente.</span><span class="sxs-lookup"><span data-stu-id="517cd-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="517cd-122">ação</span><span class="sxs-lookup"><span data-stu-id="517cd-122">action</span></span>|[<span data-ttu-id="517cd-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="517cd-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="517cd-124">Ação.</span><span class="sxs-lookup"><span data-stu-id="517cd-124">Action.</span></span> <span data-ttu-id="517cd-125">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="517cd-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="517cd-126">domainaction</span><span class="sxs-lookup"><span data-stu-id="517cd-126">domainAction</span></span>|[<span data-ttu-id="517cd-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="517cd-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="517cd-128">Ação de domínio (aplicável somente quando a ação é avaliar conexão).</span><span class="sxs-lookup"><span data-stu-id="517cd-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="517cd-129">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="517cd-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="517cd-130">domínio</span><span class="sxs-lookup"><span data-stu-id="517cd-130">domains</span></span>|<span data-ttu-id="517cd-131">String collection</span><span class="sxs-lookup"><span data-stu-id="517cd-131">String collection</span></span>|<span data-ttu-id="517cd-132">Domains (só é aplicável quando Action é Evaluate Connection).</span><span class="sxs-lookup"><span data-stu-id="517cd-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="517cd-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="517cd-133">probeRequiredUrl</span></span>|<span data-ttu-id="517cd-134">String</span><span class="sxs-lookup"><span data-stu-id="517cd-134">String</span></span>|<span data-ttu-id="517cd-135">A URL obrigatória da sonda (aplicável somente quando Action é Evaluate Connection e domainaction é conectada se necessário).</span><span class="sxs-lookup"><span data-stu-id="517cd-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="517cd-136">Relações</span><span class="sxs-lookup"><span data-stu-id="517cd-136">Relationships</span></span>
<span data-ttu-id="517cd-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="517cd-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="517cd-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="517cd-138">JSON Representation</span></span>
<span data-ttu-id="517cd-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="517cd-139">Here is a JSON representation of the resource.</span></span>
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



