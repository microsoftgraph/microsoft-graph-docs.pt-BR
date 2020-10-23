---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f20433a7e2bbb0dd134471476fd96fe3e49b9ecd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48728325"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="5d774-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="5d774-103">vpnProviderType enum type</span></span>

<span data-ttu-id="5d774-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d774-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d774-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5d774-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d774-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5d774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d774-107">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d774-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="5d774-108">Membros</span><span class="sxs-lookup"><span data-stu-id="5d774-108">Members</span></span>
|<span data-ttu-id="5d774-109">Membro</span><span class="sxs-lookup"><span data-stu-id="5d774-109">Member</span></span>|<span data-ttu-id="5d774-110">Valor</span><span class="sxs-lookup"><span data-stu-id="5d774-110">Value</span></span>|<span data-ttu-id="5d774-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5d774-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d774-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5d774-112">notConfigured</span></span>|<span data-ttu-id="5d774-113">,0</span><span class="sxs-lookup"><span data-stu-id="5d774-113">0</span></span>|<span data-ttu-id="5d774-114">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="5d774-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="5d774-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="5d774-115">appProxy</span></span>|<span data-ttu-id="5d774-116">1</span><span class="sxs-lookup"><span data-stu-id="5d774-116">1</span></span>|<span data-ttu-id="5d774-117">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5d774-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="5d774-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="5d774-118">packetTunnel</span></span>|<span data-ttu-id="5d774-119">duas</span><span class="sxs-lookup"><span data-stu-id="5d774-119">2</span></span>|<span data-ttu-id="5d774-120">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="5d774-120">Tunnel traffic at the IP layer.</span></span>|





