---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a7c202c404d9d1db16e328f9c7d4c220ddd481e9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525737"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="978d8-103">tipo de enumeração vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="978d8-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="978d8-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="978d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="978d8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="978d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="978d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="978d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="978d8-107">A ação VPN a ser tomada para um serviço específico.</span><span class="sxs-lookup"><span data-stu-id="978d8-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="978d8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="978d8-108">Members</span></span>
|<span data-ttu-id="978d8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="978d8-109">Member</span></span>|<span data-ttu-id="978d8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="978d8-110">Value</span></span>|<span data-ttu-id="978d8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="978d8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="978d8-112">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="978d8-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="978d8-113">,0</span><span class="sxs-lookup"><span data-stu-id="978d8-113">0</span></span>|<span data-ttu-id="978d8-114">Fazer com que todo o tráfego desse serviço percorra a VPN</span><span class="sxs-lookup"><span data-stu-id="978d8-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="978d8-115">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="978d8-115">allowTrafficOutside</span></span>|<span data-ttu-id="978d8-116">1 </span><span class="sxs-lookup"><span data-stu-id="978d8-116">1</span></span>|<span data-ttu-id="978d8-117">Permitir o serviço fora da VPN</span><span class="sxs-lookup"><span data-stu-id="978d8-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="978d8-118">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="978d8-118">dropTraffic</span></span>|<span data-ttu-id="978d8-119">2 </span><span class="sxs-lookup"><span data-stu-id="978d8-119">2</span></span>|<span data-ttu-id="978d8-120">Remover todo o tráfego do serviço</span><span class="sxs-lookup"><span data-stu-id="978d8-120">Drop all traffic from the service</span></span>|



