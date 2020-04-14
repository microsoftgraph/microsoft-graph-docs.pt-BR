---
title: tipo de enumeração windowsAutopilotProfileAssignmentDetailedStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d681e18ba17e591e3c97833f540c322e6e37903e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358598"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="91b75-103">tipo de enumeração windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="91b75-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

<span data-ttu-id="91b75-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91b75-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="91b75-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="91b75-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91b75-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="91b75-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91b75-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="91b75-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="91b75-108">Membros</span><span class="sxs-lookup"><span data-stu-id="91b75-108">Members</span></span>
|<span data-ttu-id="91b75-109">Membro</span><span class="sxs-lookup"><span data-stu-id="91b75-109">Member</span></span>|<span data-ttu-id="91b75-110">Valor</span><span class="sxs-lookup"><span data-stu-id="91b75-110">Value</span></span>|<span data-ttu-id="91b75-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="91b75-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b75-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="91b75-112">none</span></span>|<span data-ttu-id="91b75-113">,0</span><span class="sxs-lookup"><span data-stu-id="91b75-113">0</span></span>|<span data-ttu-id="91b75-114">Nenhum status detalhado de atribuição</span><span class="sxs-lookup"><span data-stu-id="91b75-114">No assignment detailed status</span></span>|
|<span data-ttu-id="91b75-115">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="91b75-115">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="91b75-116">1</span><span class="sxs-lookup"><span data-stu-id="91b75-116">1</span></span>|<span data-ttu-id="91b75-117">Os requisitos de hardware não são atendidos.</span><span class="sxs-lookup"><span data-stu-id="91b75-117">Hardware requirements are not met.</span></span> <span data-ttu-id="91b75-118">Isso pode acontecer se um perfil autoimplantar do autoautoria for atribuído a um dispositivo sem o TPM 2,0.</span><span class="sxs-lookup"><span data-stu-id="91b75-118">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="91b75-119">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="91b75-119">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="91b75-120">duas</span><span class="sxs-lookup"><span data-stu-id="91b75-120">2</span></span>|<span data-ttu-id="91b75-121">Isso pode acontecer quando um perfil do AutoPilot do SurfaceHub é atribuído a um dispositivo que não é SurfaceHub.</span><span class="sxs-lookup"><span data-stu-id="91b75-121">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="91b75-122">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="91b75-122">holoLensProfileNotSupported</span></span>|<span data-ttu-id="91b75-123">3D</span><span class="sxs-lookup"><span data-stu-id="91b75-123">3</span></span>|<span data-ttu-id="91b75-124">Isso pode acontecer quando um perfil do AutoPilot do HoloLens é atribuído a um dispositivo que não é HoloLens.</span><span class="sxs-lookup"><span data-stu-id="91b75-124">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="91b75-125">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="91b75-125">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="91b75-126">4 </span><span class="sxs-lookup"><span data-stu-id="91b75-126">4</span></span>|<span data-ttu-id="91b75-127">Isso pode acontecer quando um perfil do AutoPilot do WindowsPc é atribuído a um dispositivo que não é WindowsPc.</span><span class="sxs-lookup"><span data-stu-id="91b75-127">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



