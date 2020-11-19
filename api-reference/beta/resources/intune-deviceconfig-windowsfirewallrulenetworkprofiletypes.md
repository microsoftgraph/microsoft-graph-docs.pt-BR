---
title: tipo de enumeração windowsFirewallRuleNetworkProfileTypes
description: Sinalizadores que representam quais tipos de perfil de rede se aplicam a uma regra de firewall.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9e46fccf175483090bc78ae0c070112c7e3f18e9
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49215328"
---
# <a name="windowsfirewallrulenetworkprofiletypes-enum-type"></a><span data-ttu-id="c0940-103">tipo de enumeração windowsFirewallRuleNetworkProfileTypes</span><span class="sxs-lookup"><span data-stu-id="c0940-103">windowsFirewallRuleNetworkProfileTypes enum type</span></span>

<span data-ttu-id="c0940-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c0940-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c0940-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c0940-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c0940-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c0940-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c0940-107">Sinalizadores que representam quais tipos de perfil de rede se aplicam a uma regra de firewall.</span><span class="sxs-lookup"><span data-stu-id="c0940-107">Flags representing which network profile types apply to a firewall rule.</span></span>

## <a name="members"></a><span data-ttu-id="c0940-108">Membros</span><span class="sxs-lookup"><span data-stu-id="c0940-108">Members</span></span>
|<span data-ttu-id="c0940-109">Membro</span><span class="sxs-lookup"><span data-stu-id="c0940-109">Member</span></span>|<span data-ttu-id="c0940-110">Valor</span><span class="sxs-lookup"><span data-stu-id="c0940-110">Value</span></span>|<span data-ttu-id="c0940-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c0940-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0940-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c0940-112">notConfigured</span></span>|<span data-ttu-id="c0940-113">,0</span><span class="sxs-lookup"><span data-stu-id="c0940-113">0</span></span>|<span data-ttu-id="c0940-114">Nenhum sinalizador definido.</span><span class="sxs-lookup"><span data-stu-id="c0940-114">No flags set.</span></span>|
|<span data-ttu-id="c0940-115">domínio</span><span class="sxs-lookup"><span data-stu-id="c0940-115">domain</span></span>|<span data-ttu-id="c0940-116">1</span><span class="sxs-lookup"><span data-stu-id="c0940-116">1</span></span>|<span data-ttu-id="c0940-117">O perfil para redes que estão conectadas a domínios.</span><span class="sxs-lookup"><span data-stu-id="c0940-117">The profile for networks that are connected to domains.</span></span>|
|<span data-ttu-id="c0940-118">privada</span><span class="sxs-lookup"><span data-stu-id="c0940-118">private</span></span>|<span data-ttu-id="c0940-119">duas</span><span class="sxs-lookup"><span data-stu-id="c0940-119">2</span></span>|<span data-ttu-id="c0940-120">O perfil para redes privadas.</span><span class="sxs-lookup"><span data-stu-id="c0940-120">The profile for private networks.</span></span>|
|<span data-ttu-id="c0940-121">public</span><span class="sxs-lookup"><span data-stu-id="c0940-121">public</span></span>|<span data-ttu-id="c0940-122">4 </span><span class="sxs-lookup"><span data-stu-id="c0940-122">4</span></span>|<span data-ttu-id="c0940-123">O perfil para redes públicas.</span><span class="sxs-lookup"><span data-stu-id="c0940-123">The profile for public networks.</span></span>|




