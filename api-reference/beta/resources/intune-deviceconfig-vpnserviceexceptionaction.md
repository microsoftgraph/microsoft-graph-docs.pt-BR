---
title: tipo de enumeração vpnServiceExceptionAction
description: A ação VPN a ser tomada para um serviço específico.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b0c952a14db65e836c2a3391cb44a871957e708
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787303"
---
# <a name="vpnserviceexceptionaction-enum-type"></a><span data-ttu-id="1ffbc-103">tipo de enumeração vpnServiceExceptionAction</span><span class="sxs-lookup"><span data-stu-id="1ffbc-103">vpnServiceExceptionAction enum type</span></span>

> <span data-ttu-id="1ffbc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ffbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ffbc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ffbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ffbc-106">A ação VPN a ser tomada para um serviço específico.</span><span class="sxs-lookup"><span data-stu-id="1ffbc-106">The VPN action to take for a specific service.</span></span>

## <a name="members"></a><span data-ttu-id="1ffbc-107">Membros</span><span class="sxs-lookup"><span data-stu-id="1ffbc-107">Members</span></span>
|<span data-ttu-id="1ffbc-108">Membro</span><span class="sxs-lookup"><span data-stu-id="1ffbc-108">Member</span></span>|<span data-ttu-id="1ffbc-109">Valor</span><span class="sxs-lookup"><span data-stu-id="1ffbc-109">Value</span></span>|<span data-ttu-id="1ffbc-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ffbc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ffbc-111">forceTrafficViaVPN</span><span class="sxs-lookup"><span data-stu-id="1ffbc-111">forceTrafficViaVPN</span></span>|<span data-ttu-id="1ffbc-112">,0</span><span class="sxs-lookup"><span data-stu-id="1ffbc-112">0</span></span>|<span data-ttu-id="1ffbc-113">Fazer com que todo o tráfego desse serviço percorra a VPN</span><span class="sxs-lookup"><span data-stu-id="1ffbc-113">Make all traffic from that service go through the VPN</span></span>|
|<span data-ttu-id="1ffbc-114">allowTrafficOutside</span><span class="sxs-lookup"><span data-stu-id="1ffbc-114">allowTrafficOutside</span></span>|<span data-ttu-id="1ffbc-115">1</span><span class="sxs-lookup"><span data-stu-id="1ffbc-115">1</span></span>|<span data-ttu-id="1ffbc-116">Permitir o serviço fora da VPN</span><span class="sxs-lookup"><span data-stu-id="1ffbc-116">Allow the service outside of the VPN</span></span>|
|<span data-ttu-id="1ffbc-117">dropTraffic</span><span class="sxs-lookup"><span data-stu-id="1ffbc-117">dropTraffic</span></span>|<span data-ttu-id="1ffbc-118">duas</span><span class="sxs-lookup"><span data-stu-id="1ffbc-118">2</span></span>|<span data-ttu-id="1ffbc-119">Remover todo o tráfego do serviço</span><span class="sxs-lookup"><span data-stu-id="1ffbc-119">Drop all traffic from the service</span></span>|



