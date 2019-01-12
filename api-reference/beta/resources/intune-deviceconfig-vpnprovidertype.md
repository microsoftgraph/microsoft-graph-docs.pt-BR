---
title: tipo de enum vpnProviderType
description: Tipo de provedor para VPN-app.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1eeb0acf2f6e7b0773cbf4697e5a27699d1f2f27
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937723"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="4c862-103">tipo de enum vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="4c862-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="4c862-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c862-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c862-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c862-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c862-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4c862-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c862-107">Tipo de provedor para VPN-app.</span><span class="sxs-lookup"><span data-stu-id="4c862-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="4c862-108">Membros</span><span class="sxs-lookup"><span data-stu-id="4c862-108">Members</span></span>
|<span data-ttu-id="4c862-109">Membro</span><span class="sxs-lookup"><span data-stu-id="4c862-109">Member</span></span>|<span data-ttu-id="4c862-110">Valor</span><span class="sxs-lookup"><span data-stu-id="4c862-110">Value</span></span>|<span data-ttu-id="4c862-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c862-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c862-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="4c862-112">notConfigured</span></span>|<span data-ttu-id="4c862-113">0</span><span class="sxs-lookup"><span data-stu-id="4c862-113">0</span></span>|<span data-ttu-id="4c862-114">Tráfego de túnel explicitamente não está configurado.</span><span class="sxs-lookup"><span data-stu-id="4c862-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="4c862-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="4c862-115">appProxy</span></span>|<span data-ttu-id="4c862-116">1</span><span class="sxs-lookup"><span data-stu-id="4c862-116">1</span></span>|<span data-ttu-id="4c862-117">Tráfego de túnel na camada de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="4c862-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="4c862-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="4c862-118">packetTunnel</span></span>|<span data-ttu-id="4c862-119">2</span><span class="sxs-lookup"><span data-stu-id="4c862-119">2</span></span>|<span data-ttu-id="4c862-120">Tráfego de túnel na camada de IP.</span><span class="sxs-lookup"><span data-stu-id="4c862-120">Tunnel traffic at the IP layer.</span></span>|





