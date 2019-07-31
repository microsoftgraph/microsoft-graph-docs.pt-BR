---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 03c7496fe5e3d1fce5f73cc0f5954d8415668641
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968075"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="e53f3-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="e53f3-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="e53f3-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e53f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e53f3-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e53f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e53f3-106">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="e53f3-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="e53f3-107">Membros</span><span class="sxs-lookup"><span data-stu-id="e53f3-107">Members</span></span>
|<span data-ttu-id="e53f3-108">Membro</span><span class="sxs-lookup"><span data-stu-id="e53f3-108">Member</span></span>|<span data-ttu-id="e53f3-109">Valor</span><span class="sxs-lookup"><span data-stu-id="e53f3-109">Value</span></span>|<span data-ttu-id="e53f3-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e53f3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e53f3-111">none</span><span class="sxs-lookup"><span data-stu-id="e53f3-111">none</span></span>|<span data-ttu-id="e53f3-112">,0</span><span class="sxs-lookup"><span data-stu-id="e53f3-112">0</span></span>|<span data-ttu-id="e53f3-113">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="e53f3-113">no requirement set</span></span>|
|<span data-ttu-id="e53f3-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="e53f3-114">basicIntegrity</span></span>|<span data-ttu-id="e53f3-115">1</span><span class="sxs-lookup"><span data-stu-id="e53f3-115">1</span></span>|<span data-ttu-id="e53f3-116">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="e53f3-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="e53f3-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="e53f3-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="e53f3-118">duas</span><span class="sxs-lookup"><span data-stu-id="e53f3-118">2</span></span>|<span data-ttu-id="e53f3-119">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="e53f3-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|





