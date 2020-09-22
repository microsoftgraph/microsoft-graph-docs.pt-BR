---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 43b962235cda6622ca0d7d10d7da57f9f5181471
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48048992"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="8b390-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="8b390-103">vpnProviderType enum type</span></span>

<span data-ttu-id="8b390-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8b390-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8b390-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b390-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b390-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b390-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b390-107">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b390-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="8b390-108">Membros</span><span class="sxs-lookup"><span data-stu-id="8b390-108">Members</span></span>
|<span data-ttu-id="8b390-109">Membro</span><span class="sxs-lookup"><span data-stu-id="8b390-109">Member</span></span>|<span data-ttu-id="8b390-110">Valor</span><span class="sxs-lookup"><span data-stu-id="8b390-110">Value</span></span>|<span data-ttu-id="8b390-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b390-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b390-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8b390-112">notConfigured</span></span>|<span data-ttu-id="8b390-113">,0</span><span class="sxs-lookup"><span data-stu-id="8b390-113">0</span></span>|<span data-ttu-id="8b390-114">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="8b390-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="8b390-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="8b390-115">appProxy</span></span>|<span data-ttu-id="8b390-116">1 </span><span class="sxs-lookup"><span data-stu-id="8b390-116">1</span></span>|<span data-ttu-id="8b390-117">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="8b390-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="8b390-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="8b390-118">packetTunnel</span></span>|<span data-ttu-id="8b390-119">2 </span><span class="sxs-lookup"><span data-stu-id="8b390-119">2</span></span>|<span data-ttu-id="8b390-120">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="8b390-120">Tunnel traffic at the IP layer.</span></span>|






