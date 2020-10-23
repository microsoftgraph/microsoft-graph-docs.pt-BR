---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f18a4eb3dd7d31c51dc21a02999aa4ea99d2f0fd
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48723874"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="6ef7c-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="6ef7c-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="6ef7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ef7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ef7c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6ef7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ef7c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6ef7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ef7c-107">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="6ef7c-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="6ef7c-108">Membros</span><span class="sxs-lookup"><span data-stu-id="6ef7c-108">Members</span></span>
|<span data-ttu-id="6ef7c-109">Membro</span><span class="sxs-lookup"><span data-stu-id="6ef7c-109">Member</span></span>|<span data-ttu-id="6ef7c-110">Valor</span><span class="sxs-lookup"><span data-stu-id="6ef7c-110">Value</span></span>|<span data-ttu-id="6ef7c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ef7c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ef7c-112">none</span><span class="sxs-lookup"><span data-stu-id="6ef7c-112">none</span></span>|<span data-ttu-id="6ef7c-113">,0</span><span class="sxs-lookup"><span data-stu-id="6ef7c-113">0</span></span>|<span data-ttu-id="6ef7c-114">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="6ef7c-114">no requirement set</span></span>|
|<span data-ttu-id="6ef7c-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="6ef7c-115">basicIntegrity</span></span>|<span data-ttu-id="6ef7c-116">1</span><span class="sxs-lookup"><span data-stu-id="6ef7c-116">1</span></span>|<span data-ttu-id="6ef7c-117">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="6ef7c-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="6ef7c-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="6ef7c-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="6ef7c-119">duas</span><span class="sxs-lookup"><span data-stu-id="6ef7c-119">2</span></span>|<span data-ttu-id="6ef7c-120">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="6ef7c-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





