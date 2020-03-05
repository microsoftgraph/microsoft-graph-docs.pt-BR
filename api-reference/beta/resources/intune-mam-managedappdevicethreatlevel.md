---
title: tipo de enumeração managedAppDeviceThreatLevel
description: O nível de ameaça máximo permitido para que um aplicativo seja compatível.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: df62fd78a6cf26eec9c3850bde0389c5e48cc91d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527935"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="2d94d-103">tipo de enumeração managedAppDeviceThreatLevel</span><span class="sxs-lookup"><span data-stu-id="2d94d-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="2d94d-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="2d94d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2d94d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2d94d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2d94d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2d94d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2d94d-107">O nível de ameaça máximo permitido para que um aplicativo seja compatível.</span><span class="sxs-lookup"><span data-stu-id="2d94d-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="2d94d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="2d94d-108">Members</span></span>
|<span data-ttu-id="2d94d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="2d94d-109">Member</span></span>|<span data-ttu-id="2d94d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="2d94d-110">Value</span></span>|<span data-ttu-id="2d94d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2d94d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d94d-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="2d94d-112">notConfigured</span></span>|<span data-ttu-id="2d94d-113">,0</span><span class="sxs-lookup"><span data-stu-id="2d94d-113">0</span></span>|<span data-ttu-id="2d94d-114">Valor não configurado</span><span class="sxs-lookup"><span data-stu-id="2d94d-114">Value not configured</span></span>|
|<span data-ttu-id="2d94d-115">presos</span><span class="sxs-lookup"><span data-stu-id="2d94d-115">secured</span></span>|<span data-ttu-id="2d94d-116">1 </span><span class="sxs-lookup"><span data-stu-id="2d94d-116">1</span></span>|<span data-ttu-id="2d94d-117">O dispositivo precisa ter nenhuma ameaça</span><span class="sxs-lookup"><span data-stu-id="2d94d-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="2d94d-118">low</span><span class="sxs-lookup"><span data-stu-id="2d94d-118">low</span></span>|<span data-ttu-id="2d94d-119">2 </span><span class="sxs-lookup"><span data-stu-id="2d94d-119">2</span></span>|<span data-ttu-id="2d94d-120">O dispositivo precisa ter uma baixa ameaça.</span><span class="sxs-lookup"><span data-stu-id="2d94d-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="2d94d-121">medium</span><span class="sxs-lookup"><span data-stu-id="2d94d-121">medium</span></span>|<span data-ttu-id="2d94d-122">3 </span><span class="sxs-lookup"><span data-stu-id="2d94d-122">3</span></span>|<span data-ttu-id="2d94d-123">O dispositivo precisa ter não mais do que o médio risco.</span><span class="sxs-lookup"><span data-stu-id="2d94d-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="2d94d-124">high</span><span class="sxs-lookup"><span data-stu-id="2d94d-124">high</span></span>|<span data-ttu-id="2d94d-125">4 </span><span class="sxs-lookup"><span data-stu-id="2d94d-125">4</span></span>|<span data-ttu-id="2d94d-126">O dispositivo precisa ter não mais do que a alta ameaça</span><span class="sxs-lookup"><span data-stu-id="2d94d-126">Device needs to have not more than high threat</span></span>|



