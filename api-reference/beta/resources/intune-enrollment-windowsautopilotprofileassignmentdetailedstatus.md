---
title: tipo de enumeração windowsAutopilotProfileAssignmentDetailedStatus
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7902904e20dd16f6c6b8adebe633934814ca8ca1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256124"
---
# <a name="windowsautopilotprofileassignmentdetailedstatus-enum-type"></a><span data-ttu-id="badd2-103">tipo de enumeração windowsAutopilotProfileAssignmentDetailedStatus</span><span class="sxs-lookup"><span data-stu-id="badd2-103">windowsAutopilotProfileAssignmentDetailedStatus enum type</span></span>

<span data-ttu-id="badd2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="badd2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="badd2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="badd2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="badd2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="badd2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="badd2-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="badd2-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="badd2-108">Membros</span><span class="sxs-lookup"><span data-stu-id="badd2-108">Members</span></span>
|<span data-ttu-id="badd2-109">Membro</span><span class="sxs-lookup"><span data-stu-id="badd2-109">Member</span></span>|<span data-ttu-id="badd2-110">Valor</span><span class="sxs-lookup"><span data-stu-id="badd2-110">Value</span></span>|<span data-ttu-id="badd2-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="badd2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="badd2-112">nenhum</span><span class="sxs-lookup"><span data-stu-id="badd2-112">none</span></span>|<span data-ttu-id="badd2-113">,0</span><span class="sxs-lookup"><span data-stu-id="badd2-113">0</span></span>|<span data-ttu-id="badd2-114">Nenhum status detalhado de atribuição</span><span class="sxs-lookup"><span data-stu-id="badd2-114">No assignment detailed status</span></span>|
|<span data-ttu-id="badd2-115">hardwareRequirementsNotMet</span><span class="sxs-lookup"><span data-stu-id="badd2-115">hardwareRequirementsNotMet</span></span>|<span data-ttu-id="badd2-116">1</span><span class="sxs-lookup"><span data-stu-id="badd2-116">1</span></span>|<span data-ttu-id="badd2-117">Os requisitos de hardware não são atendidos.</span><span class="sxs-lookup"><span data-stu-id="badd2-117">Hardware requirements are not met.</span></span> <span data-ttu-id="badd2-118">Isso pode acontecer se um perfil autoimplantar do autoautoria for atribuído a um dispositivo sem o TPM 2,0.</span><span class="sxs-lookup"><span data-stu-id="badd2-118">This can happen if a self-deploying AutoPilot Profile is assigned to a device without TPM 2.0.</span></span>|
|<span data-ttu-id="badd2-119">surfaceHubProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="badd2-119">surfaceHubProfileNotSupported</span></span>|<span data-ttu-id="badd2-120">duas</span><span class="sxs-lookup"><span data-stu-id="badd2-120">2</span></span>|<span data-ttu-id="badd2-121">Isso pode acontecer quando um perfil do AutoPilot do SurfaceHub é atribuído a um dispositivo que não é SurfaceHub.</span><span class="sxs-lookup"><span data-stu-id="badd2-121">This can happen if a SurfaceHub AutoPilot Profile is assigned to a device that is not SurfaceHub.</span></span>|
|<span data-ttu-id="badd2-122">holoLensProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="badd2-122">holoLensProfileNotSupported</span></span>|<span data-ttu-id="badd2-123">3D</span><span class="sxs-lookup"><span data-stu-id="badd2-123">3</span></span>|<span data-ttu-id="badd2-124">Isso pode acontecer quando um perfil do AutoPilot do HoloLens é atribuído a um dispositivo que não é HoloLens.</span><span class="sxs-lookup"><span data-stu-id="badd2-124">This can happen if a HoloLens AutoPilot Profile is assigned to a device that is not HoloLens.</span></span>|
|<span data-ttu-id="badd2-125">windowsPcProfileNotSupported</span><span class="sxs-lookup"><span data-stu-id="badd2-125">windowsPcProfileNotSupported</span></span>|<span data-ttu-id="badd2-126">4 </span><span class="sxs-lookup"><span data-stu-id="badd2-126">4</span></span>|<span data-ttu-id="badd2-127">Isso pode acontecer quando um perfil do AutoPilot do WindowsPc é atribuído a um dispositivo que não é WindowsPc.</span><span class="sxs-lookup"><span data-stu-id="badd2-127">This can happen if a WindowsPc AutoPilot Profile is assigned to a device that is not WindowsPc.</span></span>|




