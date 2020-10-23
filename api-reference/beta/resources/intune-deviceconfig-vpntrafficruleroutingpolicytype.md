---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 670fa329323d169a49bab68876cd12d35289f5ed
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724520"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="2b76c-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="2b76c-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="2b76c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b76c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b76c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b76c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b76c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b76c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b76c-107">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="2b76c-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="2b76c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2b76c-108">Members</span></span>
|<span data-ttu-id="2b76c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2b76c-109">Member</span></span>|<span data-ttu-id="2b76c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2b76c-110">Value</span></span>|<span data-ttu-id="2b76c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b76c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b76c-112">none</span><span class="sxs-lookup"><span data-stu-id="2b76c-112">none</span></span>|<span data-ttu-id="2b76c-113">,0</span><span class="sxs-lookup"><span data-stu-id="2b76c-113">0</span></span>|<span data-ttu-id="2b76c-114">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="2b76c-114">No routing policy specified.</span></span>|
|<span data-ttu-id="2b76c-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="2b76c-115">splitTunnel</span></span>|<span data-ttu-id="2b76c-116">1</span><span class="sxs-lookup"><span data-stu-id="2b76c-116">1</span></span>|<span data-ttu-id="2b76c-117">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="2b76c-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="2b76c-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="2b76c-118">forceTunnel</span></span>|<span data-ttu-id="2b76c-119">duas</span><span class="sxs-lookup"><span data-stu-id="2b76c-119">2</span></span>|<span data-ttu-id="2b76c-120">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="2b76c-120">All network traffic will be routed through the VPN.</span></span>|





