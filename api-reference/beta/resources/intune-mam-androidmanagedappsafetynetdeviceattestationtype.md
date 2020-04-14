---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0ef06b8f3cc3a2e53a053f0169e5921bc02fb822
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43374351"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="73c5c-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="73c5c-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="73c5c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73c5c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="73c5c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="73c5c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73c5c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="73c5c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73c5c-107">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="73c5c-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="73c5c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="73c5c-108">Members</span></span>
|<span data-ttu-id="73c5c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="73c5c-109">Member</span></span>|<span data-ttu-id="73c5c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="73c5c-110">Value</span></span>|<span data-ttu-id="73c5c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="73c5c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73c5c-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="73c5c-112">none</span></span>|<span data-ttu-id="73c5c-113">,0</span><span class="sxs-lookup"><span data-stu-id="73c5c-113">0</span></span>|<span data-ttu-id="73c5c-114">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="73c5c-114">no requirement set</span></span>|
|<span data-ttu-id="73c5c-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="73c5c-115">basicIntegrity</span></span>|<span data-ttu-id="73c5c-116">1</span><span class="sxs-lookup"><span data-stu-id="73c5c-116">1</span></span>|<span data-ttu-id="73c5c-117">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="73c5c-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="73c5c-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="73c5c-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="73c5c-119">duas</span><span class="sxs-lookup"><span data-stu-id="73c5c-119">2</span></span>|<span data-ttu-id="73c5c-120">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="73c5c-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



