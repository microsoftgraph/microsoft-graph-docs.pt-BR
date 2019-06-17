---
title: tipo de enumeração dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis de DmaGuardDeviceEnumerationPolicy.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f4e534fca412c6d48ab9ea006f308a114c73def2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989914"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="71722-103">tipo de enumeração dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="71722-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="71722-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="71722-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="71722-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="71722-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71722-106">Valores possíveis de DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="71722-106">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="71722-107">Membros</span><span class="sxs-lookup"><span data-stu-id="71722-107">Members</span></span>
|<span data-ttu-id="71722-108">Membro</span><span class="sxs-lookup"><span data-stu-id="71722-108">Member</span></span>|<span data-ttu-id="71722-109">Valor</span><span class="sxs-lookup"><span data-stu-id="71722-109">Value</span></span>|<span data-ttu-id="71722-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="71722-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71722-111">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="71722-111">deviceDefault</span></span>|<span data-ttu-id="71722-112">,0</span><span class="sxs-lookup"><span data-stu-id="71722-112">0</span></span>|<span data-ttu-id="71722-113">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="71722-113">Default value.</span></span> <span data-ttu-id="71722-114">Dispositivos com remapeamento DMA os drivers incompatíveis só serão enumerados depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="71722-114">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="71722-115">blockAll</span><span class="sxs-lookup"><span data-stu-id="71722-115">blockAll</span></span>|<span data-ttu-id="71722-116">1</span><span class="sxs-lookup"><span data-stu-id="71722-116">1</span></span>|<span data-ttu-id="71722-117">Os dispositivos com remapeamento de DMA drivers incompatíveis nunca poderão iniciar e executar o DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="71722-117">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="71722-118">allowAll</span><span class="sxs-lookup"><span data-stu-id="71722-118">allowAll</span></span>|<span data-ttu-id="71722-119">duas</span><span class="sxs-lookup"><span data-stu-id="71722-119">2</span></span>|<span data-ttu-id="71722-120">Todos os dispositivos PCIe externos compatíveis com DMA serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="71722-120">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|





