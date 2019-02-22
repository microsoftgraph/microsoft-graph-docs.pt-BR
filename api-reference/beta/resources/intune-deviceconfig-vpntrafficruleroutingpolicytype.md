---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7a7c6121b9adc47d116a7b3321ca150a8d42449a
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157341"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="07d2e-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="07d2e-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="07d2e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07d2e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07d2e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07d2e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07d2e-106">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="07d2e-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="07d2e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="07d2e-107">Members</span></span>
|<span data-ttu-id="07d2e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="07d2e-108">Member</span></span>|<span data-ttu-id="07d2e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="07d2e-109">Value</span></span>|<span data-ttu-id="07d2e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="07d2e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07d2e-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="07d2e-111">none</span></span>|<span data-ttu-id="07d2e-112">,0</span><span class="sxs-lookup"><span data-stu-id="07d2e-112">0</span></span>|<span data-ttu-id="07d2e-113">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="07d2e-113">No routing policy specified.</span></span>|
|<span data-ttu-id="07d2e-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="07d2e-114">splitTunnel</span></span>|<span data-ttu-id="07d2e-115">1</span><span class="sxs-lookup"><span data-stu-id="07d2e-115">1</span></span>|<span data-ttu-id="07d2e-116">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="07d2e-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="07d2e-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="07d2e-117">forceTunnel</span></span>|<span data-ttu-id="07d2e-118">duas</span><span class="sxs-lookup"><span data-stu-id="07d2e-118">2</span></span>|<span data-ttu-id="07d2e-119">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="07d2e-119">All network traffic will be routed through the VPN.</span></span>|




