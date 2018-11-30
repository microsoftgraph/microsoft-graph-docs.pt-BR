---
title: tipo de enum vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
ms.openlocfilehash: df51851ef0820f5982a6689421503364e9064c78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27035902"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="b479f-103">tipo de enum vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="b479f-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="b479f-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b479f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b479f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b479f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b479f-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b479f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b479f-107">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="b479f-107">Specifies the routing policy for a VPN traffic rule.</span></span>
## <a name="members"></a><span data-ttu-id="b479f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="b479f-108">Members</span></span>
|<span data-ttu-id="b479f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="b479f-109">Member</span></span>|<span data-ttu-id="b479f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="b479f-110">Value</span></span>|<span data-ttu-id="b479f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b479f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b479f-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="b479f-112">none</span></span>|<span data-ttu-id="b479f-113">0</span><span class="sxs-lookup"><span data-stu-id="b479f-113">0</span></span>|<span data-ttu-id="b479f-114">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="b479f-114">No routing policy specified.</span></span>|
|<span data-ttu-id="b479f-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="b479f-115">splitTunnel</span></span>|<span data-ttu-id="b479f-116">1</span><span class="sxs-lookup"><span data-stu-id="b479f-116">1</span></span>|<span data-ttu-id="b479f-117">Tráfego de rede para o aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="b479f-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="b479f-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="b479f-118">forceTunnel</span></span>|<span data-ttu-id="b479f-119">2</span><span class="sxs-lookup"><span data-stu-id="b479f-119">2</span></span>|<span data-ttu-id="b479f-120">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="b479f-120">All network traffic will be routed through the VPN.</span></span>|





