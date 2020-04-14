---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 2809f0297ba952d1c302bc0597ab3e00bb33ab95
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412035"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="62b57-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="62b57-103">vpnProviderType enum type</span></span>

<span data-ttu-id="62b57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62b57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62b57-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62b57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62b57-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62b57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62b57-107">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62b57-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="62b57-108">Membros</span><span class="sxs-lookup"><span data-stu-id="62b57-108">Members</span></span>
|<span data-ttu-id="62b57-109">Membro</span><span class="sxs-lookup"><span data-stu-id="62b57-109">Member</span></span>|<span data-ttu-id="62b57-110">Valor</span><span class="sxs-lookup"><span data-stu-id="62b57-110">Value</span></span>|<span data-ttu-id="62b57-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62b57-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62b57-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="62b57-112">notConfigured</span></span>|<span data-ttu-id="62b57-113">,0</span><span class="sxs-lookup"><span data-stu-id="62b57-113">0</span></span>|<span data-ttu-id="62b57-114">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="62b57-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="62b57-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="62b57-115">appProxy</span></span>|<span data-ttu-id="62b57-116">1</span><span class="sxs-lookup"><span data-stu-id="62b57-116">1</span></span>|<span data-ttu-id="62b57-117">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="62b57-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="62b57-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="62b57-118">packetTunnel</span></span>|<span data-ttu-id="62b57-119">duas</span><span class="sxs-lookup"><span data-stu-id="62b57-119">2</span></span>|<span data-ttu-id="62b57-120">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="62b57-120">Tunnel traffic at the IP layer.</span></span>|



