---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: db3be739e6ee1e7c5ebe2a5bd33af648488df54f
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805849"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="bf574-103">tipo de recurso vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="bf574-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="bf574-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf574-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf574-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf574-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf574-106">Definição de regra DNS de VPN.</span><span class="sxs-lookup"><span data-stu-id="bf574-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bf574-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf574-107">Properties</span></span>
|<span data-ttu-id="bf574-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf574-108">Property</span></span>|<span data-ttu-id="bf574-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf574-109">Type</span></span>|<span data-ttu-id="bf574-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf574-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf574-111">nome</span><span class="sxs-lookup"><span data-stu-id="bf574-111">name</span></span>|<span data-ttu-id="bf574-112">String</span><span class="sxs-lookup"><span data-stu-id="bf574-112">String</span></span>|<span data-ttu-id="bf574-113">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="bf574-113">Name.</span></span>|
|<span data-ttu-id="bf574-114">servidores</span><span class="sxs-lookup"><span data-stu-id="bf574-114">servers</span></span>|<span data-ttu-id="bf574-115">Coleção String</span><span class="sxs-lookup"><span data-stu-id="bf574-115">String collection</span></span>|<span data-ttu-id="bf574-116">Servidores.</span><span class="sxs-lookup"><span data-stu-id="bf574-116">Servers.</span></span>|
|<span data-ttu-id="bf574-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="bf574-117">proxyServerUri</span></span>|<span data-ttu-id="bf574-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf574-118">String</span></span>|<span data-ttu-id="bf574-119">URI do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="bf574-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="bf574-120">Gatilho autoTrigger</span><span class="sxs-lookup"><span data-stu-id="bf574-120">autoTrigger</span></span>|<span data-ttu-id="bf574-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf574-121">Boolean</span></span>|<span data-ttu-id="bf574-122">Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.</span><span class="sxs-lookup"><span data-stu-id="bf574-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="bf574-123">persistente</span><span class="sxs-lookup"><span data-stu-id="bf574-123">persistent</span></span>|<span data-ttu-id="bf574-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf574-124">Boolean</span></span>|<span data-ttu-id="bf574-125">Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão</span><span class="sxs-lookup"><span data-stu-id="bf574-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf574-126">Relações</span><span class="sxs-lookup"><span data-stu-id="bf574-126">Relationships</span></span>
<span data-ttu-id="bf574-127">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bf574-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf574-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf574-128">JSON Representation</span></span>
<span data-ttu-id="bf574-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf574-129">Here is a JSON representation of the resource.</span></span>
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





