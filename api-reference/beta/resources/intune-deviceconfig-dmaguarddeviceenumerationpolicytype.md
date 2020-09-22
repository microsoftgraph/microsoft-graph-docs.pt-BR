---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2296198c9e433fbaf7d6499eca7737306c581618
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48058313"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="f35e3-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="f35e3-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="f35e3-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f35e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f35e3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f35e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f35e3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f35e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f35e3-107">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="f35e3-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="f35e3-108">Membros</span><span class="sxs-lookup"><span data-stu-id="f35e3-108">Members</span></span>
|<span data-ttu-id="f35e3-109">Membro</span><span class="sxs-lookup"><span data-stu-id="f35e3-109">Member</span></span>|<span data-ttu-id="f35e3-110">Valor</span><span class="sxs-lookup"><span data-stu-id="f35e3-110">Value</span></span>|<span data-ttu-id="f35e3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="f35e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f35e3-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="f35e3-112">deviceDefault</span></span>|<span data-ttu-id="f35e3-113">,0</span><span class="sxs-lookup"><span data-stu-id="f35e3-113">0</span></span>|<span data-ttu-id="f35e3-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="f35e3-114">Default value.</span></span> <span data-ttu-id="f35e3-115">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="f35e3-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="f35e3-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="f35e3-116">blockAll</span></span>|<span data-ttu-id="f35e3-117">1 </span><span class="sxs-lookup"><span data-stu-id="f35e3-117">1</span></span>|<span data-ttu-id="f35e3-118">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="f35e3-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="f35e3-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="f35e3-119">allowAll</span></span>|<span data-ttu-id="f35e3-120">2 </span><span class="sxs-lookup"><span data-stu-id="f35e3-120">2</span></span>|<span data-ttu-id="f35e3-121">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="f35e3-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|






