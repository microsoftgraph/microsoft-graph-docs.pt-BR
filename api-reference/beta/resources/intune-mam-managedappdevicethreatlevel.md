---
title: tipo de enumeração managedAppDeviceThreatLevel
description: O nível de ameaça máximo permitido para que um aplicativo seja compatível.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbecc5777380d69fd1b8ca64c84637d8d5490007
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43373073"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="1ccaa-103">tipo de enumeração managedAppDeviceThreatLevel</span><span class="sxs-lookup"><span data-stu-id="1ccaa-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="1ccaa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1ccaa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1ccaa-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ccaa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ccaa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ccaa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ccaa-107">O nível de ameaça máximo permitido para que um aplicativo seja compatível.</span><span class="sxs-lookup"><span data-stu-id="1ccaa-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="1ccaa-108">Membros</span><span class="sxs-lookup"><span data-stu-id="1ccaa-108">Members</span></span>
|<span data-ttu-id="1ccaa-109">Membro</span><span class="sxs-lookup"><span data-stu-id="1ccaa-109">Member</span></span>|<span data-ttu-id="1ccaa-110">Valor</span><span class="sxs-lookup"><span data-stu-id="1ccaa-110">Value</span></span>|<span data-ttu-id="1ccaa-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ccaa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ccaa-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="1ccaa-112">notConfigured</span></span>|<span data-ttu-id="1ccaa-113">,0</span><span class="sxs-lookup"><span data-stu-id="1ccaa-113">0</span></span>|<span data-ttu-id="1ccaa-114">Valor não configurado</span><span class="sxs-lookup"><span data-stu-id="1ccaa-114">Value not configured</span></span>|
|<span data-ttu-id="1ccaa-115">presos</span><span class="sxs-lookup"><span data-stu-id="1ccaa-115">secured</span></span>|<span data-ttu-id="1ccaa-116">1</span><span class="sxs-lookup"><span data-stu-id="1ccaa-116">1</span></span>|<span data-ttu-id="1ccaa-117">O dispositivo precisa ter nenhuma ameaça</span><span class="sxs-lookup"><span data-stu-id="1ccaa-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="1ccaa-118">low</span><span class="sxs-lookup"><span data-stu-id="1ccaa-118">low</span></span>|<span data-ttu-id="1ccaa-119">duas</span><span class="sxs-lookup"><span data-stu-id="1ccaa-119">2</span></span>|<span data-ttu-id="1ccaa-120">O dispositivo precisa ter uma baixa ameaça.</span><span class="sxs-lookup"><span data-stu-id="1ccaa-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="1ccaa-121">medium</span><span class="sxs-lookup"><span data-stu-id="1ccaa-121">medium</span></span>|<span data-ttu-id="1ccaa-122">3D</span><span class="sxs-lookup"><span data-stu-id="1ccaa-122">3</span></span>|<span data-ttu-id="1ccaa-123">O dispositivo precisa ter não mais do que o médio risco.</span><span class="sxs-lookup"><span data-stu-id="1ccaa-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="1ccaa-124">high</span><span class="sxs-lookup"><span data-stu-id="1ccaa-124">high</span></span>|<span data-ttu-id="1ccaa-125">4 </span><span class="sxs-lookup"><span data-stu-id="1ccaa-125">4</span></span>|<span data-ttu-id="1ccaa-126">O dispositivo precisa ter não mais do que a alta ameaça</span><span class="sxs-lookup"><span data-stu-id="1ccaa-126">Device needs to have not more than high threat</span></span>|



