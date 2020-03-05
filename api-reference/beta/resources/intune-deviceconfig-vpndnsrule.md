---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f110538f61dc16110956b05cdf42a9af85e9e542
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525779"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="d2bf6-103">tipo de recurso vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="d2bf6-103">vpnDnsRule resource type</span></span>

<span data-ttu-id="d2bf6-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d2bf6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d2bf6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2bf6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2bf6-107">Definição de regra DNS de VPN.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="d2bf6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d2bf6-108">Properties</span></span>
|<span data-ttu-id="d2bf6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d2bf6-109">Property</span></span>|<span data-ttu-id="d2bf6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d2bf6-110">Type</span></span>|<span data-ttu-id="d2bf6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d2bf6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2bf6-112">nome</span><span class="sxs-lookup"><span data-stu-id="d2bf6-112">name</span></span>|<span data-ttu-id="d2bf6-113">String</span><span class="sxs-lookup"><span data-stu-id="d2bf6-113">String</span></span>|<span data-ttu-id="d2bf6-114">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-114">Name.</span></span>|
|<span data-ttu-id="d2bf6-115">servidores</span><span class="sxs-lookup"><span data-stu-id="d2bf6-115">servers</span></span>|<span data-ttu-id="d2bf6-116">String collection</span><span class="sxs-lookup"><span data-stu-id="d2bf6-116">String collection</span></span>|<span data-ttu-id="d2bf6-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-117">Servers.</span></span>|
|<span data-ttu-id="d2bf6-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="d2bf6-118">proxyServerUri</span></span>|<span data-ttu-id="d2bf6-119">String</span><span class="sxs-lookup"><span data-stu-id="d2bf6-119">String</span></span>|<span data-ttu-id="d2bf6-120">URI do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="d2bf6-121">Gatilho autotrigger</span><span class="sxs-lookup"><span data-stu-id="d2bf6-121">autoTrigger</span></span>|<span data-ttu-id="d2bf6-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2bf6-122">Boolean</span></span>|<span data-ttu-id="d2bf6-123">Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="d2bf6-124">persistente</span><span class="sxs-lookup"><span data-stu-id="d2bf6-124">persistent</span></span>|<span data-ttu-id="d2bf6-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2bf6-125">Boolean</span></span>|<span data-ttu-id="d2bf6-126">Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão</span><span class="sxs-lookup"><span data-stu-id="d2bf6-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2bf6-127">Relações</span><span class="sxs-lookup"><span data-stu-id="d2bf6-127">Relationships</span></span>
<span data-ttu-id="d2bf6-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d2bf6-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2bf6-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d2bf6-129">JSON Representation</span></span>
<span data-ttu-id="d2bf6-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d2bf6-130">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnDnsRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnDnsRule",
  "name": "String",
  "servers": [
    "String"
  ],
  "proxyServerUri": "String",
  "autoTrigger": true,
  "persistent": true
}
```



