---
title: tipo de enumeração managedAppDeviceThreatLevel
description: O nível de ameaça máximo permitido para que um aplicativo seja compatível.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 09bdc52d0d7bfb51f9d04bdc7954c541836dcb76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030343"
---
# <a name="managedappdevicethreatlevel-enum-type"></a><span data-ttu-id="02e6f-103">tipo de enumeração managedAppDeviceThreatLevel</span><span class="sxs-lookup"><span data-stu-id="02e6f-103">managedAppDeviceThreatLevel enum type</span></span>

<span data-ttu-id="02e6f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02e6f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02e6f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="02e6f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02e6f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="02e6f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02e6f-107">O nível de ameaça máximo permitido para que um aplicativo seja compatível.</span><span class="sxs-lookup"><span data-stu-id="02e6f-107">The maxium threat level allowed for an app to be compliant.</span></span>

## <a name="members"></a><span data-ttu-id="02e6f-108">Membros</span><span class="sxs-lookup"><span data-stu-id="02e6f-108">Members</span></span>
|<span data-ttu-id="02e6f-109">Membro</span><span class="sxs-lookup"><span data-stu-id="02e6f-109">Member</span></span>|<span data-ttu-id="02e6f-110">Valor</span><span class="sxs-lookup"><span data-stu-id="02e6f-110">Value</span></span>|<span data-ttu-id="02e6f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="02e6f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02e6f-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="02e6f-112">notConfigured</span></span>|<span data-ttu-id="02e6f-113">,0</span><span class="sxs-lookup"><span data-stu-id="02e6f-113">0</span></span>|<span data-ttu-id="02e6f-114">Valor não configurado</span><span class="sxs-lookup"><span data-stu-id="02e6f-114">Value not configured</span></span>|
|<span data-ttu-id="02e6f-115">presos</span><span class="sxs-lookup"><span data-stu-id="02e6f-115">secured</span></span>|<span data-ttu-id="02e6f-116">1 </span><span class="sxs-lookup"><span data-stu-id="02e6f-116">1</span></span>|<span data-ttu-id="02e6f-117">O dispositivo precisa ter nenhuma ameaça</span><span class="sxs-lookup"><span data-stu-id="02e6f-117">Device needs to have no threat</span></span>|
|<span data-ttu-id="02e6f-118">low</span><span class="sxs-lookup"><span data-stu-id="02e6f-118">low</span></span>|<span data-ttu-id="02e6f-119">2 </span><span class="sxs-lookup"><span data-stu-id="02e6f-119">2</span></span>|<span data-ttu-id="02e6f-120">O dispositivo precisa ter uma baixa ameaça.</span><span class="sxs-lookup"><span data-stu-id="02e6f-120">Device needs to have a low threat.</span></span>|
|<span data-ttu-id="02e6f-121">medium</span><span class="sxs-lookup"><span data-stu-id="02e6f-121">medium</span></span>|<span data-ttu-id="02e6f-122">3 </span><span class="sxs-lookup"><span data-stu-id="02e6f-122">3</span></span>|<span data-ttu-id="02e6f-123">O dispositivo precisa ter não mais do que o médio risco.</span><span class="sxs-lookup"><span data-stu-id="02e6f-123">Device needs to have not more than medium threat.</span></span>|
|<span data-ttu-id="02e6f-124">high</span><span class="sxs-lookup"><span data-stu-id="02e6f-124">high</span></span>|<span data-ttu-id="02e6f-125">4 </span><span class="sxs-lookup"><span data-stu-id="02e6f-125">4</span></span>|<span data-ttu-id="02e6f-126">O dispositivo precisa ter não mais do que a alta ameaça</span><span class="sxs-lookup"><span data-stu-id="02e6f-126">Device needs to have not more than high threat</span></span>|






