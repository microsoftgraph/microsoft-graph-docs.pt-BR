---
title: tipo de enumeração managedAppDeviceThreatLevel
description: O nível de ameaça máximo permitido para que um aplicativo seja compatível.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f262c53d62d791e456edcd234249448e0c90580c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49266911"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="832f2-103">tipo de enumeração managedAppDeviceThreatLevel</span><span class="sxs-lookup"><span data-stu-id="832f2-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="832f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="832f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="832f2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="832f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="832f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="832f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="832f2-107">O nível de ameaça máximo permitido para que um aplicativo seja compatível.</span><span class="sxs-lookup"><span data-stu-id="832f2-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="832f2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="832f2-108">Members</span></span>
|<span data-ttu-id="832f2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="832f2-109">Member</span></span>|<span data-ttu-id="832f2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="832f2-110">Value</span></span>|<span data-ttu-id="832f2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="832f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="832f2-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="832f2-112">notConfigured</span></span>|<span data-ttu-id="832f2-113">,0</span><span class="sxs-lookup"><span data-stu-id="832f2-113">0</span></span>|<span data-ttu-id="832f2-114">Valor não configurado</span><span class="sxs-lookup"><span data-stu-id="832f2-114">Value not configured</span></span>|
|<span data-ttu-id="832f2-115">presos</span><span class="sxs-lookup"><span data-stu-id="832f2-115">secured</span></span>|<span data-ttu-id="832f2-116">1</span><span class="sxs-lookup"><span data-stu-id="832f2-116">1</span></span>|<span data-ttu-id="832f2-117">O dispositivo precisa ter nenhuma ameaça</span><span class="sxs-lookup"><span data-stu-id="832f2-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="832f2-118">low</span><span class="sxs-lookup"><span data-stu-id="832f2-118">low</span></span>|<span data-ttu-id="832f2-119">duas</span><span class="sxs-lookup"><span data-stu-id="832f2-119">2</span></span>|<span data-ttu-id="832f2-120">O dispositivo precisa ter uma baixa ameaça.</span><span class="sxs-lookup"><span data-stu-id="832f2-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="832f2-121">medium</span><span class="sxs-lookup"><span data-stu-id="832f2-121">medium</span></span>|<span data-ttu-id="832f2-122">3D</span><span class="sxs-lookup"><span data-stu-id="832f2-122">3</span></span>|<span data-ttu-id="832f2-123">O dispositivo precisa ter não mais do que o médio risco.</span><span class="sxs-lookup"><span data-stu-id="832f2-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="832f2-124">high</span><span class="sxs-lookup"><span data-stu-id="832f2-124">high</span></span>|<span data-ttu-id="832f2-125">4 </span><span class="sxs-lookup"><span data-stu-id="832f2-125">4</span></span>|<span data-ttu-id="832f2-126">O dispositivo precisa ter não mais do que a alta ameaça</span><span class="sxs-lookup"><span data-stu-id="832f2-126">Device needs to have not more than high threat</span></span>|




