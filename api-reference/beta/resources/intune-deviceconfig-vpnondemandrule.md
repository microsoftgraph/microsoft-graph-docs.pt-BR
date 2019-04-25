---
title: tipo de recurso vpnOnDemandRule
description: Definição de regra VPN sob demanda.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3209c91400b36adba772273cfa6768049adce448
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561926"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="7ac1c-103">tipo de recurso vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="7ac1c-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="7ac1c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7ac1c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ac1c-106">Definição de regra VPN sob demanda.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-106">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="7ac1c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7ac1c-107">Properties</span></span>
|<span data-ttu-id="7ac1c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7ac1c-108">Property</span></span>|<span data-ttu-id="7ac1c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7ac1c-109">Type</span></span>|<span data-ttu-id="7ac1c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7ac1c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ac1c-111">SSIDs</span><span class="sxs-lookup"><span data-stu-id="7ac1c-111">ssids</span></span>|<span data-ttu-id="7ac1c-112">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac1c-112">String collection</span></span>|<span data-ttu-id="7ac1c-113">Identificadores de conjuntos de serviços de rede (SSIDs).</span><span class="sxs-lookup"><span data-stu-id="7ac1c-113">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="7ac1c-114">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="7ac1c-114">dnsSearchDomains</span></span>|<span data-ttu-id="7ac1c-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac1c-115">String collection</span></span>|<span data-ttu-id="7ac1c-116">Domínios de pesquisa de DNS.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-116">DNS Search Domains.</span></span>|
|<span data-ttu-id="7ac1c-117">probeUrl</span><span class="sxs-lookup"><span data-stu-id="7ac1c-117">probeUrl</span></span>|<span data-ttu-id="7ac1c-118">String</span><span class="sxs-lookup"><span data-stu-id="7ac1c-118">String</span></span>|<span data-ttu-id="7ac1c-119">Uma URL para sondar.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-119">A URL to probe.</span></span> <span data-ttu-id="7ac1c-120">Se essa URL for obtida com êxito (retornando um código de status HTTP 200) sem redirecionamento, essa regra será correspondente.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-120">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="7ac1c-121">ação</span><span class="sxs-lookup"><span data-stu-id="7ac1c-121">action</span></span>|[<span data-ttu-id="7ac1c-122">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="7ac1c-122">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="7ac1c-123">Ação.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-123">Action.</span></span> <span data-ttu-id="7ac1c-124">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-124">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="7ac1c-125">domainaction</span><span class="sxs-lookup"><span data-stu-id="7ac1c-125">domainAction</span></span>|[<span data-ttu-id="7ac1c-126">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="7ac1c-126">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="7ac1c-127">Ação de domínio (aplicável somente quando a ação é avaliar conexão).</span><span class="sxs-lookup"><span data-stu-id="7ac1c-127">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="7ac1c-128">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-128">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="7ac1c-129">domínio</span><span class="sxs-lookup"><span data-stu-id="7ac1c-129">domains</span></span>|<span data-ttu-id="7ac1c-130">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="7ac1c-130">String collection</span></span>|<span data-ttu-id="7ac1c-131">Domains (só é aplicável quando Action é Evaluate Connection).</span><span class="sxs-lookup"><span data-stu-id="7ac1c-131">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="7ac1c-132">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="7ac1c-132">probeRequiredUrl</span></span>|<span data-ttu-id="7ac1c-133">String</span><span class="sxs-lookup"><span data-stu-id="7ac1c-133">String</span></span>|<span data-ttu-id="7ac1c-134">A URL obrigatória da sonda (aplicável somente quando Action é Evaluate Connection e domainaction é conectada se necessário).</span><span class="sxs-lookup"><span data-stu-id="7ac1c-134">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="7ac1c-135">Relações</span><span class="sxs-lookup"><span data-stu-id="7ac1c-135">Relationships</span></span>
<span data-ttu-id="7ac1c-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7ac1c-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7ac1c-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7ac1c-137">JSON Representation</span></span>
<span data-ttu-id="7ac1c-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7ac1c-138">Here is a JSON representation of the resource.</span></span>
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





