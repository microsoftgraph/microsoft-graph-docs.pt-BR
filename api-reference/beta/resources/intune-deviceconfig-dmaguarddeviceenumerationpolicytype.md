---
title: tipo de enum dmaGuardDeviceEnumerationPolicyType
description: Valores possíveis a DmaGuardDeviceEnumerationPolicy.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5baa0cfd5c80f954036e10f0e4d04d2b83e57f2b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429158"
---
# <a name="dmaguarddeviceenumerationpolicytype-enum-type"></a><span data-ttu-id="12e2d-103">tipo de enum dmaGuardDeviceEnumerationPolicyType</span><span class="sxs-lookup"><span data-stu-id="12e2d-103">dmaGuardDeviceEnumerationPolicyType enum type</span></span>

> <span data-ttu-id="12e2d-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="12e2d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="12e2d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="12e2d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="12e2d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="12e2d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="12e2d-107">Valores possíveis a DmaGuardDeviceEnumerationPolicy.</span><span class="sxs-lookup"><span data-stu-id="12e2d-107">Possible values of the DmaGuardDeviceEnumerationPolicy.</span></span>

## <a name="members"></a><span data-ttu-id="12e2d-108">Membros</span><span class="sxs-lookup"><span data-stu-id="12e2d-108">Members</span></span>
|<span data-ttu-id="12e2d-109">Membro</span><span class="sxs-lookup"><span data-stu-id="12e2d-109">Member</span></span>|<span data-ttu-id="12e2d-110">Valor</span><span class="sxs-lookup"><span data-stu-id="12e2d-110">Value</span></span>|<span data-ttu-id="12e2d-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="12e2d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="12e2d-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="12e2d-112">deviceDefault</span></span>|<span data-ttu-id="12e2d-113">0</span><span class="sxs-lookup"><span data-stu-id="12e2d-113">0</span></span>|<span data-ttu-id="12e2d-114">Valor padrão.</span><span class="sxs-lookup"><span data-stu-id="12e2d-114">Default value.</span></span> <span data-ttu-id="12e2d-115">Dispositivos com DMA novo mapeamento drivers incompatíveis serão enumerados somente depois que o usuário desbloqueia a tela.</span><span class="sxs-lookup"><span data-stu-id="12e2d-115">Devices with DMA remapping incompatible drivers will only be enumerated after the user unlocks the screen.</span></span>|
|<span data-ttu-id="12e2d-116">blockAll</span><span class="sxs-lookup"><span data-stu-id="12e2d-116">blockAll</span></span>|<span data-ttu-id="12e2d-117">1</span><span class="sxs-lookup"><span data-stu-id="12e2d-117">1</span></span>|<span data-ttu-id="12e2d-118">Dispositivos com DMA novo mapeamento drivers incompatíveis nunca poderão iniciar e executar DMA a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="12e2d-118">Devices with DMA remapping incompatible drivers will never be allowed to start and perform DMA at any time.</span></span>|
|<span data-ttu-id="12e2d-119">allowAll</span><span class="sxs-lookup"><span data-stu-id="12e2d-119">allowAll</span></span>|<span data-ttu-id="12e2d-120">2</span><span class="sxs-lookup"><span data-stu-id="12e2d-120">2</span></span>|<span data-ttu-id="12e2d-121">Todos os DMA capaz PCIe dispositivos externos serão enumerados a qualquer momento.</span><span class="sxs-lookup"><span data-stu-id="12e2d-121">All external DMA capable PCIe devices will be enumerated at any time.</span></span>|




