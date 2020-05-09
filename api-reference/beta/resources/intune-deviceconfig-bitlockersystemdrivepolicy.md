---
title: tipo de recurso bitLockerSystemDrivePolicy
description: Políticas de base de criptografia BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 40eeaa88f2e31901f39edc7b52b1a9358db70396
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/09/2020
ms.locfileid: "44179303"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="a6870-103">tipo de recurso bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="a6870-103">bitLockerSystemDrivePolicy resource type</span></span>

<span data-ttu-id="a6870-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6870-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6870-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a6870-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a6870-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6870-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6870-107">Políticas de base de criptografia BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a6870-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="a6870-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a6870-108">Properties</span></span>
|<span data-ttu-id="a6870-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6870-109">Property</span></span>|<span data-ttu-id="a6870-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6870-110">Type</span></span>|<span data-ttu-id="a6870-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6870-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6870-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a6870-112">encryptionMethod</span></span>|[<span data-ttu-id="a6870-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="a6870-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="a6870-114">Selecione o método de criptografia para unidades do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="a6870-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="a6870-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="a6870-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="a6870-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="a6870-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="a6870-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6870-117">Boolean</span></span>|<span data-ttu-id="a6870-118">Exigir autenticação adicional na inicialização.</span><span class="sxs-lookup"><span data-stu-id="a6870-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="a6870-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="a6870-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="a6870-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6870-120">Boolean</span></span>|<span data-ttu-id="a6870-121">Indica se é permitido o BitLocker sem um TPM compatível (requer uma senha ou uma chave de inicialização em uma unidade flash USB).</span><span class="sxs-lookup"><span data-stu-id="a6870-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="a6870-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="a6870-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a6870-124">Indica se a inicialização do TPM é permitida/obrigatória/não permitida.</span><span class="sxs-lookup"><span data-stu-id="a6870-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="a6870-125">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a6870-125">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="a6870-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="a6870-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a6870-128">Indica se o PIN de inicialização do TPM é permitido/obrigatório/não permitido.</span><span class="sxs-lookup"><span data-stu-id="a6870-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="a6870-129">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a6870-129">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="a6870-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="a6870-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a6870-132">Indica se a chave de inicialização do TPM é permitida/obrigatória/não permitida.</span><span class="sxs-lookup"><span data-stu-id="a6870-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="a6870-133">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a6870-133">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="a6870-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="a6870-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="a6870-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="a6870-136">Indica se a chave do PIN de inicialização do TPM e a chave são permitidas/obrigatórias/não permitidas.</span><span class="sxs-lookup"><span data-stu-id="a6870-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="a6870-137">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="a6870-137">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="a6870-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="a6870-138">minimumPinLength</span></span>|<span data-ttu-id="a6870-139">Int32</span><span class="sxs-lookup"><span data-stu-id="a6870-139">Int32</span></span>|<span data-ttu-id="a6870-140">Indica o comprimento mínimo do PIN de inicialização.</span><span class="sxs-lookup"><span data-stu-id="a6870-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="a6870-141">Valores válidos de 4 a 20</span><span class="sxs-lookup"><span data-stu-id="a6870-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="a6870-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a6870-142">recoveryOptions</span></span>|[<span data-ttu-id="a6870-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="a6870-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="a6870-144">Permite recuperar as unidades do sistema operacional criptografadas do BitLocker na ausência das informações de chave de inicialização necessárias.</span><span class="sxs-lookup"><span data-stu-id="a6870-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="a6870-145">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="a6870-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="a6870-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="a6870-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="a6870-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6870-147">Boolean</span></span>|<span data-ttu-id="a6870-148">Habilitar mensagem e URL de recuperação de pré-inicialização.</span><span class="sxs-lookup"><span data-stu-id="a6870-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="a6870-149">Se requireStartupAuthentication for false, esse valor não será afetado.</span><span class="sxs-lookup"><span data-stu-id="a6870-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="a6870-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="a6870-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="a6870-151">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a6870-151">String</span></span>|<span data-ttu-id="a6870-152">Define uma mensagem de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="a6870-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="a6870-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="a6870-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="a6870-154">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="a6870-154">String</span></span>|<span data-ttu-id="a6870-155">Define uma URL de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="a6870-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6870-156">Relações</span><span class="sxs-lookup"><span data-stu-id="a6870-156">Relationships</span></span>
<span data-ttu-id="a6870-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a6870-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a6870-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a6870-158">JSON Representation</span></span>
<span data-ttu-id="a6870-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a6870-159">Here is a JSON representation of the resource.</span></span>
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



