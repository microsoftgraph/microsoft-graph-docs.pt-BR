---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f735a5ce77c0162899d7e93974a07de4f0be137b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469160"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="45f69-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="45f69-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="45f69-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45f69-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="45f69-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="45f69-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="45f69-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="45f69-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="45f69-107">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="45f69-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="45f69-108">Membros</span><span class="sxs-lookup"><span data-stu-id="45f69-108">Members</span></span>
|<span data-ttu-id="45f69-109">Membro</span><span class="sxs-lookup"><span data-stu-id="45f69-109">Member</span></span>|<span data-ttu-id="45f69-110">Valor</span><span class="sxs-lookup"><span data-stu-id="45f69-110">Value</span></span>|<span data-ttu-id="45f69-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="45f69-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45f69-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="45f69-112">deviceDefault</span></span>|<span data-ttu-id="45f69-113">,0</span><span class="sxs-lookup"><span data-stu-id="45f69-113">0</span></span>|<span data-ttu-id="45f69-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="45f69-114">Default value.</span></span> <span data-ttu-id="45f69-115">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="45f69-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="45f69-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="45f69-116">blockAll</span></span>|<span data-ttu-id="45f69-117">1</span><span class="sxs-lookup"><span data-stu-id="45f69-117">1</span></span>|<span data-ttu-id="45f69-118">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="45f69-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="45f69-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="45f69-119">allowAll</span></span>|<span data-ttu-id="45f69-120">duas</span><span class="sxs-lookup"><span data-stu-id="45f69-120">2</span></span>|<span data-ttu-id="45f69-121">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="45f69-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



