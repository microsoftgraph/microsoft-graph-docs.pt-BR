---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 577408b34b7483ebc313f761dfaf47e0e09cdd90
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787282"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="ce6bc-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="ce6bc-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="ce6bc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce6bc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce6bc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce6bc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce6bc-106">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="ce6bc-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="ce6bc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="ce6bc-107">Members</span></span>
|<span data-ttu-id="ce6bc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="ce6bc-108">Member</span></span>|<span data-ttu-id="ce6bc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="ce6bc-109">Value</span></span>|<span data-ttu-id="ce6bc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce6bc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce6bc-111">none</span><span class="sxs-lookup"><span data-stu-id="ce6bc-111">none</span></span>|<span data-ttu-id="ce6bc-112">,0</span><span class="sxs-lookup"><span data-stu-id="ce6bc-112">0</span></span>|<span data-ttu-id="ce6bc-113">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="ce6bc-113">No routing policy specified.</span></span>|
|<span data-ttu-id="ce6bc-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="ce6bc-114">splitTunnel</span></span>|<span data-ttu-id="ce6bc-115">1</span><span class="sxs-lookup"><span data-stu-id="ce6bc-115">1</span></span>|<span data-ttu-id="ce6bc-116">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="ce6bc-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="ce6bc-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="ce6bc-117">forceTunnel</span></span>|<span data-ttu-id="ce6bc-118">duas</span><span class="sxs-lookup"><span data-stu-id="ce6bc-118">2</span></span>|<span data-ttu-id="ce6bc-119">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="ce6bc-119">All network traffic will be routed through the VPN.</span></span>|



