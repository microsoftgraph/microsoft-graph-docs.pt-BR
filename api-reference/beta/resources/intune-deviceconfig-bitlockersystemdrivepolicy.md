---
title: tipo de recurso de bitLockerSystemDrivePolicy
description: Políticas de Base de criptografia BitLocker.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 28c3b597f25e7ea83577c18620280885f4149dcf
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924654"
---
# <a name="bitlockersystemdrivepolicy-resource-type"></a><span data-ttu-id="572a6-103">tipo de recurso de bitLockerSystemDrivePolicy</span><span class="sxs-lookup"><span data-stu-id="572a6-103">bitLockerSystemDrivePolicy resource type</span></span>

> <span data-ttu-id="572a6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="572a6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="572a6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="572a6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="572a6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="572a6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="572a6-107">Políticas de Base de criptografia BitLocker.</span><span class="sxs-lookup"><span data-stu-id="572a6-107">BitLocker Encryption Base Policies.</span></span>
## <a name="properties"></a><span data-ttu-id="572a6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="572a6-108">Properties</span></span>
|<span data-ttu-id="572a6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="572a6-109">Property</span></span>|<span data-ttu-id="572a6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="572a6-110">Type</span></span>|<span data-ttu-id="572a6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="572a6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="572a6-112">encryptionMethod</span><span class="sxs-lookup"><span data-stu-id="572a6-112">encryptionMethod</span></span>|[<span data-ttu-id="572a6-113">bitLockerEncryptionMethod</span><span class="sxs-lookup"><span data-stu-id="572a6-113">bitLockerEncryptionMethod</span></span>](../resources/intune-deviceconfig-bitlockerencryptionmethod.md)|<span data-ttu-id="572a6-114">Selecione o método de criptografia para unidades do sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="572a6-114">Select the encryption method for operating system drives.</span></span> <span data-ttu-id="572a6-115">Os valores possíveis são: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span><span class="sxs-lookup"><span data-stu-id="572a6-115">Possible values are: `aesCbc128`, `aesCbc256`, `xtsAes128`, `xtsAes256`.</span></span>|
|<span data-ttu-id="572a6-116">startupAuthenticationRequired</span><span class="sxs-lookup"><span data-stu-id="572a6-116">startupAuthenticationRequired</span></span>|<span data-ttu-id="572a6-117">Booliano</span><span class="sxs-lookup"><span data-stu-id="572a6-117">Boolean</span></span>|<span data-ttu-id="572a6-118">Exigem autenticação adicional na inicialização.</span><span class="sxs-lookup"><span data-stu-id="572a6-118">Require additional authentication at startup.</span></span>|
|<span data-ttu-id="572a6-119">startupAuthenticationBlockWithoutTpmChip</span><span class="sxs-lookup"><span data-stu-id="572a6-119">startupAuthenticationBlockWithoutTpmChip</span></span>|<span data-ttu-id="572a6-120">Booliano</span><span class="sxs-lookup"><span data-stu-id="572a6-120">Boolean</span></span>|<span data-ttu-id="572a6-121">Indica se você deseja permitir BitLocker sem um TPM compatível (exige uma senha ou uma chave de inicialização em uma unidade flash USB).</span><span class="sxs-lookup"><span data-stu-id="572a6-121">Indicates whether to allow BitLocker without a compatible TPM (requires a password or a startup key on a USB flash drive).</span></span>|
|<span data-ttu-id="572a6-122">startupAuthenticationTpmUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-122">startupAuthenticationTpmUsage</span></span>|[<span data-ttu-id="572a6-123">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-123">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="572a6-124">Indica se a inicialização do TPM é permitido/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="572a6-124">Indicates if TPM startup is allowed/required/disallowed.</span></span> <span data-ttu-id="572a6-125">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="572a6-125">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="572a6-126">startupAuthenticationTpmPinUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-126">startupAuthenticationTpmPinUsage</span></span>|[<span data-ttu-id="572a6-127">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-127">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="572a6-128">Indica se o pin de inicialização TPM é permitido/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="572a6-128">Indicates if TPM startup pin is allowed/required/disallowed.</span></span> <span data-ttu-id="572a6-129">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="572a6-129">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="572a6-130">startupAuthenticationTpmKeyUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-130">startupAuthenticationTpmKeyUsage</span></span>|[<span data-ttu-id="572a6-131">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-131">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="572a6-132">Indica se a chave de inicialização do TPM será permitido/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="572a6-132">Indicates if TPM startup key is allowed/required/disallowed.</span></span> <span data-ttu-id="572a6-133">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="572a6-133">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="572a6-134">startupAuthenticationTpmPinAndKeyUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-134">startupAuthenticationTpmPinAndKeyUsage</span></span>|[<span data-ttu-id="572a6-135">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="572a6-135">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="572a6-136">Indica se a inicialização do TPM fixar chave e chave são permitidos/necessário/não permitido.</span><span class="sxs-lookup"><span data-stu-id="572a6-136">Indicates if TPM startup pin key and key are allowed/required/disallowed.</span></span> <span data-ttu-id="572a6-137">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="572a6-137">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="572a6-138">minimumPinLength</span><span class="sxs-lookup"><span data-stu-id="572a6-138">minimumPinLength</span></span>|<span data-ttu-id="572a6-139">Int32</span><span class="sxs-lookup"><span data-stu-id="572a6-139">Int32</span></span>|<span data-ttu-id="572a6-140">Indica o tamanho mínimo do pin de inicialização.</span><span class="sxs-lookup"><span data-stu-id="572a6-140">Indicates the minimum length of startup pin.</span></span> <span data-ttu-id="572a6-141">Valores válidos 4 a 20</span><span class="sxs-lookup"><span data-stu-id="572a6-141">Valid values 4 to 20</span></span>|
|<span data-ttu-id="572a6-142">recoveryOptions</span><span class="sxs-lookup"><span data-stu-id="572a6-142">recoveryOptions</span></span>|[<span data-ttu-id="572a6-143">bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="572a6-143">bitLockerRecoveryOptions</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryoptions.md)|<span data-ttu-id="572a6-144">Permite recuperar BitLocker criptografado unidades do sistema operacional na ausência das informações de chave de inicialização necessários.</span><span class="sxs-lookup"><span data-stu-id="572a6-144">Allows to recover BitLocker encrypted operating system drives in the absence of the required startup key information.</span></span> <span data-ttu-id="572a6-145">Essa configuração de política é aplicada quando você ativa o BitLocker.</span><span class="sxs-lookup"><span data-stu-id="572a6-145">This policy setting is applied when you turn on BitLocker.</span></span>|
|<span data-ttu-id="572a6-146">prebootRecoveryEnableMessageAndUrl</span><span class="sxs-lookup"><span data-stu-id="572a6-146">prebootRecoveryEnableMessageAndUrl</span></span>|<span data-ttu-id="572a6-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="572a6-147">Boolean</span></span>|<span data-ttu-id="572a6-148">Habilite a mensagem de recuperação antes da inicialização e a Url.</span><span class="sxs-lookup"><span data-stu-id="572a6-148">Enable pre-boot recovery message and Url.</span></span> <span data-ttu-id="572a6-149">Se requireStartupAuthentication for false, esse valor não afeta.</span><span class="sxs-lookup"><span data-stu-id="572a6-149">If requireStartupAuthentication is false, this value does not affect.</span></span>|
|<span data-ttu-id="572a6-150">prebootRecoveryMessage</span><span class="sxs-lookup"><span data-stu-id="572a6-150">prebootRecoveryMessage</span></span>|<span data-ttu-id="572a6-151">String</span><span class="sxs-lookup"><span data-stu-id="572a6-151">String</span></span>|<span data-ttu-id="572a6-152">Define uma mensagem de recuperação personalizada.</span><span class="sxs-lookup"><span data-stu-id="572a6-152">Defines a custom recovery message.</span></span>|
|<span data-ttu-id="572a6-153">prebootRecoveryUrl</span><span class="sxs-lookup"><span data-stu-id="572a6-153">prebootRecoveryUrl</span></span>|<span data-ttu-id="572a6-154">String</span><span class="sxs-lookup"><span data-stu-id="572a6-154">String</span></span>|<span data-ttu-id="572a6-155">Define uma URL personalizada de recuperação.</span><span class="sxs-lookup"><span data-stu-id="572a6-155">Defines a custom recovery URL.</span></span>|

## <a name="relationships"></a><span data-ttu-id="572a6-156">Relações</span><span class="sxs-lookup"><span data-stu-id="572a6-156">Relationships</span></span>
<span data-ttu-id="572a6-157">Nenhum</span><span class="sxs-lookup"><span data-stu-id="572a6-157">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="572a6-158">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="572a6-158">JSON Representation</span></span>
<span data-ttu-id="572a6-159">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="572a6-159">Here is a JSON representation of the resource.</span></span>
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





