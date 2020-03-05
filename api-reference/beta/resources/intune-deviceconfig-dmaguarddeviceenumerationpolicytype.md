---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03e93e6ad3e5dae8a455bb3ceb9aa65f11dcf2e1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526570"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="766bf-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="766bf-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

<span data-ttu-id="766bf-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="766bf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="766bf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="766bf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="766bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="766bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="766bf-107">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="766bf-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="766bf-108">Membros</span><span class="sxs-lookup"><span data-stu-id="766bf-108">Members</span></span>
|<span data-ttu-id="766bf-109">Membro</span><span class="sxs-lookup"><span data-stu-id="766bf-109">Member</span></span>|<span data-ttu-id="766bf-110">Valor</span><span class="sxs-lookup"><span data-stu-id="766bf-110">Value</span></span>|<span data-ttu-id="766bf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="766bf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="766bf-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="766bf-112">deviceDefault</span></span>|<span data-ttu-id="766bf-113">,0</span><span class="sxs-lookup"><span data-stu-id="766bf-113">0</span></span>|<span data-ttu-id="766bf-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="766bf-114">Default value.</span></span> <span data-ttu-id="766bf-115">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="766bf-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="766bf-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="766bf-116">blockAll</span></span>|<span data-ttu-id="766bf-117">1 </span><span class="sxs-lookup"><span data-stu-id="766bf-117">1</span></span>|<span data-ttu-id="766bf-118">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="766bf-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="766bf-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="766bf-119">allowAll</span></span>|<span data-ttu-id="766bf-120">2 </span><span class="sxs-lookup"><span data-stu-id="766bf-120">2</span></span>|<span data-ttu-id="766bf-121">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="766bf-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|



