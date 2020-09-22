---
title: tipo de recurso bitLockerSystemDrivePolicy
description: Políticas de base de criptografia BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a2ef33abdcb8cc5c27fe1e0cd6146f0f736202aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48040018"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="da257-103">tipo de recurso bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="da257-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="da257-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da257-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da257-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="da257-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da257-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="da257-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da257-107">Políticas de base de criptografia BitLocker.</span><span class="sxs-lookup"><span data-stu-id="da257-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="da257-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="da257-108">Properties</span></span>
|<span data-ttu-id="da257-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="da257-109">Property</span></span>|<span data-ttu-id="da257-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="da257-110">Type</span></span>|<span data-ttu-id="da257-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="da257-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da257-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="da257-112">encryptionMethod</span></span>|[<span data-ttu-id="da257-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="da257-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="da257-114">Selecione o método de criptografia para unidades do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="da257-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="da257-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="da257-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="da257-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="da257-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="da257-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="da257-117">Boolean</span></span>|<span data-ttu-id="da257-118">Exigir autenticação adicional na inicialização.</span><span class="sxs-lookup"><span data-stu-id="da257-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="da257-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="da257-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="da257-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="da257-120">Boolean</span></span>|<span data-ttu-id="da257-121">Indica se é permitido o BitLocker sem um TPM compatível (requer uma senha ou uma chave de inicialização em uma unidade flash USB).</span><span class="sxs-lookup"><span data-stu-id="da257-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="da257-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="da257-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="da257-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da257-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da257-124">Indica se a inicialização do TPM é permitida/obrigatória/não permitida.</span><span class="sxs-lookup"><span data-stu-id="da257-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="da257-125">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da257-125">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da257-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="da257-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="da257-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da257-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da257-128">Indica se o PIN de inicialização do TPM é permitido/obrigatório/não permitido.</span><span class="sxs-lookup"><span data-stu-id="da257-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="da257-129">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da257-129">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da257-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="da257-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="da257-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da257-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da257-132">Indica se a chave de inicialização do TPM é permitida/obrigatória/não permitida.</span><span class="sxs-lookup"><span data-stu-id="da257-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="da257-133">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da257-133">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da257-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="da257-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="da257-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="da257-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="da257-136">Indica se a chave do PIN de inicialização do TPM e a chave são permitidas/obrigatórias/não permitidas.</span><span class="sxs-lookup"><span data-stu-id="da257-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="da257-137">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="da257-137">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="da257-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="da257-138">minimumPinLength</span></span>|<span data-ttu-id="da257-139">Int32</span><span class="sxs-lookup"><span data-stu-id="da257-139">Int32</span></span>|<span data-ttu-id="da257-140">Indica o comprimento mínimo do PIN de inicialização.</span><span class="sxs-lookup"><span data-stu-id="da257-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="da257-141">Valores válidos de 4 a 20</span><span class="sxs-lookup"><span data-stu-id="da257-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="da257-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="da257-142">recoveryOptions</span></span>|[<span data-ttu-id="da257-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="da257-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="da257-144">Permite recuperar as unidades do sistema operacional criptografadas do BitLocker na ausência das informações de chave de inicialização necessárias.</span><span class="sxs-lookup"><span data-stu-id="da257-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="da257-145">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="da257-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="da257-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="da257-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="da257-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="da257-147">Boolean</span></span>|<span data-ttu-id="da257-148">Habilitar mensagem e URL de recuperação de pré-inicialização.</span><span class="sxs-lookup"><span data-stu-id="da257-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="da257-149">Se requireStartupAuthentication for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="da257-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="da257-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="da257-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="da257-151">String</span><span class="sxs-lookup"><span data-stu-id="da257-151">String</span></span>|<span data-ttu-id="da257-152">Define uma mensagem de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="da257-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="da257-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="da257-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="da257-154">String</span><span class="sxs-lookup"><span data-stu-id="da257-154">String</span></span>|<span data-ttu-id="da257-155">Define uma URL de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="da257-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="da257-156">Relações</span><span class="sxs-lookup"><span data-stu-id="da257-156">Relationships</span></span>
<span data-ttu-id="da257-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="da257-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="da257-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="da257-158">JSON Representation</span></span>
<span data-ttu-id="da257-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="da257-159">Here is a JSON representation of the resource.</span></span>
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






