---
title: tipo de enumeração vpnProviderType
description: Tipo de provedor para VPN por aplicativo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fb29fc6a77eb6db051279cdeb630dbf4104aa9af
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279574"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="c49de-103">tipo de enumeração vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="c49de-103">vpnProviderType enum type</span></span>

<span data-ttu-id="c49de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c49de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c49de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c49de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c49de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c49de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c49de-107">Tipo de provedor para VPN por aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c49de-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="c49de-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c49de-108">Members</span></span>
|<span data-ttu-id="c49de-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c49de-109">Member</span></span>|<span data-ttu-id="c49de-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c49de-110">Value</span></span>|<span data-ttu-id="c49de-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c49de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c49de-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c49de-112">notConfigured</span></span>|<span data-ttu-id="c49de-113">,0</span><span class="sxs-lookup"><span data-stu-id="c49de-113">0</span></span>|<span data-ttu-id="c49de-114">O tráfego de encapsulamento não é configurado explicitamente.</span><span class="sxs-lookup"><span data-stu-id="c49de-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="c49de-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="c49de-115">appProxy</span></span>|<span data-ttu-id="c49de-116">1</span><span class="sxs-lookup"><span data-stu-id="c49de-116">1</span></span>|<span data-ttu-id="c49de-117">Tráfego de túnel na camada do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="c49de-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="c49de-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="c49de-118">packetTunnel</span></span>|<span data-ttu-id="c49de-119">duas</span><span class="sxs-lookup"><span data-stu-id="c49de-119">2</span></span>|<span data-ttu-id="c49de-120">Tráfego de túnel na camada IP.</span><span class="sxs-lookup"><span data-stu-id="c49de-120">Tunnel traffic at the IP layer.</span></span>|




