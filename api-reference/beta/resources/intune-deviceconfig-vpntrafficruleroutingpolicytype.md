---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5cbbba22017a40ae2f7db41e25f497c09156a2f1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969370"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="f34dc-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="f34dc-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="f34dc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f34dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f34dc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f34dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f34dc-106">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="f34dc-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="f34dc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f34dc-107">Members</span></span>
|<span data-ttu-id="f34dc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f34dc-108">Member</span></span>|<span data-ttu-id="f34dc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f34dc-109">Value</span></span>|<span data-ttu-id="f34dc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f34dc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f34dc-111">none</span><span class="sxs-lookup"><span data-stu-id="f34dc-111">none</span></span>|<span data-ttu-id="f34dc-112">,0</span><span class="sxs-lookup"><span data-stu-id="f34dc-112">0</span></span>|<span data-ttu-id="f34dc-113">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="f34dc-113">No routing policy specified.</span></span>|
|<span data-ttu-id="f34dc-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="f34dc-114">splitTunnel</span></span>|<span data-ttu-id="f34dc-115">1</span><span class="sxs-lookup"><span data-stu-id="f34dc-115">1</span></span>|<span data-ttu-id="f34dc-116">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="f34dc-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="f34dc-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="f34dc-117">forceTunnel</span></span>|<span data-ttu-id="f34dc-118">duas</span><span class="sxs-lookup"><span data-stu-id="f34dc-118">2</span></span>|<span data-ttu-id="f34dc-119">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="f34dc-119">All network traffic will be routed through the VPN.</span></span>|





