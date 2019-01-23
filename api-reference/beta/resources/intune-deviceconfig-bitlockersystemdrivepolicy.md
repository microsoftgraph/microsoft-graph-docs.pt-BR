---
title: tipo de recurso de bitLockerSystemDrivePolicy
description: Políticas de Base de criptografia BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9b63d075538508941d012df1e44f7cb563fed20d
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425705"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="87b5e-103">tipo de recurso de bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="87b5e-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="87b5e-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="87b5e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87b5e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="87b5e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87b5e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="87b5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87b5e-107">Políticas de Base de criptografia BitLocker.</span><span class="sxs-lookup"><span data-stu-id="87b5e-107">BitLocker Encryption Base Policies.</span></span>

## <a name="properties"></a><span data-ttu-id="87b5e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="87b5e-108">Properties</span></span>
|<span data-ttu-id="87b5e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87b5e-109">Property</span></span>|<span data-ttu-id="87b5e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="87b5e-110">Type</span></span>|<span data-ttu-id="87b5e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="87b5e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87b5e-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="87b5e-112">encryptionMethod</span></span>|[<span data-ttu-id="87b5e-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="87b5e-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="87b5e-114">Selecione o método de criptografia para unidades do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="87b5e-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="87b5e-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="87b5e-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="87b5e-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="87b5e-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="87b5e-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="87b5e-117">Boolean</span></span>|<span data-ttu-id="87b5e-118">Exigem autenticação adicional na inicialização.</span><span class="sxs-lookup"><span data-stu-id="87b5e-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="87b5e-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="87b5e-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="87b5e-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="87b5e-120">Boolean</span></span>|<span data-ttu-id="87b5e-121">Indica se você deseja permitir BitLocker sem um TPM compatível (exige uma senha ou uma chave de inicialização em uma unidade flash USB).</span><span class="sxs-lookup"><span data-stu-id="87b5e-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="87b5e-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="87b5e-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="87b5e-124">Indica se a inicialização do TPM é permitido/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="87b5e-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="87b5e-125">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="87b5e-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="87b5e-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="87b5e-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="87b5e-128">Indica se o pin de inicialização TPM é permitido/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="87b5e-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="87b5e-129">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="87b5e-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="87b5e-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="87b5e-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="87b5e-132">Indica se a chave de inicialização do TPM será permitido/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="87b5e-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="87b5e-133">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="87b5e-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="87b5e-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="87b5e-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="87b5e-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="87b5e-136">Indica se a inicialização do TPM fixar chave e chave são permitidos/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="87b5e-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="87b5e-137">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="87b5e-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="87b5e-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="87b5e-138">minimumPinLength</span></span>|<span data-ttu-id="87b5e-139">Int32</span><span class="sxs-lookup"><span data-stu-id="87b5e-139">Int32</span></span>|<span data-ttu-id="87b5e-140">Indica o tamanho mínimo do pin de inicialização.</span><span class="sxs-lookup"><span data-stu-id="87b5e-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="87b5e-141">Valores válidos 4 a 20</span><span class="sxs-lookup"><span data-stu-id="87b5e-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="87b5e-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="87b5e-142">recoveryOptions</span></span>|[<span data-ttu-id="87b5e-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="87b5e-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="87b5e-144">Permite recuperar BitLocker criptografado unidades do sistema operacional na ausência das informações de chave de inicialização necessários.</span><span class="sxs-lookup"><span data-stu-id="87b5e-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="87b5e-145">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="87b5e-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="87b5e-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="87b5e-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="87b5e-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="87b5e-147">Boolean</span></span>|<span data-ttu-id="87b5e-148">Habilite a mensagem de recuperação antes da inicialização e a Url.</span><span class="sxs-lookup"><span data-stu-id="87b5e-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="87b5e-149">Se requireStartupAuthentication for false, esse valor não afeta.</span><span class="sxs-lookup"><span data-stu-id="87b5e-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="87b5e-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="87b5e-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="87b5e-151">String</span><span class="sxs-lookup"><span data-stu-id="87b5e-151">String</span></span>|<span data-ttu-id="87b5e-152">Define uma mensagem de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="87b5e-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="87b5e-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="87b5e-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="87b5e-154">String</span><span class="sxs-lookup"><span data-stu-id="87b5e-154">String</span></span>|<span data-ttu-id="87b5e-155">Define uma URL personalizada de recuperação.</span><span class="sxs-lookup"><span data-stu-id="87b5e-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="87b5e-156">Relações</span><span class="sxs-lookup"><span data-stu-id="87b5e-156">Relationships</span></span>
<span data-ttu-id="87b5e-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="87b5e-157">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="87b5e-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="87b5e-158">JSON Representation</span></span>
<span data-ttu-id="87b5e-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="87b5e-159">Here is a JSON representation of the resource.</span></span>
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




