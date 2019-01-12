---
title: Criar androidWorkProfileGeneralDeviceConfiguration
description: Crie um novo objeto de androidWorkProfileGeneralDeviceConfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 92cdd51d4bf68aa4607b71ca31c10b35277a06ab
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912796"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="e0232-103">Criar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e0232-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="e0232-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e0232-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0232-105">Crie um novo objeto de [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="e0232-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e0232-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e0232-106">Prerequisites</span></span>
<span data-ttu-id="e0232-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e0232-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e0232-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e0232-109">Permission type</span></span>|<span data-ttu-id="e0232-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e0232-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e0232-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e0232-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e0232-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e0232-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e0232-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e0232-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e0232-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0232-114">Not supported.</span></span>|
|<span data-ttu-id="e0232-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e0232-115">Application</span></span>|<span data-ttu-id="e0232-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e0232-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e0232-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e0232-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e0232-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e0232-118">Request headers</span></span>
|<span data-ttu-id="e0232-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e0232-119">Header</span></span>|<span data-ttu-id="e0232-120">Valor</span><span class="sxs-lookup"><span data-stu-id="e0232-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e0232-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="e0232-121">Authorization</span></span>|<span data-ttu-id="e0232-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e0232-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e0232-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e0232-123">Accept</span></span>|<span data-ttu-id="e0232-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e0232-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e0232-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e0232-125">Request body</span></span>
<span data-ttu-id="e0232-126">No corpo da solicitação, fornece uma representação JSON para o objeto androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e0232-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e0232-127">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e0232-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e0232-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e0232-128">Property</span></span>|<span data-ttu-id="e0232-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="e0232-129">Type</span></span>|<span data-ttu-id="e0232-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="e0232-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0232-131">id</span><span class="sxs-lookup"><span data-stu-id="e0232-131">id</span></span>|<span data-ttu-id="e0232-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0232-132">String</span></span>|<span data-ttu-id="e0232-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e0232-133">Key of the entity.</span></span> <span data-ttu-id="e0232-134">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0232-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0232-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e0232-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e0232-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0232-136">DateTimeOffset</span></span>|<span data-ttu-id="e0232-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e0232-137">DateTime the object was last modified.</span></span> <span data-ttu-id="e0232-138">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0232-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0232-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e0232-139">createdDateTime</span></span>|<span data-ttu-id="e0232-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e0232-140">DateTimeOffset</span></span>|<span data-ttu-id="e0232-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e0232-141">DateTime the object was created.</span></span> <span data-ttu-id="e0232-142">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0232-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0232-143">description</span><span class="sxs-lookup"><span data-stu-id="e0232-143">description</span></span>|<span data-ttu-id="e0232-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0232-144">String</span></span>|<span data-ttu-id="e0232-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0232-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e0232-146">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0232-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0232-147">displayName</span><span class="sxs-lookup"><span data-stu-id="e0232-147">displayName</span></span>|<span data-ttu-id="e0232-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e0232-148">String</span></span>|<span data-ttu-id="e0232-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0232-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e0232-150">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0232-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0232-151">version</span><span class="sxs-lookup"><span data-stu-id="e0232-151">version</span></span>|<span data-ttu-id="e0232-152">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-152">Int32</span></span>|<span data-ttu-id="e0232-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e0232-153">Version of the device configuration.</span></span> <span data-ttu-id="e0232-154">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e0232-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e0232-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e0232-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e0232-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-156">Boolean</span></span>|<span data-ttu-id="e0232-157">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e0232-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e0232-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e0232-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e0232-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-159">Boolean</span></span>|<span data-ttu-id="e0232-160">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="e0232-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e0232-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e0232-161">passwordExpirationDays</span></span>|<span data-ttu-id="e0232-162">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-162">Int32</span></span>|<span data-ttu-id="e0232-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="e0232-163">Number of days before the password expires.</span></span> <span data-ttu-id="e0232-164">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="e0232-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e0232-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e0232-165">passwordMinimumLength</span></span>|<span data-ttu-id="e0232-166">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-166">Int32</span></span>|<span data-ttu-id="e0232-167">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="e0232-167">Minimum length of passwords.</span></span> <span data-ttu-id="e0232-168">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="e0232-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e0232-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e0232-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e0232-170">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-170">Int32</span></span>|<span data-ttu-id="e0232-171">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e0232-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e0232-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e0232-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e0232-173">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-173">Int32</span></span>|<span data-ttu-id="e0232-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e0232-174">Number of previous passwords to block.</span></span> <span data-ttu-id="e0232-175">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e0232-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e0232-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e0232-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e0232-177">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-177">Int32</span></span>|<span data-ttu-id="e0232-178">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="e0232-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e0232-179">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="e0232-179">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e0232-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e0232-180">passwordRequiredType</span></span>|[<span data-ttu-id="e0232-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e0232-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e0232-182">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e0232-182">Type of password that is required.</span></span> <span data-ttu-id="e0232-183">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e0232-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e0232-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e0232-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="e0232-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e0232-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="e0232-186">Tipo de dados de compartilhamento que é permitido.</span><span class="sxs-lookup"><span data-stu-id="e0232-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="e0232-187">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="e0232-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="e0232-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e0232-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="e0232-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-189">Boolean</span></span>|<span data-ttu-id="e0232-190">Indica se deve ou não bloquear notificações de dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e0232-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="e0232-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="e0232-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="e0232-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-192">Boolean</span></span>|<span data-ttu-id="e0232-193">Impedir que os usuários de adicionar/remover contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="e0232-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="e0232-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="e0232-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-195">Boolean</span></span>|<span data-ttu-id="e0232-196">Permitir que os dispositivos bluetooth acessar contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="e0232-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="e0232-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e0232-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="e0232-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-198">Boolean</span></span>|<span data-ttu-id="e0232-199">Captura de tela de bloqueio no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="e0232-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="e0232-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="e0232-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-201">Boolean</span></span>|<span data-ttu-id="e0232-202">Bloquear exibição trabalho perfil ID do chamador no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e0232-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="e0232-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="e0232-203">workProfileBlockCamera</span></span>|<span data-ttu-id="e0232-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-204">Boolean</span></span>|<span data-ttu-id="e0232-205">Câmera de perfil de trabalho de bloco.</span><span class="sxs-lookup"><span data-stu-id="e0232-205">Block work profile camera.</span></span>|
|<span data-ttu-id="e0232-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="e0232-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="e0232-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-207">Boolean</span></span>|<span data-ttu-id="e0232-208">Disponibilidade do bloco trabalho perfil contatos no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e0232-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="e0232-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e0232-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="e0232-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-210">Boolean</span></span>|<span data-ttu-id="e0232-211">Boolean que indica se a configuração não permitir cruzado perfil copiar/colar está habilitada.</span><span class="sxs-lookup"><span data-stu-id="e0232-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="e0232-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="e0232-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="e0232-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e0232-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="e0232-214">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e0232-214">Type of password that is required.</span></span> <span data-ttu-id="e0232-215">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="e0232-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e0232-216">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e0232-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e0232-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-217">Boolean</span></span>|<span data-ttu-id="e0232-218">Indica se o bloqueio da impressão digital ou não desbloquear para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="e0232-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e0232-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="e0232-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-220">Boolean</span></span>|<span data-ttu-id="e0232-221">Indica se deve ou não bloquear bloqueio inteligente e outros operadores de confiabilidade para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="e0232-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e0232-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="e0232-223">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-223">Int32</span></span>|<span data-ttu-id="e0232-224">Número de dias até a senha do perfil de trabalho expira.</span><span class="sxs-lookup"><span data-stu-id="e0232-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="e0232-225">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="e0232-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e0232-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e0232-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="e0232-227">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-227">Int32</span></span>|<span data-ttu-id="e0232-228">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-228">Minimum length of work profile password.</span></span> <span data-ttu-id="e0232-229">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="e0232-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e0232-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="e0232-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="e0232-231">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-231">Int32</span></span>|<span data-ttu-id="e0232-232">Número mínimo de caracteres numéricos necessários em senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="e0232-233">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e0232-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e0232-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e0232-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="e0232-235">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-235">Int32</span></span>|<span data-ttu-id="e0232-236">Número mínimo de caracteres não alfabéticos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="e0232-237">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e0232-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e0232-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e0232-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="e0232-239">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-239">Int32</span></span>|<span data-ttu-id="e0232-240">Número mínimo de caracteres de carta necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="e0232-241">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e0232-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e0232-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e0232-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="e0232-243">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-243">Int32</span></span>|<span data-ttu-id="e0232-244">Número mínimo de caracteres minúscula necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="e0232-245">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e0232-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e0232-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e0232-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="e0232-247">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-247">Int32</span></span>|<span data-ttu-id="e0232-248">Número mínimo de caracteres de maiusculas necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="e0232-249">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e0232-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e0232-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="e0232-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="e0232-251">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-251">Int32</span></span>|<span data-ttu-id="e0232-252">Número mínimo de símbolos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e0232-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="e0232-253">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e0232-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e0232-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e0232-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e0232-255">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-255">Int32</span></span>|<span data-ttu-id="e0232-256">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e0232-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e0232-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e0232-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e0232-258">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-258">Int32</span></span>|<span data-ttu-id="e0232-259">Número de senhas anteriores de perfil de trabalho para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e0232-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="e0232-260">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e0232-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e0232-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e0232-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e0232-262">Int32</span><span class="sxs-lookup"><span data-stu-id="e0232-262">Int32</span></span>|<span data-ttu-id="e0232-263">Número de falhas permitidas antes que o perfil de trabalho é removido e todos os dados corporativos excluídos de entrada.</span><span class="sxs-lookup"><span data-stu-id="e0232-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="e0232-264">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="e0232-264">Valid values 4 to 11</span></span>|
|<span data-ttu-id="e0232-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e0232-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="e0232-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e0232-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e0232-267">Tipo de senha de perfil de trabalho que é necessário.</span><span class="sxs-lookup"><span data-stu-id="e0232-267">Type of work profile password that is required.</span></span> <span data-ttu-id="e0232-268">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e0232-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e0232-269">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e0232-269">workProfileRequirePassword</span></span>|<span data-ttu-id="e0232-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-270">Boolean</span></span>|<span data-ttu-id="e0232-271">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="e0232-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="e0232-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e0232-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="e0232-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="e0232-273">Boolean</span></span>|<span data-ttu-id="e0232-274">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="e0232-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="e0232-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0232-275">Response</span></span>
<span data-ttu-id="e0232-276">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e0232-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e0232-277">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e0232-277">Example</span></span>
### <a name="request"></a><span data-ttu-id="e0232-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0232-278">Request</span></span>
<span data-ttu-id="e0232-279">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e0232-279">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 1831

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```

### <a name="response"></a><span data-ttu-id="e0232-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0232-280">Response</span></span>
<span data-ttu-id="e0232-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e0232-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2003

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "passwordBlockFingerprintUnlock": true,
  "passwordBlockTrustAgents": true,
  "passwordExpirationDays": 6,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordSignInFailureCountBeforeFactoryReset": 12,
  "passwordRequiredType": "lowSecurityBiometric",
  "workProfileDataSharingType": "preventAny",
  "workProfileBlockNotificationsWhileDeviceLocked": true,
  "workProfileBlockAddingAccounts": true,
  "workProfileBluetoothEnableContactSharing": true,
  "workProfileBlockScreenCapture": true,
  "workProfileBlockCrossProfileCallerId": true,
  "workProfileBlockCamera": true,
  "workProfileBlockCrossProfileContactsSearch": true,
  "workProfileBlockCrossProfileCopyPaste": true,
  "workProfileDefaultAppPermissionPolicy": "prompt",
  "workProfilePasswordBlockFingerprintUnlock": true,
  "workProfilePasswordBlockTrustAgents": true,
  "workProfilePasswordExpirationDays": 1,
  "workProfilePasswordMinimumLength": 0,
  "workProfilePasswordMinNumericCharacters": 7,
  "workProfilePasswordMinNonLetterCharacters": 9,
  "workProfilePasswordMinLetterCharacters": 6,
  "workProfilePasswordMinLowerCaseCharacters": 9,
  "workProfilePasswordMinUpperCaseCharacters": 9,
  "workProfilePasswordMinSymbolCharacters": 6,
  "workProfilePasswordMinutesOfInactivityBeforeScreenTimeout": 9,
  "workProfilePasswordPreviousPasswordBlockCount": 13,
  "workProfilePasswordSignInFailureCountBeforeFactoryReset": 7,
  "workProfilePasswordRequiredType": "lowSecurityBiometric",
  "workProfileRequirePassword": true,
  "securityRequireVerifyApps": true
}
```



