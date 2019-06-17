---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f2188efc73201aabf98267a77fee96b9c60de9d
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996334"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="52f87-103">tipo de recurso vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="52f87-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="52f87-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="52f87-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="52f87-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="52f87-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="52f87-106">Definição de regra DNS de VPN.</span><span class="sxs-lookup"><span data-stu-id="52f87-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="52f87-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52f87-107">Properties</span></span>
|<span data-ttu-id="52f87-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52f87-108">Property</span></span>|<span data-ttu-id="52f87-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="52f87-109">Type</span></span>|<span data-ttu-id="52f87-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="52f87-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52f87-111">name</span><span class="sxs-lookup"><span data-stu-id="52f87-111">name</span></span>|<span data-ttu-id="52f87-112">String</span><span class="sxs-lookup"><span data-stu-id="52f87-112">String</span></span>|<span data-ttu-id="52f87-113">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="52f87-113">Name.</span></span>|
|<span data-ttu-id="52f87-114">servidores</span><span class="sxs-lookup"><span data-stu-id="52f87-114">servers</span></span>|<span data-ttu-id="52f87-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="52f87-115">String collection</span></span>|<span data-ttu-id="52f87-116">Servidores.</span><span class="sxs-lookup"><span data-stu-id="52f87-116">Servers.</span></span>|
|<span data-ttu-id="52f87-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="52f87-117">proxyServerUri</span></span>|<span data-ttu-id="52f87-118">String</span><span class="sxs-lookup"><span data-stu-id="52f87-118">String</span></span>|<span data-ttu-id="52f87-119">URI do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="52f87-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="52f87-120">Gatilho autotrigger</span><span class="sxs-lookup"><span data-stu-id="52f87-120">autoTrigger</span></span>|<span data-ttu-id="52f87-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="52f87-121">Boolean</span></span>|<span data-ttu-id="52f87-122">Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.</span><span class="sxs-lookup"><span data-stu-id="52f87-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="52f87-123">persistente</span><span class="sxs-lookup"><span data-stu-id="52f87-123">persistent</span></span>|<span data-ttu-id="52f87-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="52f87-124">Boolean</span></span>|<span data-ttu-id="52f87-125">Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão</span><span class="sxs-lookup"><span data-stu-id="52f87-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="52f87-126">Relações</span><span class="sxs-lookup"><span data-stu-id="52f87-126">Relationships</span></span>
<span data-ttu-id="52f87-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52f87-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="52f87-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52f87-128">JSON Representation</span></span>
<span data-ttu-id="52f87-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52f87-129">Here is a JSON representation of the resource.</span></span>
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





