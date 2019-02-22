---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 512bf44d25629f4b1c88c2309c464e9d0f33f625
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159707"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="3440d-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="3440d-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="3440d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3440d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3440d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3440d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3440d-106">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="3440d-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="3440d-107">Membros</span><span class="sxs-lookup"><span data-stu-id="3440d-107">Members</span></span>
|<span data-ttu-id="3440d-108">Membro</span><span class="sxs-lookup"><span data-stu-id="3440d-108">Member</span></span>|<span data-ttu-id="3440d-109">Valor</span><span class="sxs-lookup"><span data-stu-id="3440d-109">Value</span></span>|<span data-ttu-id="3440d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="3440d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3440d-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="3440d-111">deviceDefault</span></span>|<span data-ttu-id="3440d-112">,0</span><span class="sxs-lookup"><span data-stu-id="3440d-112">0</span></span>|<span data-ttu-id="3440d-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="3440d-113">Default value.</span></span> <span data-ttu-id="3440d-114">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="3440d-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="3440d-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="3440d-115">blockAll</span></span>|<span data-ttu-id="3440d-116">1</span><span class="sxs-lookup"><span data-stu-id="3440d-116">1</span></span>|<span data-ttu-id="3440d-117">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="3440d-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="3440d-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="3440d-118">allowAll</span></span>|<span data-ttu-id="3440d-119">duas</span><span class="sxs-lookup"><span data-stu-id="3440d-119">2</span></span>|<span data-ttu-id="3440d-120">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="3440d-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




