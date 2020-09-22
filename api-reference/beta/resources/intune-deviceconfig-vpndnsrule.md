---
title: tipo de recurso vpnDnsRule
description: Definição de regra DNS de VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8d3f9349d7b966a608aaa1b0bef04b00df6a475f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049104"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="bf80c-103">tipo de recurso vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="bf80c-103">vpnDnsRule resource type</span></span>

<span data-ttu-id="bf80c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf80c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bf80c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bf80c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bf80c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bf80c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bf80c-107">Definição de regra DNS de VPN.</span><span class="sxs-lookup"><span data-stu-id="bf80c-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="bf80c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bf80c-108">Properties</span></span>
|<span data-ttu-id="bf80c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bf80c-109">Property</span></span>|<span data-ttu-id="bf80c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bf80c-110">Type</span></span>|<span data-ttu-id="bf80c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bf80c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bf80c-112">nome</span><span class="sxs-lookup"><span data-stu-id="bf80c-112">name</span></span>|<span data-ttu-id="bf80c-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf80c-113">String</span></span>|<span data-ttu-id="bf80c-114">Tdomínio.</span><span class="sxs-lookup"><span data-stu-id="bf80c-114">Name.</span></span>|
|<span data-ttu-id="bf80c-115">servidores</span><span class="sxs-lookup"><span data-stu-id="bf80c-115">servers</span></span>|<span data-ttu-id="bf80c-116">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf80c-116">String collection</span></span>|<span data-ttu-id="bf80c-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="bf80c-117">Servers.</span></span>|
|<span data-ttu-id="bf80c-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="bf80c-118">proxyServerUri</span></span>|<span data-ttu-id="bf80c-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bf80c-119">String</span></span>|<span data-ttu-id="bf80c-120">URI do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="bf80c-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="bf80c-121">Gatilho autotrigger</span><span class="sxs-lookup"><span data-stu-id="bf80c-121">autoTrigger</span></span>|<span data-ttu-id="bf80c-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf80c-122">Boolean</span></span>|<span data-ttu-id="bf80c-123">Conectar-se automaticamente à VPN quando o dispositivo se conectar a este domínio: padrão false.</span><span class="sxs-lookup"><span data-stu-id="bf80c-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="bf80c-124">persistente</span><span class="sxs-lookup"><span data-stu-id="bf80c-124">persistent</span></span>|<span data-ttu-id="bf80c-125">Booliano</span><span class="sxs-lookup"><span data-stu-id="bf80c-125">Boolean</span></span>|<span data-ttu-id="bf80c-126">Manter esta regra ativa mesmo quando a VPN não estiver conectada: false padrão</span><span class="sxs-lookup"><span data-stu-id="bf80c-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="bf80c-127">Relações</span><span class="sxs-lookup"><span data-stu-id="bf80c-127">Relationships</span></span>
<span data-ttu-id="bf80c-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bf80c-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bf80c-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bf80c-129">JSON Representation</span></span>
<span data-ttu-id="bf80c-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bf80c-130">Here is a JSON representation of the resource.</span></span>
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






