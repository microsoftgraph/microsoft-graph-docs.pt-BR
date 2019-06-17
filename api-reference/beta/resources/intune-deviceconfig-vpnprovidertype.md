---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 23d8382c535a459beaf22d8cf229d0f6b3a50237
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987548"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="950c1-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="950c1-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="950c1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="950c1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="950c1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="950c1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950c1-106">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="950c1-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="950c1-107">Membros</span><span class="sxs-lookup"><span data-stu-id="950c1-107">Members</span></span>
|<span data-ttu-id="950c1-108">Membro</span><span class="sxs-lookup"><span data-stu-id="950c1-108">Member</span></span>|<span data-ttu-id="950c1-109">Valor</span><span class="sxs-lookup"><span data-stu-id="950c1-109">Value</span></span>|<span data-ttu-id="950c1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="950c1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950c1-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="950c1-111">notConfigured</span></span>|<span data-ttu-id="950c1-112">,0</span><span class="sxs-lookup"><span data-stu-id="950c1-112">0</span></span>|<span data-ttu-id="950c1-113">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="950c1-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="950c1-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="950c1-114">appProxy</span></span>|<span data-ttu-id="950c1-115">1</span><span class="sxs-lookup"><span data-stu-id="950c1-115">1</span></span>|<span data-ttu-id="950c1-116">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="950c1-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="950c1-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="950c1-117">packetTunnel</span></span>|<span data-ttu-id="950c1-118">duas</span><span class="sxs-lookup"><span data-stu-id="950c1-118">2</span></span>|<span data-ttu-id="950c1-119">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="950c1-119">Tunnel traffic at the IP layer.</span></span>|





