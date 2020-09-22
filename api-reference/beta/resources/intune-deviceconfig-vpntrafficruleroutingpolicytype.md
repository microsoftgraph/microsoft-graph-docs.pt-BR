---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e5782555214897ec0513ab7293adf1d877ec5f96
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48042419"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="83713-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="83713-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="83713-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83713-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83713-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="83713-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83713-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="83713-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83713-107">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="83713-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="83713-108">Membros</span><span class="sxs-lookup"><span data-stu-id="83713-108">Members</span></span>
|<span data-ttu-id="83713-109">Membro</span><span class="sxs-lookup"><span data-stu-id="83713-109">Member</span></span>|<span data-ttu-id="83713-110">Valor</span><span class="sxs-lookup"><span data-stu-id="83713-110">Value</span></span>|<span data-ttu-id="83713-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="83713-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83713-112">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="83713-112">none</span></span>|<span data-ttu-id="83713-113">,0</span><span class="sxs-lookup"><span data-stu-id="83713-113">0</span></span>|<span data-ttu-id="83713-114">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="83713-114">No routing policy specified.</span></span>|
|<span data-ttu-id="83713-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="83713-115">splitTunnel</span></span>|<span data-ttu-id="83713-116">1 </span><span class="sxs-lookup"><span data-stu-id="83713-116">1</span></span>|<span data-ttu-id="83713-117">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="83713-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="83713-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="83713-118">forceTunnel</span></span>|<span data-ttu-id="83713-119">2 </span><span class="sxs-lookup"><span data-stu-id="83713-119">2</span></span>|<span data-ttu-id="83713-120">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="83713-120">All network traffic will be routed through the VPN.</span></span>|






