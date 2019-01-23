---
title: tipo de recurso de vpnDnsRule
description: Definição de regra de DNS da VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ae6141cc0579840a23a28be2dce951c160f90248
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425579"
---
# <a name="vpndnsrule-resource-type"></a><span data-ttu-id="97f13-103">tipo de recurso de vpnDnsRule</span><span class="sxs-lookup"><span data-stu-id="97f13-103">vpnDnsRule resource type</span></span>

> <span data-ttu-id="97f13-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="97f13-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="97f13-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="97f13-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97f13-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="97f13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97f13-107">Definição de regra de DNS da VPN.</span><span class="sxs-lookup"><span data-stu-id="97f13-107">VPN DNS Rule definition.</span></span>

## <a name="properties"></a><span data-ttu-id="97f13-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="97f13-108">Properties</span></span>
|<span data-ttu-id="97f13-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="97f13-109">Property</span></span>|<span data-ttu-id="97f13-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="97f13-110">Type</span></span>|<span data-ttu-id="97f13-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="97f13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97f13-112">name</span><span class="sxs-lookup"><span data-stu-id="97f13-112">name</span></span>|<span data-ttu-id="97f13-113">String</span><span class="sxs-lookup"><span data-stu-id="97f13-113">String</span></span>|<span data-ttu-id="97f13-114">Nome.</span><span class="sxs-lookup"><span data-stu-id="97f13-114">Name.</span></span>|
|<span data-ttu-id="97f13-115">servidores</span><span class="sxs-lookup"><span data-stu-id="97f13-115">servers</span></span>|<span data-ttu-id="97f13-116">String collection</span><span class="sxs-lookup"><span data-stu-id="97f13-116">String collection</span></span>|<span data-ttu-id="97f13-117">Servidores.</span><span class="sxs-lookup"><span data-stu-id="97f13-117">Servers.</span></span>|
|<span data-ttu-id="97f13-118">proxyServerUri</span><span class="sxs-lookup"><span data-stu-id="97f13-118">proxyServerUri</span></span>|<span data-ttu-id="97f13-119">String</span><span class="sxs-lookup"><span data-stu-id="97f13-119">String</span></span>|<span data-ttu-id="97f13-120">Uri do servidor proxy.</span><span class="sxs-lookup"><span data-stu-id="97f13-120">Proxy Server Uri.</span></span>|
|<span data-ttu-id="97f13-121">autoTrigger</span><span class="sxs-lookup"><span data-stu-id="97f13-121">autoTrigger</span></span>|<span data-ttu-id="97f13-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f13-122">Boolean</span></span>|<span data-ttu-id="97f13-123">Conectar-se automaticamente à VPN quando o dispositivo se conecta a esse domínio: padrão False.</span><span class="sxs-lookup"><span data-stu-id="97f13-123">Automatically connect to the VPN when the device connects to this domain: Default False.</span></span>|
|<span data-ttu-id="97f13-124">persistente</span><span class="sxs-lookup"><span data-stu-id="97f13-124">persistent</span></span>|<span data-ttu-id="97f13-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="97f13-125">Boolean</span></span>|<span data-ttu-id="97f13-126">Mantenha esta regra ativos, mesmo quando não estiver conectada a VPN: padrão False</span><span class="sxs-lookup"><span data-stu-id="97f13-126">Keep this rule active even when the VPN is not connected: Default False</span></span>|

## <a name="relationships"></a><span data-ttu-id="97f13-127">Relações</span><span class="sxs-lookup"><span data-stu-id="97f13-127">Relationships</span></span>
<span data-ttu-id="97f13-128">Nenhum</span><span class="sxs-lookup"><span data-stu-id="97f13-128">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="97f13-129">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="97f13-129">JSON Representation</span></span>
<span data-ttu-id="97f13-130">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="97f13-130">Here is a JSON representation of the resource.</span></span>
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




