---
title: tipo de enumeração vpnTrafficRuleRoutingPolicyType
description: Especifica a política de roteamento para uma regra de tráfego VPN.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: cbedfb515da4cb2ec68e928363ec69bfc96837e3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215629"
---
# <a name="vpntrafficruleroutingpolicytype-enum-type"></a><span data-ttu-id="93ace-103">tipo de enumeração vpnTrafficRuleRoutingPolicyType</span><span class="sxs-lookup"><span data-stu-id="93ace-103">vpnTrafficRuleRoutingPolicyType enum type</span></span>

<span data-ttu-id="93ace-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93ace-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="93ace-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="93ace-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93ace-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="93ace-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93ace-107">Especifica a política de roteamento para uma regra de tráfego VPN.</span><span class="sxs-lookup"><span data-stu-id="93ace-107">Specifies the routing policy for a VPN traffic rule.</span></span>

## <a name="members"></a><span data-ttu-id="93ace-108">Membros</span><span class="sxs-lookup"><span data-stu-id="93ace-108">Members</span></span>
|<span data-ttu-id="93ace-109">Membro</span><span class="sxs-lookup"><span data-stu-id="93ace-109">Member</span></span>|<span data-ttu-id="93ace-110">Valor</span><span class="sxs-lookup"><span data-stu-id="93ace-110">Value</span></span>|<span data-ttu-id="93ace-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="93ace-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93ace-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="93ace-112">none</span></span>|<span data-ttu-id="93ace-113">,0</span><span class="sxs-lookup"><span data-stu-id="93ace-113">0</span></span>|<span data-ttu-id="93ace-114">Nenhuma política de roteamento especificada.</span><span class="sxs-lookup"><span data-stu-id="93ace-114">No routing policy specified.</span></span>|
|<span data-ttu-id="93ace-115">splitTunnel</span><span class="sxs-lookup"><span data-stu-id="93ace-115">splitTunnel</span></span>|<span data-ttu-id="93ace-116">1</span><span class="sxs-lookup"><span data-stu-id="93ace-116">1</span></span>|<span data-ttu-id="93ace-117">O tráfego de rede do aplicativo especificado será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="93ace-117">Network traffic for the specified app will be routed through the VPN.</span></span>|
|<span data-ttu-id="93ace-118">forceTunnel</span><span class="sxs-lookup"><span data-stu-id="93ace-118">forceTunnel</span></span>|<span data-ttu-id="93ace-119">duas</span><span class="sxs-lookup"><span data-stu-id="93ace-119">2</span></span>|<span data-ttu-id="93ace-120">Todo o tráfego de rede será roteado através da VPN.</span><span class="sxs-lookup"><span data-stu-id="93ace-120">All network traffic will be routed through the VPN.</span></span>|




