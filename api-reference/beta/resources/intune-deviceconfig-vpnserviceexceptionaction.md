---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba0ea4081ea958d4eb36d2506c4cc4cab5ef59a7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985920"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="f0626-103">tipo de enumeração vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="f0626-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="f0626-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0626-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0626-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0626-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0626-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0626-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0626-107">A ação VPN a ser tomada para um serviço específico.</span><span class="sxs-lookup"><span data-stu-id="f0626-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="f0626-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f0626-108">Members</span></span>
|<span data-ttu-id="f0626-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f0626-109">Member</span></span>|<span data-ttu-id="f0626-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f0626-110">Value</span></span>|<span data-ttu-id="f0626-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0626-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0626-112">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="f0626-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="f0626-113">,0</span><span class="sxs-lookup"><span data-stu-id="f0626-113">0</span></span>|<span data-ttu-id="f0626-114">Fazer com que todo o tráfego desse serviço percorra a VPN</span><span class="sxs-lookup"><span data-stu-id="f0626-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="f0626-115">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="f0626-115">allowTrafficOutside</span></span>|<span data-ttu-id="f0626-116">1 </span><span class="sxs-lookup"><span data-stu-id="f0626-116">1</span></span>|<span data-ttu-id="f0626-117">Permitir o serviço fora da VPN</span><span class="sxs-lookup"><span data-stu-id="f0626-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="f0626-118">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="f0626-118">dropTraffic</span></span>|<span data-ttu-id="f0626-119">2 </span><span class="sxs-lookup"><span data-stu-id="f0626-119">2</span></span>|<span data-ttu-id="f0626-120">Remover todo o tráfego do serviço</span><span class="sxs-lookup"><span data-stu-id="f0626-120">Drop all traffic from the service</span></span>|






