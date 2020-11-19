---
title: tipo de enumeração macOSSoftwareUpdateDelayPolicy
description: Sinalizador enum para determinar se deve atrasar as atualizações de software para o macOS.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 87f4b34447ee8cba65153fcff903239061aef17b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279868"
---
# <a name="macossoftwareupdatedelaypolicy-enum-type"></a><span data-ttu-id="e7618-103">tipo de enumeração macOSSoftwareUpdateDelayPolicy</span><span class="sxs-lookup"><span data-stu-id="e7618-103">macOSSoftwareUpdateDelayPolicy enum type</span></span>

<span data-ttu-id="e7618-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7618-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7618-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e7618-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7618-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e7618-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7618-107">Sinalizador enum para determinar se deve atrasar as atualizações de software para o macOS.</span><span class="sxs-lookup"><span data-stu-id="e7618-107">Flag enum to determine whether to delay software updates for macOS.</span></span>

## <a name="members"></a><span data-ttu-id="e7618-108">Membros</span><span class="sxs-lookup"><span data-stu-id="e7618-108">Members</span></span>
|<span data-ttu-id="e7618-109">Membro</span><span class="sxs-lookup"><span data-stu-id="e7618-109">Member</span></span>|<span data-ttu-id="e7618-110">Valor</span><span class="sxs-lookup"><span data-stu-id="e7618-110">Value</span></span>|<span data-ttu-id="e7618-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="e7618-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7618-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="e7618-112">none</span></span>|<span data-ttu-id="e7618-113">,0</span><span class="sxs-lookup"><span data-stu-id="e7618-113">0</span></span>|<span data-ttu-id="e7618-114">Os atrasos de atualização de software não serão impostos.</span><span class="sxs-lookup"><span data-stu-id="e7618-114">Software update delays will not be enforced.</span></span>|
|<span data-ttu-id="e7618-115">delayOSUpdateVisibility</span><span class="sxs-lookup"><span data-stu-id="e7618-115">delayOSUpdateVisibility</span></span>|<span data-ttu-id="e7618-116">1</span><span class="sxs-lookup"><span data-stu-id="e7618-116">1</span></span>|<span data-ttu-id="e7618-117">Forçar atrasos para atualizações de software de so.</span><span class="sxs-lookup"><span data-stu-id="e7618-117">Force delays for OS software updates.</span></span>|
|<span data-ttu-id="e7618-118">delayAppUpdateVisibility</span><span class="sxs-lookup"><span data-stu-id="e7618-118">delayAppUpdateVisibility</span></span>|<span data-ttu-id="e7618-119">duas</span><span class="sxs-lookup"><span data-stu-id="e7618-119">2</span></span>|<span data-ttu-id="e7618-120">Forçar atrasos para atualizações de software de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e7618-120">Force delays for app software updates.</span></span>|




