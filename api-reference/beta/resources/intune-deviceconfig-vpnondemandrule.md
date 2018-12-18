---
title: tipo de recurso de vpnOnDemandRule
description: Definição de regra de sob demanda de VPN.
author: tfitzmac
ms.openlocfilehash: 72b85971dc9c613026bb9e720ca55165845e0c9e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27352189"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="22e51-103">tipo de recurso de vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="22e51-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="22e51-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="22e51-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22e51-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="22e51-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22e51-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="22e51-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22e51-107">Definição de regra de sob demanda de VPN.</span><span class="sxs-lookup"><span data-stu-id="22e51-107">VPN On-Demand Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="22e51-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="22e51-108">Properties</span></span>
|<span data-ttu-id="22e51-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="22e51-109">Property</span></span>|<span data-ttu-id="22e51-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="22e51-110">Type</span></span>|<span data-ttu-id="22e51-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="22e51-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22e51-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="22e51-112">ssids</span></span>|<span data-ttu-id="22e51-113">String collection</span><span class="sxs-lookup"><span data-stu-id="22e51-113">String collection</span></span>|<span data-ttu-id="22e51-114">Identificadores (SSIDs) do conjunto de serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="22e51-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="22e51-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="22e51-115">dnsSearchDomains</span></span>|<span data-ttu-id="22e51-116">String collection</span><span class="sxs-lookup"><span data-stu-id="22e51-116">String collection</span></span>|<span data-ttu-id="22e51-117">Domínios de pesquisa DNS.</span><span class="sxs-lookup"><span data-stu-id="22e51-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="22e51-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="22e51-118">probeUrl</span></span>|<span data-ttu-id="22e51-119">String</span><span class="sxs-lookup"><span data-stu-id="22e51-119">String</span></span>|<span data-ttu-id="22e51-120">Uma URL para teste.</span><span class="sxs-lookup"><span data-stu-id="22e51-120">A URL to probe.</span></span> <span data-ttu-id="22e51-121">Se essa URL é com êxito procurada (retornando um código de status HTTP 200) sem redirecionamento, correspondentes a esta regra.</span><span class="sxs-lookup"><span data-stu-id="22e51-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="22e51-122">action</span><span class="sxs-lookup"><span data-stu-id="22e51-122">action</span></span>|[<span data-ttu-id="22e51-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="22e51-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="22e51-124">Ação.</span><span class="sxs-lookup"><span data-stu-id="22e51-124">Action.</span></span> <span data-ttu-id="22e51-125">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="22e51-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="22e51-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="22e51-126">domainAction</span></span>|[<span data-ttu-id="22e51-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="22e51-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="22e51-128">Ação de domínio (aplicável somente quando a ação é avaliar a conexão).</span><span class="sxs-lookup"><span data-stu-id="22e51-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="22e51-129">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="22e51-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="22e51-130">domínios</span><span class="sxs-lookup"><span data-stu-id="22e51-130">domains</span></span>|<span data-ttu-id="22e51-131">String collection</span><span class="sxs-lookup"><span data-stu-id="22e51-131">String collection</span></span>|<span data-ttu-id="22e51-132">Domínios (aplicáveis somente quando a ação é avaliar a conexão).</span><span class="sxs-lookup"><span data-stu-id="22e51-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="22e51-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="22e51-133">probeRequiredUrl</span></span>|<span data-ttu-id="22e51-134">String</span><span class="sxs-lookup"><span data-stu-id="22e51-134">String</span></span>|<span data-ttu-id="22e51-135">Investigue obrigatório Url (aplicável somente quando a ação é avaliar a conexão e DomainAction é conectar, se necessário).</span><span class="sxs-lookup"><span data-stu-id="22e51-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="22e51-136">Relações</span><span class="sxs-lookup"><span data-stu-id="22e51-136">Relationships</span></span>
<span data-ttu-id="22e51-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="22e51-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="22e51-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="22e51-138">JSON Representation</span></span>
<span data-ttu-id="22e51-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="22e51-139">Here is a JSON representation of the resource.</span></span>
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





