---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 93d65431cfcdfc952231237f2646eee79e331ef3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42782696"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="e741b-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="e741b-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="e741b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e741b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e741b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e741b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e741b-106">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e741b-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="e741b-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e741b-107">Members</span></span>
|<span data-ttu-id="e741b-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e741b-108">Member</span></span>|<span data-ttu-id="e741b-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e741b-109">Value</span></span>|<span data-ttu-id="e741b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e741b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e741b-111">none</span><span class="sxs-lookup"><span data-stu-id="e741b-111">none</span></span>|<span data-ttu-id="e741b-112">,0</span><span class="sxs-lookup"><span data-stu-id="e741b-112">0</span></span>|<span data-ttu-id="e741b-113">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="e741b-113">no requirement set</span></span>|
|<span data-ttu-id="e741b-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="e741b-114">basicIntegrity</span></span>|<span data-ttu-id="e741b-115">1</span><span class="sxs-lookup"><span data-stu-id="e741b-115">1</span></span>|<span data-ttu-id="e741b-116">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="e741b-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="e741b-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="e741b-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="e741b-118">duas</span><span class="sxs-lookup"><span data-stu-id="e741b-118">2</span></span>|<span data-ttu-id="e741b-119">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e741b-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



