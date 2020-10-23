---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5f1238c423fc12605c8ca2d3a8828d814a74b288
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48701575"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="d5fea-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="d5fea-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="d5fea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5fea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5fea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d5fea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5fea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d5fea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5fea-107">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="d5fea-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="d5fea-108">Membros</span><span class="sxs-lookup"><span data-stu-id="d5fea-108">Members</span></span>
|<span data-ttu-id="d5fea-109">Membro</span><span class="sxs-lookup"><span data-stu-id="d5fea-109">Member</span></span>|<span data-ttu-id="d5fea-110">Valor</span><span class="sxs-lookup"><span data-stu-id="d5fea-110">Value</span></span>|<span data-ttu-id="d5fea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d5fea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5fea-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="d5fea-112">deviceDefault</span></span>|<span data-ttu-id="d5fea-113">,0</span><span class="sxs-lookup"><span data-stu-id="d5fea-113">0</span></span>|<span data-ttu-id="d5fea-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="d5fea-114">Default value.</span></span> <span data-ttu-id="d5fea-115">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="d5fea-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="d5fea-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="d5fea-116">blockAll</span></span>|<span data-ttu-id="d5fea-117">1</span><span class="sxs-lookup"><span data-stu-id="d5fea-117">1</span></span>|<span data-ttu-id="d5fea-118">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="d5fea-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="d5fea-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="d5fea-119">allowAll</span></span>|<span data-ttu-id="d5fea-120">duas</span><span class="sxs-lookup"><span data-stu-id="d5fea-120">2</span></span>|<span data-ttu-id="d5fea-121">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="d5fea-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





