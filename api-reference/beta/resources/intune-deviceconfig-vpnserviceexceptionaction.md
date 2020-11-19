---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 069b7dc910a7c4ce9e281235aefc52b498519351
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279434"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="305ab-103">tipo de enumeração vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="305ab-103">vpnServiceExceptionAction enum type</span></span>

<span data-ttu-id="305ab-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="305ab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="305ab-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="305ab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="305ab-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="305ab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="305ab-107">A ação VPN a ser tomada para um serviço específico.</span><span class="sxs-lookup"><span data-stu-id="305ab-107">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="305ab-108">Membros</span><span class="sxs-lookup"><span data-stu-id="305ab-108">Members</span></span>
|<span data-ttu-id="305ab-109">Membro</span><span class="sxs-lookup"><span data-stu-id="305ab-109">Member</span></span>|<span data-ttu-id="305ab-110">Valor</span><span class="sxs-lookup"><span data-stu-id="305ab-110">Value</span></span>|<span data-ttu-id="305ab-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="305ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="305ab-112">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="305ab-112">forceTrafficViaVPN</span></span>|<span data-ttu-id="305ab-113">,0</span><span class="sxs-lookup"><span data-stu-id="305ab-113">0</span></span>|<span data-ttu-id="305ab-114">Fazer com que todo o tráfego desse serviço percorra a VPN</span><span class="sxs-lookup"><span data-stu-id="305ab-114">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="305ab-115">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="305ab-115">allowTrafficOutside</span></span>|<span data-ttu-id="305ab-116">1</span><span class="sxs-lookup"><span data-stu-id="305ab-116">1</span></span>|<span data-ttu-id="305ab-117">Permitir o serviço fora da VPN</span><span class="sxs-lookup"><span data-stu-id="305ab-117">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="305ab-118">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="305ab-118">dropTraffic</span></span>|<span data-ttu-id="305ab-119">duas</span><span class="sxs-lookup"><span data-stu-id="305ab-119">2</span></span>|<span data-ttu-id="305ab-120">Remover todo o tráfego do serviço</span><span class="sxs-lookup"><span data-stu-id="305ab-120">Drop all traffic from the service</span></span>|




