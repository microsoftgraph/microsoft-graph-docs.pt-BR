---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7455e6a3f3d9887a36dd49e9c66a207da950c785
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529295"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="8f2d9-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="8f2d9-103">vpnProviderType enum type</span></span>

<span data-ttu-id="8f2d9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8f2d9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8f2d9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8f2d9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8f2d9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8f2d9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8f2d9-107">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f2d9-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="8f2d9-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8f2d9-108">Members</span></span>
|<span data-ttu-id="8f2d9-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8f2d9-109">Member</span></span>|<span data-ttu-id="8f2d9-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8f2d9-110">Value</span></span>|<span data-ttu-id="8f2d9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f2d9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f2d9-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8f2d9-112">notConfigured</span></span>|<span data-ttu-id="8f2d9-113">,0</span><span class="sxs-lookup"><span data-stu-id="8f2d9-113">0</span></span>|<span data-ttu-id="8f2d9-114">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="8f2d9-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="8f2d9-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="8f2d9-115">appProxy</span></span>|<span data-ttu-id="8f2d9-116">1 </span><span class="sxs-lookup"><span data-stu-id="8f2d9-116">1</span></span>|<span data-ttu-id="8f2d9-117">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8f2d9-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="8f2d9-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="8f2d9-118">packetTunnel</span></span>|<span data-ttu-id="8f2d9-119">2 </span><span class="sxs-lookup"><span data-stu-id="8f2d9-119">2</span></span>|<span data-ttu-id="8f2d9-120">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="8f2d9-120">Tunnel traffic at the IP layer.</span></span>|



