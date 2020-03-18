---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ffc8c01aadfe77bd3d92d9f7618a5846cf7c855
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787387"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="23754-103">tipo de recurso vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="23754-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="23754-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="23754-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23754-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="23754-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23754-106">Definição de regra DNS de VPN.</span><span class="sxs-lookup"><span data-stu-id="23754-106">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="23754-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23754-107">Properties</span></span>
|<span data-ttu-id="23754-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23754-108">Property</span></span>|<span data-ttu-id="23754-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="23754-109">Type</span></span>|<span data-ttu-id="23754-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="23754-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23754-111">nome</span><span class="sxs-lookup"><span data-stu-id="23754-111">name</span></span>|<span data-ttu-id="23754-112">String</span><span class="sxs-lookup"><span data-stu-id="23754-112">String</span></span>|<span data-ttu-id="23754-113">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="23754-113">Name.</span></span>|
|<span data-ttu-id="23754-114">servidores</span><span class="sxs-lookup"><span data-stu-id="23754-114">servers</span></span>|<span data-ttu-id="23754-115">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="23754-115">String collection</span></span>|<span data-ttu-id="23754-116">Servidores.</span><span class="sxs-lookup"><span data-stu-id="23754-116">Servers.</span></span>|
|<span data-ttu-id="23754-117">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="23754-117">proxyServerUri</span></span>|<span data-ttu-id="23754-118">String</span><span class="sxs-lookup"><span data-stu-id="23754-118">String</span></span>|<span data-ttu-id="23754-119">URI do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="23754-119">Proxy Server Uri.</span></span>|
|<span data-ttu-id="23754-120">Gatilho autotrigger</span><span class="sxs-lookup"><span data-stu-id="23754-120">autoTrigger</span></span>|<span data-ttu-id="23754-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="23754-121">Boolean</span></span>|<span data-ttu-id="23754-122">Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.</span><span class="sxs-lookup"><span data-stu-id="23754-122">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="23754-123">persistente</span><span class="sxs-lookup"><span data-stu-id="23754-123">persistent</span></span>|<span data-ttu-id="23754-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="23754-124">Boolean</span></span>|<span data-ttu-id="23754-125">Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão</span><span class="sxs-lookup"><span data-stu-id="23754-125">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="23754-126">Relações</span><span class="sxs-lookup"><span data-stu-id="23754-126">Relationships</span></span>
<span data-ttu-id="23754-127">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23754-127">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23754-128">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23754-128">JSON Representation</span></span>
<span data-ttu-id="23754-129">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23754-129">Here is a JSON representation of the resource.</span></span>
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



