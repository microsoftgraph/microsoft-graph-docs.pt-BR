---
title: tipo de enumeração managedAppDeviceThreatLevel
description: O nível de ameaça máximo permitido para que um aplicativo seja compatível.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 63fa79d3ce378c64a870bb40f2491402fee34e99
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42781947"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="e4000-103">tipo de enumeração managedAppDeviceThreatLevel</span><span class="sxs-lookup"><span data-stu-id="e4000-103">managedAppDeviceThreatLevel enum type</span></span>

> <span data-ttu-id="e4000-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e4000-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e4000-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4000-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4000-106">O nível de ameaça máximo permitido para que um aplicativo seja compatível.</span><span class="sxs-lookup"><span data-stu-id="e4000-106">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="e4000-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e4000-107">Members</span></span>
|<span data-ttu-id="e4000-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e4000-108">Member</span></span>|<span data-ttu-id="e4000-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e4000-109">Value</span></span>|<span data-ttu-id="e4000-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4000-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4000-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e4000-111">notConfigured</span></span>|<span data-ttu-id="e4000-112">,0</span><span class="sxs-lookup"><span data-stu-id="e4000-112">0</span></span>|<span data-ttu-id="e4000-113">Valor não configurado</span><span class="sxs-lookup"><span data-stu-id="e4000-113">Value not configured</span></span>|
|<span data-ttu-id="e4000-114">presos</span><span class="sxs-lookup"><span data-stu-id="e4000-114">secured</span></span>|<span data-ttu-id="e4000-115">1</span><span class="sxs-lookup"><span data-stu-id="e4000-115">1</span></span>|<span data-ttu-id="e4000-116">O dispositivo precisa ter nenhuma ameaça</span><span class="sxs-lookup"><span data-stu-id="e4000-116">Device needs to have no threat</span></span>|
|<span data-ttu-id="e4000-117">low</span><span class="sxs-lookup"><span data-stu-id="e4000-117">low</span></span>|<span data-ttu-id="e4000-118">duas</span><span class="sxs-lookup"><span data-stu-id="e4000-118">2</span></span>|<span data-ttu-id="e4000-119">O dispositivo precisa ter uma baixa ameaça.</span><span class="sxs-lookup"><span data-stu-id="e4000-119">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="e4000-120">medium</span><span class="sxs-lookup"><span data-stu-id="e4000-120">medium</span></span>|<span data-ttu-id="e4000-121">3D</span><span class="sxs-lookup"><span data-stu-id="e4000-121">3</span></span>|<span data-ttu-id="e4000-122">O dispositivo precisa ter não mais do que o médio risco.</span><span class="sxs-lookup"><span data-stu-id="e4000-122">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="e4000-123">high</span><span class="sxs-lookup"><span data-stu-id="e4000-123">high</span></span>|<span data-ttu-id="e4000-124">4 </span><span class="sxs-lookup"><span data-stu-id="e4000-124">4</span></span>|<span data-ttu-id="e4000-125">O dispositivo precisa ter não mais do que a alta ameaça</span><span class="sxs-lookup"><span data-stu-id="e4000-125">Device needs to have not more than high threat</span></span>|



