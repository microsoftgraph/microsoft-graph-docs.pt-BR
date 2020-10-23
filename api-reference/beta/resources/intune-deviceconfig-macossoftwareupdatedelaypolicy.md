---
title: tipo de enumeração macOSSoftwareUpdateDelayPolicy
description: Sinalizador enum para determinar se deve atrasar as atualizações de software para o macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2f9d9100fc7bad05a6fd8d48a90a07cd268d0977
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731089"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a><span data-ttu-id="ba530-103">tipo de enumeração macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="ba530-103">macOSSoftwareUpdateDelayPolicy enum type</span></span>

<span data-ttu-id="ba530-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba530-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba530-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ba530-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba530-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ba530-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba530-107">Sinalizador enum para determinar se deve atrasar as atualizações de software para o macOS.</span><span class="sxs-lookup"><span data-stu-id="ba530-107">Flag enum to determine whether to delay software updates for macOS.</span></span>

## <a name="members"></a><span data-ttu-id="ba530-108">Membros</span><span class="sxs-lookup"><span data-stu-id="ba530-108">Members</span></span>
|<span data-ttu-id="ba530-109">Membro</span><span class="sxs-lookup"><span data-stu-id="ba530-109">Member</span></span>|<span data-ttu-id="ba530-110">Valor</span><span class="sxs-lookup"><span data-stu-id="ba530-110">Value</span></span>|<span data-ttu-id="ba530-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ba530-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba530-112">none</span><span class="sxs-lookup"><span data-stu-id="ba530-112">none</span></span>|<span data-ttu-id="ba530-113">,0</span><span class="sxs-lookup"><span data-stu-id="ba530-113">0</span></span>|<span data-ttu-id="ba530-114">Os atrasos de atualização de software não serão impostos.</span><span class="sxs-lookup"><span data-stu-id="ba530-114">Software update delays will not be enforced.</span></span>|
|<span data-ttu-id="ba530-115">delayOSUpdateVisibility</span><span class="sxs-lookup"><span data-stu-id="ba530-115">delayOSUpdateVisibility</span></span>|<span data-ttu-id="ba530-116">1</span><span class="sxs-lookup"><span data-stu-id="ba530-116">1</span></span>|<span data-ttu-id="ba530-117">Forçar atrasos para atualizações de software de so.</span><span class="sxs-lookup"><span data-stu-id="ba530-117">Force delays for OS software updates.</span></span>|
|<span data-ttu-id="ba530-118">delayAppUpdateVisibility</span><span class="sxs-lookup"><span data-stu-id="ba530-118">delayAppUpdateVisibility</span></span>|<span data-ttu-id="ba530-119">duas</span><span class="sxs-lookup"><span data-stu-id="ba530-119">2</span></span>|<span data-ttu-id="ba530-120">Forçar atrasos para atualizações de software de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ba530-120">Force delays for app software updates.</span></span>|





