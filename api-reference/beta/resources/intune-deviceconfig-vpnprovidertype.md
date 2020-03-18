---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4b064c86413d84a06884de9728ccfa9cb83d61d2
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787345"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="f5869-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="f5869-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="f5869-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f5869-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5869-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f5869-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5869-106">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5869-106">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="f5869-107">Membros</span><span class="sxs-lookup"><span data-stu-id="f5869-107">Members</span></span>
|<span data-ttu-id="f5869-108">Membro</span><span class="sxs-lookup"><span data-stu-id="f5869-108">Member</span></span>|<span data-ttu-id="f5869-109">Valor</span><span class="sxs-lookup"><span data-stu-id="f5869-109">Value</span></span>|<span data-ttu-id="f5869-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f5869-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5869-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f5869-111">notConfigured</span></span>|<span data-ttu-id="f5869-112">,0</span><span class="sxs-lookup"><span data-stu-id="f5869-112">0</span></span>|<span data-ttu-id="f5869-113">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="f5869-113">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="f5869-114">appProxy</span><span class="sxs-lookup"><span data-stu-id="f5869-114">appProxy</span></span>|<span data-ttu-id="f5869-115">1</span><span class="sxs-lookup"><span data-stu-id="f5869-115">1</span></span>|<span data-ttu-id="f5869-116">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f5869-116">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="f5869-117">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="f5869-117">packetTunnel</span></span>|<span data-ttu-id="f5869-118">duas</span><span class="sxs-lookup"><span data-stu-id="f5869-118">2</span></span>|<span data-ttu-id="f5869-119">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="f5869-119">Tunnel traffic at the IP layer.</span></span>|



