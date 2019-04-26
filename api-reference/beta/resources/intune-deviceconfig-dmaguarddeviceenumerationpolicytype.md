---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6910172ef4ab733b09d837dcc9a7196893402ab
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567155"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="39c63-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="39c63-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="39c63-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="39c63-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="39c63-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="39c63-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="39c63-106">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="39c63-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="39c63-107">Membros</span><span class="sxs-lookup"><span data-stu-id="39c63-107">Members</span></span>
|<span data-ttu-id="39c63-108">Membro</span><span class="sxs-lookup"><span data-stu-id="39c63-108">Member</span></span>|<span data-ttu-id="39c63-109">Valor</span><span class="sxs-lookup"><span data-stu-id="39c63-109">Value</span></span>|<span data-ttu-id="39c63-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="39c63-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39c63-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="39c63-111">deviceDefault</span></span>|<span data-ttu-id="39c63-112">,0</span><span class="sxs-lookup"><span data-stu-id="39c63-112">0</span></span>|<span data-ttu-id="39c63-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="39c63-113">Default value.</span></span> <span data-ttu-id="39c63-114">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="39c63-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="39c63-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="39c63-115">blockAll</span></span>|<span data-ttu-id="39c63-116">1 </span><span class="sxs-lookup"><span data-stu-id="39c63-116">1</span></span>|<span data-ttu-id="39c63-117">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="39c63-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="39c63-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="39c63-118">allowAll</span></span>|<span data-ttu-id="39c63-119">2 </span><span class="sxs-lookup"><span data-stu-id="39c63-119">2</span></span>|<span data-ttu-id="39c63-120">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="39c63-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





