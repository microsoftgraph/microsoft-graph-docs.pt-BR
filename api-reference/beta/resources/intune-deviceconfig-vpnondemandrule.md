---
title: tipo de recurso de vpnOnDemandRule
description: Definição de regra de sob demanda de VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8164d1c12aeb172120bb9803d7f3dd98366ec948
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421456"
---
# <a name="vpnondemandrule-resource-type"></a><span data-ttu-id="da022-103">tipo de recurso de vpnOnDemandRule</span><span class="sxs-lookup"><span data-stu-id="da022-103">vpnOnDemandRule resource type</span></span>

> <span data-ttu-id="da022-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="da022-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="da022-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="da022-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da022-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="da022-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da022-107">Definição de regra de sob demanda de VPN.</span><span class="sxs-lookup"><span data-stu-id="da022-107">VPN On-Demand Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="da022-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da022-108">Properties</span></span>
|<span data-ttu-id="da022-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da022-109">Property</span></span>|<span data-ttu-id="da022-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da022-110">Type</span></span>|<span data-ttu-id="da022-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da022-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da022-112">SSIDs</span><span class="sxs-lookup"><span data-stu-id="da022-112">ssids</span></span>|<span data-ttu-id="da022-113">String collection</span><span class="sxs-lookup"><span data-stu-id="da022-113">String collection</span></span>|<span data-ttu-id="da022-114">Identificadores (SSIDs) do conjunto de serviço de rede.</span><span class="sxs-lookup"><span data-stu-id="da022-114">Network Service Set Identifiers (SSIDs).</span></span>|
|<span data-ttu-id="da022-115">dnsSearchDomains</span><span class="sxs-lookup"><span data-stu-id="da022-115">dnsSearchDomains</span></span>|<span data-ttu-id="da022-116">String collection</span><span class="sxs-lookup"><span data-stu-id="da022-116">String collection</span></span>|<span data-ttu-id="da022-117">Domínios de pesquisa DNS.</span><span class="sxs-lookup"><span data-stu-id="da022-117">DNS Search Domains.</span></span>|
|<span data-ttu-id="da022-118">probeUrl</span><span class="sxs-lookup"><span data-stu-id="da022-118">probeUrl</span></span>|<span data-ttu-id="da022-119">String</span><span class="sxs-lookup"><span data-stu-id="da022-119">String</span></span>|<span data-ttu-id="da022-120">Uma URL para teste.</span><span class="sxs-lookup"><span data-stu-id="da022-120">A URL to probe.</span></span> <span data-ttu-id="da022-121">Se essa URL é com êxito procurada (retornando um código de status HTTP 200) sem redirecionamento, correspondentes a esta regra.</span><span class="sxs-lookup"><span data-stu-id="da022-121">If this URL is successfully fetched (returning a 200 HTTP status code) without redirection, this rule matches.</span></span>|
|<span data-ttu-id="da022-122">action</span><span class="sxs-lookup"><span data-stu-id="da022-122">action</span></span>|[<span data-ttu-id="da022-123">vpnOnDemandRuleConnectionAction</span><span class="sxs-lookup"><span data-stu-id="da022-123">vpnOnDemandRuleConnectionAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectionaction.md)|<span data-ttu-id="da022-124">Ação.</span><span class="sxs-lookup"><span data-stu-id="da022-124">Action.</span></span> <span data-ttu-id="da022-125">Os valores possíveis são: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span><span class="sxs-lookup"><span data-stu-id="da022-125">Possible values are: `connect`, `evaluateConnection`, `ignore`, `disconnect`.</span></span>|
|<span data-ttu-id="da022-126">domainAction</span><span class="sxs-lookup"><span data-stu-id="da022-126">domainAction</span></span>|[<span data-ttu-id="da022-127">vpnOnDemandRuleConnectionDomainAction</span><span class="sxs-lookup"><span data-stu-id="da022-127">vpnOnDemandRuleConnectionDomainAction</span></span>](../resources/intune-deviceconfig-vpnondemandruleconnectiondomainaction.md)|<span data-ttu-id="da022-128">Ação de domínio (aplicável somente quando a ação é avaliar a conexão).</span><span class="sxs-lookup"><span data-stu-id="da022-128">Domain Action (Only applicable when Action is evaluate connection).</span></span> <span data-ttu-id="da022-129">Os valores possíveis são: `connectIfNeeded` e `neverConnect`.</span><span class="sxs-lookup"><span data-stu-id="da022-129">Possible values are: `connectIfNeeded`, `neverConnect`.</span></span>|
|<span data-ttu-id="da022-130">domínios</span><span class="sxs-lookup"><span data-stu-id="da022-130">domains</span></span>|<span data-ttu-id="da022-131">String collection</span><span class="sxs-lookup"><span data-stu-id="da022-131">String collection</span></span>|<span data-ttu-id="da022-132">Domínios (aplicáveis somente quando a ação é avaliar a conexão).</span><span class="sxs-lookup"><span data-stu-id="da022-132">Domains (Only applicable when Action is evaluate connection).</span></span>|
|<span data-ttu-id="da022-133">probeRequiredUrl</span><span class="sxs-lookup"><span data-stu-id="da022-133">probeRequiredUrl</span></span>|<span data-ttu-id="da022-134">String</span><span class="sxs-lookup"><span data-stu-id="da022-134">String</span></span>|<span data-ttu-id="da022-135">Investigue obrigatório Url (aplicável somente quando a ação é avaliar a conexão e DomainAction é conectar, se necessário).</span><span class="sxs-lookup"><span data-stu-id="da022-135">Probe Required Url (Only applicable when Action is evaluate connection and DomainAction is connect if needed).</span></span>|

## <a name="relationships"></a><span data-ttu-id="da022-136">Relações</span><span class="sxs-lookup"><span data-stu-id="da022-136">Relationships</span></span>
<span data-ttu-id="da022-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da022-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da022-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da022-138">JSON Representation</span></span>
<span data-ttu-id="da022-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da022-139">Here is a JSON representation of the resource.</span></span>
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




