---
title: tipo de enumeração windowsFirewallRuleNetworkProfileTypes
description: Sinalizadores que representam quais tipos de perfil de rede se aplicam a uma regra de firewall.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3cd5c501c50f74e53c0c00fcef2d3bb8a85cedf7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32570121"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="c8d9e-103">tipo de enumeração windowsFirewallRuleNetworkProfileTypes</span><span class="sxs-lookup"><span data-stu-id="c8d9e-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

> <span data-ttu-id="c8d9e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c8d9e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c8d9e-106">Sinalizadores que representam quais tipos de perfil de rede se aplicam a uma regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-106">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="c8d9e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c8d9e-107">Members</span></span>
|<span data-ttu-id="c8d9e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c8d9e-108">Member</span></span>|<span data-ttu-id="c8d9e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c8d9e-109">Value</span></span>|<span data-ttu-id="c8d9e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c8d9e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8d9e-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c8d9e-111">notConfigured</span></span>|<span data-ttu-id="c8d9e-112">,0</span><span class="sxs-lookup"><span data-stu-id="c8d9e-112">0</span></span>|<span data-ttu-id="c8d9e-113">Nenhum sinalizador definido.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-113">No flags set.</span></span>|
|<span data-ttu-id="c8d9e-114">domínio</span><span class="sxs-lookup"><span data-stu-id="c8d9e-114">domain</span></span>|<span data-ttu-id="c8d9e-115">1 </span><span class="sxs-lookup"><span data-stu-id="c8d9e-115">1</span></span>|<span data-ttu-id="c8d9e-116">O perfil para redes que estão conectadas a domínios.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-116">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="c8d9e-117">privada</span><span class="sxs-lookup"><span data-stu-id="c8d9e-117">private</span></span>|<span data-ttu-id="c8d9e-118">2 </span><span class="sxs-lookup"><span data-stu-id="c8d9e-118">2</span></span>|<span data-ttu-id="c8d9e-119">O perfil para redes privadas.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-119">The profile for private networks.</span></span>|
|<span data-ttu-id="c8d9e-120">public</span><span class="sxs-lookup"><span data-stu-id="c8d9e-120">public</span></span>|<span data-ttu-id="c8d9e-121">4 </span><span class="sxs-lookup"><span data-stu-id="c8d9e-121">4</span></span>|<span data-ttu-id="c8d9e-122">O perfil para redes públicas.</span><span class="sxs-lookup"><span data-stu-id="c8d9e-122">The profile for public networks.</span></span>|





