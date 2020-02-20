---
title: tipo de enumeração windowsAutopilotProfileAssignmentDetailedStatus
description: Ainda não documentado
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 418670dd5f334b169d43022a9908c2a39f279b60
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/20/2020
ms.locfileid: "42163896"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="8c12f-103">tipo de enumeração windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="8c12f-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

> <span data-ttu-id="8c12f-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8c12f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8c12f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8c12f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c12f-106">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="8c12f-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="8c12f-107">Membros</span><span class="sxs-lookup"><span data-stu-id="8c12f-107">Members</span></span>
|<span data-ttu-id="8c12f-108">Membro</span><span class="sxs-lookup"><span data-stu-id="8c12f-108">Member</span></span>|<span data-ttu-id="8c12f-109">Valor</span><span class="sxs-lookup"><span data-stu-id="8c12f-109">Value</span></span>|<span data-ttu-id="8c12f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8c12f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c12f-111">nenhuma</span><span class="sxs-lookup"><span data-stu-id="8c12f-111">none</span></span>|<span data-ttu-id="8c12f-112">,0</span><span class="sxs-lookup"><span data-stu-id="8c12f-112">0</span></span>|<span data-ttu-id="8c12f-113">Nenhum status detalhado de atribuição</span><span class="sxs-lookup"><span data-stu-id="8c12f-113">No assignment detailed status</span></span>|
|<span data-ttu-id="8c12f-114">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="8c12f-114">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="8c12f-115">1</span><span class="sxs-lookup"><span data-stu-id="8c12f-115">1</span></span>|<span data-ttu-id="8c12f-116">Os requisitos de hardware não são atendidos.</span><span class="sxs-lookup"><span data-stu-id="8c12f-116">Hardware requirements are not met.</span></span> <span data-ttu-id="8c12f-117">Isso pode acontecer se um perfil autoimplantar do autoautoria for atribuído a um dispositivo sem o TPM 2,0.</span><span class="sxs-lookup"><span data-stu-id="8c12f-117">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="8c12f-118">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="8c12f-118">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="8c12f-119">duas</span><span class="sxs-lookup"><span data-stu-id="8c12f-119">2</span></span>|<span data-ttu-id="8c12f-120">Isso pode acontecer quando um perfil do AutoPilot do SurfaceHub é atribuído a um dispositivo que não é SurfaceHub.</span><span class="sxs-lookup"><span data-stu-id="8c12f-120">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="8c12f-121">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="8c12f-121">holoLensProfileNotSupported</span></span>|<span data-ttu-id="8c12f-122">3D</span><span class="sxs-lookup"><span data-stu-id="8c12f-122">3</span></span>|<span data-ttu-id="8c12f-123">Isso pode acontecer quando um perfil do AutoPilot do HoloLens é atribuído a um dispositivo que não é HoloLens.</span><span class="sxs-lookup"><span data-stu-id="8c12f-123">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="8c12f-124">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="8c12f-124">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="8c12f-125">quatro</span><span class="sxs-lookup"><span data-stu-id="8c12f-125">4</span></span>|<span data-ttu-id="8c12f-126">Isso pode acontecer quando um perfil do AutoPilot do WindowsPc é atribuído a um dispositivo que não é WindowsPc.</span><span class="sxs-lookup"><span data-stu-id="8c12f-126">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|



