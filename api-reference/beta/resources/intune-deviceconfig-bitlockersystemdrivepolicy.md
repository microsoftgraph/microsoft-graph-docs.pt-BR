---
title: tipo de recurso bitLockerSystemDrivePolicy
description: Políticas de base de criptografia BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bca77059f2ec819f62326469454f373b3916b7f7
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34990180"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="32cd2-103">tipo de recurso bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="32cd2-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="32cd2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="32cd2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="32cd2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="32cd2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="32cd2-106">Políticas de base de criptografia BitLocker.</span><span class="sxs-lookup"><span data-stu-id="32cd2-106">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="32cd2-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="32cd2-107">Properties</span></span>
|<span data-ttu-id="32cd2-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="32cd2-108">Property</span></span>|<span data-ttu-id="32cd2-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="32cd2-109">Type</span></span>|<span data-ttu-id="32cd2-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="32cd2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="32cd2-111">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="32cd2-111">encryptionMethod</span></span>|[<span data-ttu-id="32cd2-112">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="32cd2-112">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="32cd2-113">Selecione o método de criptografia para unidades do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="32cd2-113">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="32cd2-114">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="32cd2-114">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="32cd2-115">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="32cd2-115">startupAuthenticationRequired</span></span>|<span data-ttu-id="32cd2-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="32cd2-116">Boolean</span></span>|<span data-ttu-id="32cd2-117">Exigir autenticação adicional na inicialização.</span><span class="sxs-lookup"><span data-stu-id="32cd2-117">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="32cd2-118">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="32cd2-118">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="32cd2-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="32cd2-119">Boolean</span></span>|<span data-ttu-id="32cd2-120">Indica se é permitido o BitLocker sem um TPM compatível (requer uma senha ou uma chave de inicialização em uma unidade flash USB).</span><span class="sxs-lookup"><span data-stu-id="32cd2-120">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="32cd2-121">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-121">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="32cd2-122">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-122">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="32cd2-123">Indica se a inicialização do TPM é permitida/obrigatória/não permitida.</span><span class="sxs-lookup"><span data-stu-id="32cd2-123">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="32cd2-124">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="32cd2-124">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="32cd2-125">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-125">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="32cd2-126">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-126">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="32cd2-127">Indica se o PIN de inicialização do TPM é permitido/obrigatório/não permitido.</span><span class="sxs-lookup"><span data-stu-id="32cd2-127">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="32cd2-128">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="32cd2-128">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="32cd2-129">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-129">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="32cd2-130">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-130">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="32cd2-131">Indica se a chave de inicialização do TPM é permitida/obrigatória/não permitida.</span><span class="sxs-lookup"><span data-stu-id="32cd2-131">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="32cd2-132">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="32cd2-132">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="32cd2-133">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-133">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="32cd2-134">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="32cd2-134">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="32cd2-135">Indica se a chave do PIN de inicialização do TPM e a chave são permitidas/obrigatórias/não permitidas.</span><span class="sxs-lookup"><span data-stu-id="32cd2-135">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="32cd2-136">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="32cd2-136">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="32cd2-137">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="32cd2-137">minimumPinLength</span></span>|<span data-ttu-id="32cd2-138">Int32</span><span class="sxs-lookup"><span data-stu-id="32cd2-138">Int32</span></span>|<span data-ttu-id="32cd2-139">Indica o comprimento mínimo do PIN de inicialização.</span><span class="sxs-lookup"><span data-stu-id="32cd2-139">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="32cd2-140">Valores válidos de 4 a 20</span><span class="sxs-lookup"><span data-stu-id="32cd2-140">Valid values 4 to 20</span></span>|
|<span data-ttu-id="32cd2-141">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="32cd2-141">recoveryOptions</span></span>|[<span data-ttu-id="32cd2-142">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="32cd2-142">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="32cd2-143">Permite recuperar as unidades do sistema operacional criptografadas do BitLocker na ausência das informações de chave de inicialização necessárias.</span><span class="sxs-lookup"><span data-stu-id="32cd2-143">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="32cd2-144">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="32cd2-144">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="32cd2-145">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="32cd2-145">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="32cd2-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="32cd2-146">Boolean</span></span>|<span data-ttu-id="32cd2-147">Habilitar mensagem e URL de recuperação de pré-inicialização.</span><span class="sxs-lookup"><span data-stu-id="32cd2-147">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="32cd2-148">Se requireStartupAuthentication for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="32cd2-148">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="32cd2-149">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="32cd2-149">prebootRecoveryMessage</span></span>|<span data-ttu-id="32cd2-150">String</span><span class="sxs-lookup"><span data-stu-id="32cd2-150">String</span></span>|<span data-ttu-id="32cd2-151">Define uma mensagem de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="32cd2-151">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="32cd2-152">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="32cd2-152">prebootRecoveryUrl</span></span>|<span data-ttu-id="32cd2-153">String</span><span class="sxs-lookup"><span data-stu-id="32cd2-153">String</span></span>|<span data-ttu-id="32cd2-154">Define uma URL de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="32cd2-154">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="32cd2-155">Relações</span><span class="sxs-lookup"><span data-stu-id="32cd2-155">Relationships</span></span>
<span data-ttu-id="32cd2-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="32cd2-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="32cd2-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="32cd2-157">JSON Representation</span></span>
<span data-ttu-id="32cd2-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="32cd2-158">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerSystemDrivePolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerSystemDrivePolicy",
  "encryptionMethod": "String",
  "startupAuthenticationRequired": true,
  "startupAuthenticationBlockWithoutTpmChip": true,
  "startupAuthenticationTpmUsage": "String",
  "startupAuthenticationTpmPinUsage": "String",
  "startupAuthenticationTpmKeyUsage": "String",
  "startupAuthenticationTpmPinAndKeyUsage": "String",
  "minimumPinLength": 1024,
  "recoveryOptions": {
    "@odata.type": "microsoft.graph.bitLockerRecoveryOptions",
    "blockDataRecoveryAgent": true,
    "recoveryPasswordUsage": "String",
    "recoveryKeyUsage": "String",
    "hideRecoveryOptions": true,
    "enableRecoveryInformationSaveToStore": true,
    "recoveryInformationToStore": "String",
    "enableBitLockerAfterRecoveryInformationToStore": true
  },
  "prebootRecoveryEnableMessageAndUrl": true,
  "prebootRecoveryMessage": "String",
  "prebootRecoveryUrl": "String"
}
```





