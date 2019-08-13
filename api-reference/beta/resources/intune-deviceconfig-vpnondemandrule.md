---
title: tipo de recurso vpnOnDemandRule
description: Definição de regra VPN sob demanda.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f7b562f9f1be09c5214905e67b2a8ac604e03f20
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367663"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="3ae74-103">tipo de recurso vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="3ae74-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="3ae74-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3ae74-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ae74-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3ae74-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ae74-106">Definição de regra VPN sob demanda.</span><span class="sxs-lookup"><span data-stu-id="3ae74-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="3ae74-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3ae74-107">Properties</span></span>
|<span data-ttu-id="3ae74-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3ae74-108">Property</span></span>|<span data-ttu-id="3ae74-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="3ae74-109">Type</span></span>|<span data-ttu-id="3ae74-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3ae74-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ae74-111">SSIDs</span><span class="sxs-lookup"><span data-stu-id="3ae74-111">ssids</span></span>|<span data-ttu-id="3ae74-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ae74-112">String collection</span></span>|<span data-ttu-id="3ae74-113">Identificadores de conjuntos de serviços de rede (SSIDs).</span><span class="sxs-lookup"><span data-stu-id="3ae74-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="3ae74-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="3ae74-114">dnsSearchDomains</span></span>|<span data-ttu-id="3ae74-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ae74-115">String collection</span></span>|<span data-ttu-id="3ae74-116">Domínios de pesquisa de DNS.</span><span class="sxs-lookup"><span data-stu-id="3ae74-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="3ae74-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="3ae74-117">probeUrl</span></span>|<span data-ttu-id="3ae74-118">String</span><span class="sxs-lookup"><span data-stu-id="3ae74-118">String</span></span>|<span data-ttu-id="3ae74-119">Uma URL para sondar.</span><span class="sxs-lookup"><span data-stu-id="3ae74-119">A URL to probe.</span></span> <span data-ttu-id="3ae74-120">Se essa URL for obtida com êxito (retornando um código de status HTTP 200) sem redirecionamento, essa regra será correspondente.</span><span class="sxs-lookup"><span data-stu-id="3ae74-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="3ae74-121">ação</span><span class="sxs-lookup"><span data-stu-id="3ae74-121">action</span></span>|[<span data-ttu-id="3ae74-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="3ae74-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="3ae74-123">Ação.</span><span class="sxs-lookup"><span data-stu-id="3ae74-123">Action.</span></span> <span data-ttu-id="3ae74-124">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="3ae74-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="3ae74-125">domainaction</span><span class="sxs-lookup"><span data-stu-id="3ae74-125">domainAction</span></span>|[<span data-ttu-id="3ae74-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="3ae74-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="3ae74-127">Ação de domínio (aplicável somente quando a ação é avaliar conexão).</span><span class="sxs-lookup"><span data-stu-id="3ae74-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="3ae74-128">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="3ae74-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="3ae74-129">domínio</span><span class="sxs-lookup"><span data-stu-id="3ae74-129">domains</span></span>|<span data-ttu-id="3ae74-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="3ae74-130">String collection</span></span>|<span data-ttu-id="3ae74-131">Domains (só é aplicável quando Action é Evaluate Connection).</span><span class="sxs-lookup"><span data-stu-id="3ae74-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="3ae74-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="3ae74-132">probeRequiredUrl</span></span>|<span data-ttu-id="3ae74-133">String</span><span class="sxs-lookup"><span data-stu-id="3ae74-133">String</span></span>|<span data-ttu-id="3ae74-134">A URL obrigatória da sonda (aplicável somente quando Action é Evaluate Connection e domainaction é conectada se necessário).</span><span class="sxs-lookup"><span data-stu-id="3ae74-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="3ae74-135">Relações</span><span class="sxs-lookup"><span data-stu-id="3ae74-135">Relationships</span></span>
<span data-ttu-id="3ae74-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3ae74-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3ae74-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3ae74-137">JSON Representation</span></span>
<span data-ttu-id="3ae74-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3ae74-138">Here is a JSON representation of the resource.</span></span>
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



