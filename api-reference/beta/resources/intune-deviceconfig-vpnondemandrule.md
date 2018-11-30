---
title: tipo de recurso de vpnOnDemandRule
description: Definição de regra de sob demanda de VPN.
ms.openlocfilehash: 366dd373d31b04d4f245c2394a7a6e476710cf84
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035201"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="1f76c-103">tipo de recurso de vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="1f76c-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="1f76c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f76c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f76c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f76c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f76c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f76c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f76c-107">Definição de regra de sob demanda de VPN.</span><span class="sxs-lookup"><span data-stu-id="1f76c-107">VPN On-Demand Rule definition.</span></span>
## <a name="properties"></a><span data-ttu-id="1f76c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f76c-108">Properties</span></span>
|<span data-ttu-id="1f76c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f76c-109">Property</span></span>|<span data-ttu-id="1f76c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f76c-110">Type</span></span>|<span data-ttu-id="1f76c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f76c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f76c-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="1f76c-112">ssids</span></span>|<span data-ttu-id="1f76c-113">String collection</span><span class="sxs-lookup"><span data-stu-id="1f76c-113">String collection</span></span>|<span data-ttu-id="1f76c-114">Identificadores (SSIDs) do conjunto de serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="1f76c-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="1f76c-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="1f76c-115">dnsSearchDomains</span></span>|<span data-ttu-id="1f76c-116">String collection</span><span class="sxs-lookup"><span data-stu-id="1f76c-116">String collection</span></span>|<span data-ttu-id="1f76c-117">Domínios de pesquisa DNS.</span><span class="sxs-lookup"><span data-stu-id="1f76c-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="1f76c-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="1f76c-118">probeUrl</span></span>|<span data-ttu-id="1f76c-119">String</span><span class="sxs-lookup"><span data-stu-id="1f76c-119">String</span></span>|<span data-ttu-id="1f76c-120">Uma URL para teste.</span><span class="sxs-lookup"><span data-stu-id="1f76c-120">A URL to probe.</span></span> <span data-ttu-id="1f76c-121">Se essa URL é com êxito procurada (retornando um código de status HTTP 200) sem redirecionamento, correspondentes a esta regra.</span><span class="sxs-lookup"><span data-stu-id="1f76c-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="1f76c-122">action</span><span class="sxs-lookup"><span data-stu-id="1f76c-122">action</span></span>|[<span data-ttu-id="1f76c-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="1f76c-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="1f76c-124">Ação.</span><span class="sxs-lookup"><span data-stu-id="1f76c-124">Action.</span></span> <span data-ttu-id="1f76c-125">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="1f76c-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="1f76c-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="1f76c-126">domainAction</span></span>|[<span data-ttu-id="1f76c-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="1f76c-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="1f76c-128">Ação de domínio (aplicável somente quando a ação é avaliar a conexão).</span><span class="sxs-lookup"><span data-stu-id="1f76c-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="1f76c-129">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="1f76c-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="1f76c-130">domínios</span><span class="sxs-lookup"><span data-stu-id="1f76c-130">domains</span></span>|<span data-ttu-id="1f76c-131">String collection</span><span class="sxs-lookup"><span data-stu-id="1f76c-131">String collection</span></span>|<span data-ttu-id="1f76c-132">Domínios (aplicáveis somente quando a ação é avaliar a conexão).</span><span class="sxs-lookup"><span data-stu-id="1f76c-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="1f76c-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="1f76c-133">probeRequiredUrl</span></span>|<span data-ttu-id="1f76c-134">String</span><span class="sxs-lookup"><span data-stu-id="1f76c-134">String</span></span>|<span data-ttu-id="1f76c-135">Investigue obrigatório Url (aplicável somente quando a ação é avaliar a conexão e DomainAction é conectar, se necessário).</span><span class="sxs-lookup"><span data-stu-id="1f76c-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f76c-136">Relações</span><span class="sxs-lookup"><span data-stu-id="1f76c-136">Relationships</span></span>
<span data-ttu-id="1f76c-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f76c-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f76c-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f76c-138">JSON Representation</span></span>
<span data-ttu-id="1f76c-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f76c-139">Here is a JSON representation of the resource.</span></span>
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





