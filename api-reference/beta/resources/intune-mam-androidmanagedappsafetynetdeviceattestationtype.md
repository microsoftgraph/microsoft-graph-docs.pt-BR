---
title: tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType
description: Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6a75a8fda81c4169051c8b12fae9c1f7ece07795
ms.sourcegitcommit: 8eb88cfb48b0eb8f992570caebef577dfa2f30d3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/14/2019
ms.locfileid: "30631428"
---
# <a name="androidmanagedappsafetynetdeviceattestationtype-enum-type"></a><span data-ttu-id="c4d9e-103">tipo de enumeração androidManagedAppSafetyNetDeviceAttestationType</span><span class="sxs-lookup"><span data-stu-id="c4d9e-103">androidManagedAppSafetyNetDeviceAttestationType enum type</span></span>

> <span data-ttu-id="c4d9e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c4d9e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c4d9e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c4d9e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c4d9e-106">Um requisito de atestado de dispositivo do SafetyNet do Android aplicado por administradores em um aplicativo gerenciado.</span><span class="sxs-lookup"><span data-stu-id="c4d9e-106">An admin enforced Android SafetyNet Device Attestation requirement on a managed app.</span></span>

## <a name="members"></a><span data-ttu-id="c4d9e-107">Membros</span><span class="sxs-lookup"><span data-stu-id="c4d9e-107">Members</span></span>
|<span data-ttu-id="c4d9e-108">Membro</span><span class="sxs-lookup"><span data-stu-id="c4d9e-108">Member</span></span>|<span data-ttu-id="c4d9e-109">Valor</span><span class="sxs-lookup"><span data-stu-id="c4d9e-109">Value</span></span>|<span data-ttu-id="c4d9e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c4d9e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c4d9e-111">nenhum</span><span class="sxs-lookup"><span data-stu-id="c4d9e-111">none</span></span>|<span data-ttu-id="c4d9e-112">,0</span><span class="sxs-lookup"><span data-stu-id="c4d9e-112">0</span></span>|<span data-ttu-id="c4d9e-113">nenhum conjunto de requisitos</span><span class="sxs-lookup"><span data-stu-id="c4d9e-113">no requirement set</span></span>|
|<span data-ttu-id="c4d9e-114">basicIntegrity</span><span class="sxs-lookup"><span data-stu-id="c4d9e-114">basicIntegrity</span></span>|<span data-ttu-id="c4d9e-115">1</span><span class="sxs-lookup"><span data-stu-id="c4d9e-115">1</span></span>|<span data-ttu-id="c4d9e-116">exigir que o dispositivo Android passe na validação da integridade básica do SafetyNet</span><span class="sxs-lookup"><span data-stu-id="c4d9e-116">require that Android device passes SafetyNet Basic Integrity validation</span></span>|
|<span data-ttu-id="c4d9e-117">basicIntegrityAndDeviceCertification</span><span class="sxs-lookup"><span data-stu-id="c4d9e-117">basicIntegrityAndDeviceCertification</span></span>|<span data-ttu-id="c4d9e-118">duas</span><span class="sxs-lookup"><span data-stu-id="c4d9e-118">2</span></span>|<span data-ttu-id="c4d9e-119">exigir que o dispositivo Android passe a integridade básica do SafetyNet e as validações de certificação de dispositivos</span><span class="sxs-lookup"><span data-stu-id="c4d9e-119">require that Android device passes SafetyNet Basic Integrity and Device Certification validations</span></span>|




