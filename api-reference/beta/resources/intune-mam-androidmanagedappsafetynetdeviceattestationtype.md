---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cef86d779a866174749a0916ab606f64374bfa1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563998"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="c94fe-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="c94fe-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="c94fe-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c94fe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c94fe-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c94fe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c94fe-106">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c94fe-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="c94fe-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c94fe-107">Members</span></span>
|<span data-ttu-id="c94fe-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c94fe-108">Member</span></span>|<span data-ttu-id="c94fe-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c94fe-109">Value</span></span>|<span data-ttu-id="c94fe-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c94fe-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c94fe-111">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="c94fe-111">none</span></span>|<span data-ttu-id="c94fe-112">,0</span><span class="sxs-lookup"><span data-stu-id="c94fe-112">0</span></span>|<span data-ttu-id="c94fe-113">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="c94fe-113">no requirement set</span></span>|
|<span data-ttu-id="c94fe-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c94fe-114">basicIntegrity</span></span>|<span data-ttu-id="c94fe-115">1 </span><span class="sxs-lookup"><span data-stu-id="c94fe-115">1</span></span>|<span data-ttu-id="c94fe-116">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="c94fe-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="c94fe-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="c94fe-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="c94fe-118">2 </span><span class="sxs-lookup"><span data-stu-id="c94fe-118">2</span></span>|<span data-ttu-id="c94fe-119">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c94fe-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





