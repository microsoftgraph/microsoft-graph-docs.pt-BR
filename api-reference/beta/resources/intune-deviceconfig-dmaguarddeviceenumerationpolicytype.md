---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e3289a40916d4942980274e2375aefdf6081934c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42791965"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="e293f-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="e293f-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="e293f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e293f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e293f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e293f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e293f-106">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="e293f-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="e293f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e293f-107">Members</span></span>
|<span data-ttu-id="e293f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e293f-108">Member</span></span>|<span data-ttu-id="e293f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e293f-109">Value</span></span>|<span data-ttu-id="e293f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e293f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e293f-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="e293f-111">deviceDefault</span></span>|<span data-ttu-id="e293f-112">,0</span><span class="sxs-lookup"><span data-stu-id="e293f-112">0</span></span>|<span data-ttu-id="e293f-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="e293f-113">Default value.</span></span> <span data-ttu-id="e293f-114">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="e293f-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="e293f-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="e293f-115">blockAll</span></span>|<span data-ttu-id="e293f-116">1</span><span class="sxs-lookup"><span data-stu-id="e293f-116">1</span></span>|<span data-ttu-id="e293f-117">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="e293f-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="e293f-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="e293f-118">allowAll</span></span>|<span data-ttu-id="e293f-119">duas</span><span class="sxs-lookup"><span data-stu-id="e293f-119">2</span></span>|<span data-ttu-id="e293f-120">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="e293f-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



