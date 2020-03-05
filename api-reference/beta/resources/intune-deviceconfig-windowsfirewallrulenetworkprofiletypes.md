---
title: tipo de enumeração windowsFirewallRuleNetworkProfileTypes
description: Sinalizadores que representam quais tipos de perfil de rede se aplicam a uma regra de firewall.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0d57b5e52261ac720090921003665b05dd467ad1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525548"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="68ae3-103">tipo de enumeração windowsFirewallRuleNetworkProfileTypes</span><span class="sxs-lookup"><span data-stu-id="68ae3-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="68ae3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="68ae3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68ae3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="68ae3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68ae3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="68ae3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68ae3-107">Sinalizadores que representam quais tipos de perfil de rede se aplicam a uma regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="68ae3-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="68ae3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="68ae3-108">Members</span></span>
|<span data-ttu-id="68ae3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="68ae3-109">Member</span></span>|<span data-ttu-id="68ae3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="68ae3-110">Value</span></span>|<span data-ttu-id="68ae3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="68ae3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68ae3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="68ae3-112">notConfigured</span></span>|<span data-ttu-id="68ae3-113">,0</span><span class="sxs-lookup"><span data-stu-id="68ae3-113">0</span></span>|<span data-ttu-id="68ae3-114">Nenhum sinalizador definido.</span><span class="sxs-lookup"><span data-stu-id="68ae3-114">No flags set.</span></span>|
|<span data-ttu-id="68ae3-115">domínio</span><span class="sxs-lookup"><span data-stu-id="68ae3-115">domain</span></span>|<span data-ttu-id="68ae3-116">1 </span><span class="sxs-lookup"><span data-stu-id="68ae3-116">1</span></span>|<span data-ttu-id="68ae3-117">O perfil para redes que estão conectadas a domínios.</span><span class="sxs-lookup"><span data-stu-id="68ae3-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="68ae3-118">privada</span><span class="sxs-lookup"><span data-stu-id="68ae3-118">private</span></span>|<span data-ttu-id="68ae3-119">2 </span><span class="sxs-lookup"><span data-stu-id="68ae3-119">2</span></span>|<span data-ttu-id="68ae3-120">O perfil para redes privadas.</span><span class="sxs-lookup"><span data-stu-id="68ae3-120">The profile for private networks.</span></span>|
|<span data-ttu-id="68ae3-121">public</span><span class="sxs-lookup"><span data-stu-id="68ae3-121">public</span></span>|<span data-ttu-id="68ae3-122">4 </span><span class="sxs-lookup"><span data-stu-id="68ae3-122">4</span></span>|<span data-ttu-id="68ae3-123">O perfil para redes públicas.</span><span class="sxs-lookup"><span data-stu-id="68ae3-123">The profile for public networks.</span></span>|



