---
title: Atualizar androidWorkProfileGeneralDeviceConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f9e7a9e4c36823ae1b66eedaf342f6fa6574fab8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756691"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="80207-103">Atualizar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="80207-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="80207-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="80207-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="80207-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="80207-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="80207-106">Atualize as propriedades de [um objeto androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="80207-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="80207-107">Prerequisites</span></span>
<span data-ttu-id="80207-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="80207-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80207-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="80207-110">Permission type</span></span>|<span data-ttu-id="80207-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="80207-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80207-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="80207-112">Delegated (work or school account)</span></span>|<span data-ttu-id="80207-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80207-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80207-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="80207-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80207-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="80207-115">Not supported.</span></span>|
|<span data-ttu-id="80207-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="80207-116">Application</span></span>|<span data-ttu-id="80207-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80207-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="80207-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="80207-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="80207-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="80207-119">Request headers</span></span>
|<span data-ttu-id="80207-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="80207-120">Header</span></span>|<span data-ttu-id="80207-121">Valor</span><span class="sxs-lookup"><span data-stu-id="80207-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80207-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="80207-122">Authorization</span></span>|<span data-ttu-id="80207-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="80207-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80207-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="80207-124">Accept</span></span>|<span data-ttu-id="80207-125">application/json</span><span class="sxs-lookup"><span data-stu-id="80207-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80207-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="80207-126">Request body</span></span>
<span data-ttu-id="80207-127">No corpo da solicitação, fornece uma representação JSON para o [objeto androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="80207-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [o androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="80207-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="80207-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="80207-129">Property</span></span>|<span data-ttu-id="80207-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="80207-130">Type</span></span>|<span data-ttu-id="80207-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="80207-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80207-132">id</span><span class="sxs-lookup"><span data-stu-id="80207-132">id</span></span>|<span data-ttu-id="80207-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80207-133">String</span></span>|<span data-ttu-id="80207-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="80207-134">Key of the entity.</span></span> <span data-ttu-id="80207-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80207-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80207-136">lastModifiedDateTime</span></span>|<span data-ttu-id="80207-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80207-137">DateTimeOffset</span></span>|<span data-ttu-id="80207-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="80207-138">DateTime the object was last modified.</span></span> <span data-ttu-id="80207-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80207-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80207-140">createdDateTime</span></span>|<span data-ttu-id="80207-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80207-141">DateTimeOffset</span></span>|<span data-ttu-id="80207-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="80207-142">DateTime the object was created.</span></span> <span data-ttu-id="80207-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80207-144">descrição</span><span class="sxs-lookup"><span data-stu-id="80207-144">description</span></span>|<span data-ttu-id="80207-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80207-145">String</span></span>|<span data-ttu-id="80207-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80207-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="80207-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80207-148">displayName</span><span class="sxs-lookup"><span data-stu-id="80207-148">displayName</span></span>|<span data-ttu-id="80207-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="80207-149">String</span></span>|<span data-ttu-id="80207-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80207-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="80207-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80207-152">versão</span><span class="sxs-lookup"><span data-stu-id="80207-152">version</span></span>|<span data-ttu-id="80207-153">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-153">Int32</span></span>|<span data-ttu-id="80207-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="80207-154">Version of the device configuration.</span></span> <span data-ttu-id="80207-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="80207-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="80207-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="80207-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="80207-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="80207-157">Boolean</span></span>|<span data-ttu-id="80207-158">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="80207-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="80207-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="80207-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="80207-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="80207-160">Boolean</span></span>|<span data-ttu-id="80207-161">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="80207-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="80207-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="80207-162">passwordExpirationDays</span></span>|<span data-ttu-id="80207-163">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-163">Int32</span></span>|<span data-ttu-id="80207-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="80207-164">Number of days before the password expires.</span></span> <span data-ttu-id="80207-165">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="80207-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="80207-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="80207-166">passwordMinimumLength</span></span>|<span data-ttu-id="80207-167">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-167">Int32</span></span>|<span data-ttu-id="80207-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="80207-168">Minimum length of passwords.</span></span> <span data-ttu-id="80207-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="80207-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="80207-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="80207-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="80207-171">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-171">Int32</span></span>|<span data-ttu-id="80207-172">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="80207-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="80207-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="80207-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="80207-174">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-174">Int32</span></span>|<span data-ttu-id="80207-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="80207-175">Number of previous passwords to block.</span></span> <span data-ttu-id="80207-176">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="80207-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="80207-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="80207-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="80207-178">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-178">Int32</span></span>|<span data-ttu-id="80207-179">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="80207-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="80207-180">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="80207-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="80207-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="80207-181">passwordRequiredType</span></span>|[<span data-ttu-id="80207-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80207-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="80207-183">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="80207-183">Type of password that is required.</span></span> <span data-ttu-id="80207-184">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="80207-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="80207-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="80207-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="80207-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="80207-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="80207-187">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="80207-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="80207-188">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="80207-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="80207-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="80207-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="80207-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-190">Boolean</span></span>|<span data-ttu-id="80207-191">Indica se as notificações são bloqueadas ou não enquanto o dispositivo está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="80207-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="80207-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="80207-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="80207-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-193">Boolean</span></span>|<span data-ttu-id="80207-194">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="80207-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="80207-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="80207-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-196">Boolean</span></span>|<span data-ttu-id="80207-197">Permitir que dispositivos bluetooth acessem contatos corporativos.</span><span class="sxs-lookup"><span data-stu-id="80207-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="80207-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="80207-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="80207-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-199">Boolean</span></span>|<span data-ttu-id="80207-200">Bloquear captura de tela no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="80207-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="80207-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="80207-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-202">Boolean</span></span>|<span data-ttu-id="80207-203">Bloqueie a ID do chamador de perfil de trabalho de exibição no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="80207-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="80207-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="80207-204">workProfileBlockCamera</span></span>|<span data-ttu-id="80207-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-205">Boolean</span></span>|<span data-ttu-id="80207-206">Bloquear a câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-206">Block work profile camera.</span></span>|
|<span data-ttu-id="80207-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="80207-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="80207-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-208">Boolean</span></span>|<span data-ttu-id="80207-209">Bloquear a disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="80207-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="80207-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="80207-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="80207-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-211">Boolean</span></span>|<span data-ttu-id="80207-212">Boolean que indica se a configuração não permitir cópia/colar entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="80207-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="80207-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="80207-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="80207-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="80207-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="80207-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="80207-215">Type of password that is required.</span></span> <span data-ttu-id="80207-216">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="80207-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="80207-217">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="80207-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="80207-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-218">Boolean</span></span>|<span data-ttu-id="80207-219">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="80207-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="80207-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="80207-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-221">Boolean</span></span>|<span data-ttu-id="80207-222">Indica se o Smart Lock deve ou não ser bloqueado e outros agentes de confiança para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="80207-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="80207-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="80207-224">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-224">Int32</span></span>|<span data-ttu-id="80207-225">Número de dias antes que a senha do perfil de trabalho expire.</span><span class="sxs-lookup"><span data-stu-id="80207-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="80207-226">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="80207-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="80207-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="80207-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="80207-228">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-228">Int32</span></span>|<span data-ttu-id="80207-229">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-229">Minimum length of work profile password.</span></span> <span data-ttu-id="80207-230">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="80207-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="80207-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="80207-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="80207-232">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-232">Int32</span></span>|<span data-ttu-id="80207-233">Mínimo # de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="80207-234">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="80207-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80207-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="80207-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="80207-236">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-236">Int32</span></span>|<span data-ttu-id="80207-237">Mínimo # de caracteres que não são letras exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="80207-238">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="80207-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80207-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="80207-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="80207-240">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-240">Int32</span></span>|<span data-ttu-id="80207-241">Mínimo # de caracteres de letra necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="80207-242">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="80207-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80207-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="80207-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="80207-244">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-244">Int32</span></span>|<span data-ttu-id="80207-245">Mínimo # de caracteres de menor ocorrência exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="80207-246">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="80207-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80207-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="80207-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="80207-248">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-248">Int32</span></span>|<span data-ttu-id="80207-249">Mínimo # de caracteres de maiúsculas e médias exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="80207-250">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="80207-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80207-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="80207-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="80207-252">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-252">Int32</span></span>|<span data-ttu-id="80207-253">Mínimo # de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="80207-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="80207-254">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="80207-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="80207-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="80207-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="80207-256">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-256">Int32</span></span>|<span data-ttu-id="80207-257">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="80207-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="80207-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="80207-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="80207-259">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-259">Int32</span></span>|<span data-ttu-id="80207-260">Número de senhas de perfil de trabalho anteriores a bloquear.</span><span class="sxs-lookup"><span data-stu-id="80207-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="80207-261">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="80207-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="80207-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="80207-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="80207-263">Int32</span><span class="sxs-lookup"><span data-stu-id="80207-263">Int32</span></span>|<span data-ttu-id="80207-264">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="80207-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="80207-265">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="80207-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="80207-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="80207-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="80207-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="80207-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="80207-268">Tipo de senha de perfil de trabalho necessária.</span><span class="sxs-lookup"><span data-stu-id="80207-268">Type of work profile password that is required.</span></span> <span data-ttu-id="80207-269">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="80207-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="80207-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="80207-270">workProfileRequirePassword</span></span>|<span data-ttu-id="80207-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="80207-271">Boolean</span></span>|<span data-ttu-id="80207-272">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="80207-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="80207-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="80207-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="80207-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="80207-274">Boolean</span></span>|<span data-ttu-id="80207-275">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="80207-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="80207-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="80207-276">Response</span></span>
<span data-ttu-id="80207-277">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="80207-277">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80207-278">Exemplo</span><span class="sxs-lookup"><span data-stu-id="80207-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="80207-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="80207-279">Request</span></span>
<span data-ttu-id="80207-280">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="80207-280">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
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

### <a name="response"></a><span data-ttu-id="80207-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="80207-281">Response</span></span>
<span data-ttu-id="80207-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="80207-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




