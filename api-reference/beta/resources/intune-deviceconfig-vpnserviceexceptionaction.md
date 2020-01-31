---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1310d91da9a7ea8e3a6274acd48e8ebc1359cafd
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636711"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="c6e4c-103">tipo de enumeração vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="c6e4c-103">vpnServiceExceptionAction enum type</span></span>

> <span data-ttu-id="c6e4c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c6e4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6e4c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c6e4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6e4c-106">A ação VPN a ser tomada para um serviço específico.</span><span class="sxs-lookup"><span data-stu-id="c6e4c-106">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="c6e4c-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c6e4c-107">Members</span></span>
|<span data-ttu-id="c6e4c-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c6e4c-108">Member</span></span>|<span data-ttu-id="c6e4c-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c6e4c-109">Value</span></span>|<span data-ttu-id="c6e4c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c6e4c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6e4c-111">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="c6e4c-111">forceTrafficViaVPN</span></span>|<span data-ttu-id="c6e4c-112">,0</span><span class="sxs-lookup"><span data-stu-id="c6e4c-112">0</span></span>|<span data-ttu-id="c6e4c-113">Fazer com que todo o tráfego desse serviço percorra a VPN</span><span class="sxs-lookup"><span data-stu-id="c6e4c-113">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="c6e4c-114">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="c6e4c-114">allowTrafficOutside</span></span>|<span data-ttu-id="c6e4c-115">1 </span><span class="sxs-lookup"><span data-stu-id="c6e4c-115">1</span></span>|<span data-ttu-id="c6e4c-116">Permitir o serviço fora da VPN</span><span class="sxs-lookup"><span data-stu-id="c6e4c-116">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="c6e4c-117">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="c6e4c-117">dropTraffic</span></span>|<span data-ttu-id="c6e4c-118">2 </span><span class="sxs-lookup"><span data-stu-id="c6e4c-118">2</span></span>|<span data-ttu-id="c6e4c-119">Remover todo o tráfego do serviço</span><span class="sxs-lookup"><span data-stu-id="c6e4c-119">Drop all traffic from the service</span></span>|



