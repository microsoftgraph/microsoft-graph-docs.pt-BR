---
title: tipo de enum vpnProviderType
description: Tipo de provedor para VPN-app.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2de8f78222ba0c945000b84f28039c2f6af58daa
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407218"
---
# <a name="vpnprovidertype-enum-type"></a><span data-ttu-id="9e1ae-103">tipo de enum vpnProviderType</span><span class="sxs-lookup"><span data-stu-id="9e1ae-103">vpnProviderType enum type</span></span>

> <span data-ttu-id="9e1ae-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9e1ae-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e1ae-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e1ae-107">Tipo de provedor para VPN-app.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-107">Provider type for per-app VPN.</span></span>

## <a name="members"></a><span data-ttu-id="9e1ae-108">Membros</span><span class="sxs-lookup"><span data-stu-id="9e1ae-108">Members</span></span>
|<span data-ttu-id="9e1ae-109">Membro</span><span class="sxs-lookup"><span data-stu-id="9e1ae-109">Member</span></span>|<span data-ttu-id="9e1ae-110">Valor</span><span class="sxs-lookup"><span data-stu-id="9e1ae-110">Value</span></span>|<span data-ttu-id="9e1ae-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9e1ae-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e1ae-112">não-configuradas</span><span class="sxs-lookup"><span data-stu-id="9e1ae-112">notConfigured</span></span>|<span data-ttu-id="9e1ae-113">0</span><span class="sxs-lookup"><span data-stu-id="9e1ae-113">0</span></span>|<span data-ttu-id="9e1ae-114">Tráfego de túnel explicitamente não está configurado.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-114">Tunnel traffic is not explicitly configured.</span></span>|
|<span data-ttu-id="9e1ae-115">appProxy</span><span class="sxs-lookup"><span data-stu-id="9e1ae-115">appProxy</span></span>|<span data-ttu-id="9e1ae-116">1</span><span class="sxs-lookup"><span data-stu-id="9e1ae-116">1</span></span>|<span data-ttu-id="9e1ae-117">Tráfego de túnel na camada de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-117">Tunnel traffic at the application layer.</span></span>|
|<span data-ttu-id="9e1ae-118">packetTunnel</span><span class="sxs-lookup"><span data-stu-id="9e1ae-118">packetTunnel</span></span>|<span data-ttu-id="9e1ae-119">2</span><span class="sxs-lookup"><span data-stu-id="9e1ae-119">2</span></span>|<span data-ttu-id="9e1ae-120">Tráfego de túnel na camada de IP.</span><span class="sxs-lookup"><span data-stu-id="9e1ae-120">Tunnel traffic at the IP layer.</span></span>|




