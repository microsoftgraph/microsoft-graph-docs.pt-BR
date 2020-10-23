---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 00edcb55e71f4bd789687769033588cdb9f7fe00
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728374"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="f37f7-103">tipo de recurso vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="f37f7-103">vpnDnsRule resource type</span></span>

<span data-ttu-id="f37f7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f37f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f37f7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f37f7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f37f7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f37f7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f37f7-107">Definição de regra DNS de VPN.</span><span class="sxs-lookup"><span data-stu-id="f37f7-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f37f7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f37f7-108">Properties</span></span>
|<span data-ttu-id="f37f7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f37f7-109">Property</span></span>|<span data-ttu-id="f37f7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="f37f7-110">Type</span></span>|<span data-ttu-id="f37f7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f37f7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f37f7-112">nome</span><span class="sxs-lookup"><span data-stu-id="f37f7-112">name</span></span>|<span data-ttu-id="f37f7-113">String</span><span class="sxs-lookup"><span data-stu-id="f37f7-113">String</span></span>|<span data-ttu-id="f37f7-114">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="f37f7-114">Name.</span></span>|
|<span data-ttu-id="f37f7-115">servidores</span><span class="sxs-lookup"><span data-stu-id="f37f7-115">servers</span></span>|<span data-ttu-id="f37f7-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="f37f7-116">String collection</span></span>|<span data-ttu-id="f37f7-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="f37f7-117">Servers.</span></span>|
|<span data-ttu-id="f37f7-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="f37f7-118">proxyServerUri</span></span>|<span data-ttu-id="f37f7-119">String</span><span class="sxs-lookup"><span data-stu-id="f37f7-119">String</span></span>|<span data-ttu-id="f37f7-120">URI do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="f37f7-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="f37f7-121">Gatilho autotrigger</span><span class="sxs-lookup"><span data-stu-id="f37f7-121">autoTrigger</span></span>|<span data-ttu-id="f37f7-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="f37f7-122">Boolean</span></span>|<span data-ttu-id="f37f7-123">Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.</span><span class="sxs-lookup"><span data-stu-id="f37f7-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="f37f7-124">persistente</span><span class="sxs-lookup"><span data-stu-id="f37f7-124">persistent</span></span>|<span data-ttu-id="f37f7-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="f37f7-125">Boolean</span></span>|<span data-ttu-id="f37f7-126">Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão</span><span class="sxs-lookup"><span data-stu-id="f37f7-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="f37f7-127">Relações</span><span class="sxs-lookup"><span data-stu-id="f37f7-127">Relationships</span></span>
<span data-ttu-id="f37f7-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f37f7-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f37f7-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f37f7-129">JSON Representation</span></span>
<span data-ttu-id="f37f7-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f37f7-130">Here is a JSON representation of the resource.</span></span>
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





