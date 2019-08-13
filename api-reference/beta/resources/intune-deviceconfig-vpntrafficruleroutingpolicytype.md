---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 529c42722d8ce3827bb9daa4c0f158cfd92d8383
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367516"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="0748f-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="0748f-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

> <span data-ttu-id="0748f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0748f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0748f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0748f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0748f-106">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="0748f-106">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="0748f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="0748f-107">Members</span></span>
|<span data-ttu-id="0748f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="0748f-108">Member</span></span>|<span data-ttu-id="0748f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="0748f-109">Value</span></span>|<span data-ttu-id="0748f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0748f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0748f-111">none</span><span class="sxs-lookup"><span data-stu-id="0748f-111">none</span></span>|<span data-ttu-id="0748f-112">,0</span><span class="sxs-lookup"><span data-stu-id="0748f-112">0</span></span>|<span data-ttu-id="0748f-113">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="0748f-113">No routing policy specified.</span></span>|
|<span data-ttu-id="0748f-114">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="0748f-114">splitTunnel</span></span>|<span data-ttu-id="0748f-115">1</span><span class="sxs-lookup"><span data-stu-id="0748f-115">1</span></span>|<span data-ttu-id="0748f-116">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="0748f-116">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="0748f-117">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="0748f-117">forceTunnel</span></span>|<span data-ttu-id="0748f-118">duas</span><span class="sxs-lookup"><span data-stu-id="0748f-118">2</span></span>|<span data-ttu-id="0748f-119">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="0748f-119">All network traffic will be routed through the VPN.</span></span>|



