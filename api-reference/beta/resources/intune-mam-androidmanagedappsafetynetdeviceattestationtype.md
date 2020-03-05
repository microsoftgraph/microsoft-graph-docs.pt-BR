---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 285389d07f4ea6f667a0e12260fe5a5296808923
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524361"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="756c0-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="756c0-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

<span data-ttu-id="756c0-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="756c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="756c0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="756c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="756c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="756c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="756c0-107">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="756c0-107">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="756c0-108">Membros</span><span class="sxs-lookup"><span data-stu-id="756c0-108">Members</span></span>
|<span data-ttu-id="756c0-109">Membro</span><span class="sxs-lookup"><span data-stu-id="756c0-109">Member</span></span>|<span data-ttu-id="756c0-110">Valor</span><span class="sxs-lookup"><span data-stu-id="756c0-110">Value</span></span>|<span data-ttu-id="756c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="756c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="756c0-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="756c0-112">none</span></span>|<span data-ttu-id="756c0-113">,0</span><span class="sxs-lookup"><span data-stu-id="756c0-113">0</span></span>|<span data-ttu-id="756c0-114">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="756c0-114">no requirement set</span></span>|
|<span data-ttu-id="756c0-115">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="756c0-115">basicIntegrity</span></span>|<span data-ttu-id="756c0-116">1 </span><span class="sxs-lookup"><span data-stu-id="756c0-116">1</span></span>|<span data-ttu-id="756c0-117">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="756c0-117">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="756c0-118">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="756c0-118">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="756c0-119">2 </span><span class="sxs-lookup"><span data-stu-id="756c0-119">2</span></span>|<span data-ttu-id="756c0-120">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="756c0-120">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|



