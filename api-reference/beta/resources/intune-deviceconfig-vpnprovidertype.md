---
title: tipo de enum vpnProviderType
description: Tipo de provedor para VPN-app.
author: tfitzmac
ms.openlocfilehash: d8f002582879302bcbe0fb965110eaa5e674a689
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27351594"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="0da53-103">tipo de enum vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="0da53-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="0da53-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0da53-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0da53-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0da53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0da53-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0da53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0da53-107">Tipo de provedor para VPN-app.</span><span class="sxs-lookup"><span data-stu-id="0da53-107">Provider type for per-app VPN.</span></span>
## <a name="members"></a><span data-ttu-id="0da53-108">Membros</span><span class="sxs-lookup"><span data-stu-id="0da53-108">Members</span></span>
|<span data-ttu-id="0da53-109">Membro</span><span class="sxs-lookup"><span data-stu-id="0da53-109">Member</span></span>|<span data-ttu-id="0da53-110">Valor</span><span class="sxs-lookup"><span data-stu-id="0da53-110">Value</span></span>|<span data-ttu-id="0da53-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0da53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0da53-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="0da53-112">notConfigured</span></span>|<span data-ttu-id="0da53-113">0</span><span class="sxs-lookup"><span data-stu-id="0da53-113">0</span></span>|<span data-ttu-id="0da53-114">Tráfego de túnel explicitamente não está configurado.</span><span class="sxs-lookup"><span data-stu-id="0da53-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="0da53-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="0da53-115">appProxy</span></span>|<span data-ttu-id="0da53-116">1</span><span class="sxs-lookup"><span data-stu-id="0da53-116">1</span></span>|<span data-ttu-id="0da53-117">Tráfego de túnel na camada de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0da53-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="0da53-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="0da53-118">packetTunnel</span></span>|<span data-ttu-id="0da53-119">2</span><span class="sxs-lookup"><span data-stu-id="0da53-119">2</span></span>|<span data-ttu-id="0da53-120">Tráfego de túnel na camada de IP.</span><span class="sxs-lookup"><span data-stu-id="0da53-120">Tunnel traffic at the IP layer.</span></span>|





