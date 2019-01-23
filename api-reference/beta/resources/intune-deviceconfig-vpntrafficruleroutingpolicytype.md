---
title: tipo de enum vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 028e49085e4a1fa5f01ac59ff00fbafd8846dfb9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415002"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="39fa6-103">tipo de enum vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="39fa6-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="39fa6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="39fa6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="39fa6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="39fa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39fa6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="39fa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39fa6-107">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="39fa6-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="39fa6-108">Membros</span><span class="sxs-lookup"><span data-stu-id="39fa6-108">Members</span></span>
|<span data-ttu-id="39fa6-109">Membro</span><span class="sxs-lookup"><span data-stu-id="39fa6-109">Member</span></span>|<span data-ttu-id="39fa6-110">Valor</span><span class="sxs-lookup"><span data-stu-id="39fa6-110">Value</span></span>|<span data-ttu-id="39fa6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="39fa6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39fa6-112">none</span><span class="sxs-lookup"><span data-stu-id="39fa6-112">none</span></span>|<span data-ttu-id="39fa6-113">0</span><span class="sxs-lookup"><span data-stu-id="39fa6-113">0</span></span>|<span data-ttu-id="39fa6-114">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="39fa6-114">No routing policy specified.</span></span>|
|<span data-ttu-id="39fa6-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="39fa6-115">splitTunnel</span></span>|<span data-ttu-id="39fa6-116">1</span><span class="sxs-lookup"><span data-stu-id="39fa6-116">1</span></span>|<span data-ttu-id="39fa6-117">Tráfego de rede para o aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="39fa6-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="39fa6-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="39fa6-118">forceTunnel</span></span>|<span data-ttu-id="39fa6-119">2</span><span class="sxs-lookup"><span data-stu-id="39fa6-119">2</span></span>|<span data-ttu-id="39fa6-120">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="39fa6-120">All network traffic will be routed through the VPN.</span></span>|




