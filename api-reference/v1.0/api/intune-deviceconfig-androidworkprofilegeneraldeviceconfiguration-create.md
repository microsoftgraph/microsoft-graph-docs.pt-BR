---
title: Criar Entidadeandroidforworkprofiledeviceconfiguration
description: Criar um novo objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 86a0c8a5951d22a5283d5343201a2efa7d85ca64
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515221"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="709ef-103">Criar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="709ef-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="709ef-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="709ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="709ef-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="709ef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="709ef-106">Criar um novo objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="709ef-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="709ef-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="709ef-107">Prerequisites</span></span>
<span data-ttu-id="709ef-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="709ef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="709ef-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="709ef-110">Permission type</span></span>|<span data-ttu-id="709ef-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="709ef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="709ef-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="709ef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="709ef-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="709ef-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="709ef-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="709ef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="709ef-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="709ef-115">Not supported.</span></span>|
|<span data-ttu-id="709ef-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="709ef-116">Application</span></span>|<span data-ttu-id="709ef-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="709ef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="709ef-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="709ef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="709ef-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="709ef-119">Request headers</span></span>
|<span data-ttu-id="709ef-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="709ef-120">Header</span></span>|<span data-ttu-id="709ef-121">Valor</span><span class="sxs-lookup"><span data-stu-id="709ef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="709ef-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="709ef-122">Authorization</span></span>|<span data-ttu-id="709ef-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="709ef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="709ef-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="709ef-124">Accept</span></span>|<span data-ttu-id="709ef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="709ef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="709ef-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="709ef-126">Request body</span></span>
<span data-ttu-id="709ef-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="709ef-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="709ef-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="709ef-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="709ef-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="709ef-129">Property</span></span>|<span data-ttu-id="709ef-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="709ef-130">Type</span></span>|<span data-ttu-id="709ef-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="709ef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="709ef-132">id</span><span class="sxs-lookup"><span data-stu-id="709ef-132">id</span></span>|<span data-ttu-id="709ef-133">String</span><span class="sxs-lookup"><span data-stu-id="709ef-133">String</span></span>|<span data-ttu-id="709ef-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="709ef-134">Key of the entity.</span></span> <span data-ttu-id="709ef-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="709ef-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="709ef-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="709ef-136">lastModifiedDateTime</span></span>|<span data-ttu-id="709ef-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="709ef-137">DateTimeOffset</span></span>|<span data-ttu-id="709ef-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="709ef-138">DateTime the object was last modified.</span></span> <span data-ttu-id="709ef-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="709ef-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="709ef-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="709ef-140">createdDateTime</span></span>|<span data-ttu-id="709ef-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="709ef-141">DateTimeOffset</span></span>|<span data-ttu-id="709ef-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="709ef-142">DateTime the object was created.</span></span> <span data-ttu-id="709ef-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="709ef-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="709ef-144">description</span><span class="sxs-lookup"><span data-stu-id="709ef-144">description</span></span>|<span data-ttu-id="709ef-145">String</span><span class="sxs-lookup"><span data-stu-id="709ef-145">String</span></span>|<span data-ttu-id="709ef-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="709ef-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="709ef-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="709ef-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="709ef-148">displayName</span><span class="sxs-lookup"><span data-stu-id="709ef-148">displayName</span></span>|<span data-ttu-id="709ef-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="709ef-149">String</span></span>|<span data-ttu-id="709ef-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="709ef-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="709ef-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="709ef-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="709ef-152">versão</span><span class="sxs-lookup"><span data-stu-id="709ef-152">version</span></span>|<span data-ttu-id="709ef-153">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-153">Int32</span></span>|<span data-ttu-id="709ef-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="709ef-154">Version of the device configuration.</span></span> <span data-ttu-id="709ef-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="709ef-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="709ef-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="709ef-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="709ef-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-157">Boolean</span></span>|<span data-ttu-id="709ef-158">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="709ef-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="709ef-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="709ef-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="709ef-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="709ef-160">Boolean</span></span>|<span data-ttu-id="709ef-161">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="709ef-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="709ef-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="709ef-162">passwordExpirationDays</span></span>|<span data-ttu-id="709ef-163">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-163">Int32</span></span>|<span data-ttu-id="709ef-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="709ef-164">Number of days before the password expires.</span></span> <span data-ttu-id="709ef-165">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="709ef-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="709ef-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="709ef-166">passwordMinimumLength</span></span>|<span data-ttu-id="709ef-167">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-167">Int32</span></span>|<span data-ttu-id="709ef-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="709ef-168">Minimum length of passwords.</span></span> <span data-ttu-id="709ef-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="709ef-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="709ef-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="709ef-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="709ef-171">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-171">Int32</span></span>|<span data-ttu-id="709ef-172">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="709ef-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="709ef-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="709ef-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="709ef-174">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-174">Int32</span></span>|<span data-ttu-id="709ef-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="709ef-175">Number of previous passwords to block.</span></span> <span data-ttu-id="709ef-176">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="709ef-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="709ef-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="709ef-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="709ef-178">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-178">Int32</span></span>|<span data-ttu-id="709ef-179">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="709ef-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="709ef-180">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="709ef-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="709ef-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="709ef-181">passwordRequiredType</span></span>|[<span data-ttu-id="709ef-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="709ef-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="709ef-183">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="709ef-183">Type of password that is required.</span></span> <span data-ttu-id="709ef-184">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="709ef-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="709ef-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="709ef-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="709ef-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="709ef-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="709ef-187">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="709ef-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="709ef-188">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="709ef-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="709ef-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="709ef-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="709ef-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-190">Boolean</span></span>|<span data-ttu-id="709ef-191">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="709ef-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="709ef-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="709ef-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="709ef-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-193">Boolean</span></span>|<span data-ttu-id="709ef-194">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="709ef-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="709ef-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="709ef-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-196">Boolean</span></span>|<span data-ttu-id="709ef-197">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="709ef-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="709ef-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="709ef-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="709ef-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-199">Boolean</span></span>|<span data-ttu-id="709ef-200">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="709ef-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="709ef-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="709ef-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-202">Boolean</span></span>|<span data-ttu-id="709ef-203">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="709ef-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="709ef-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="709ef-204">workProfileBlockCamera</span></span>|<span data-ttu-id="709ef-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-205">Boolean</span></span>|<span data-ttu-id="709ef-206">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-206">Block work profile camera.</span></span>|
|<span data-ttu-id="709ef-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="709ef-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="709ef-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-208">Boolean</span></span>|<span data-ttu-id="709ef-209">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="709ef-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="709ef-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="709ef-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="709ef-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-211">Boolean</span></span>|<span data-ttu-id="709ef-212">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="709ef-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="709ef-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="709ef-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="709ef-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="709ef-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="709ef-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="709ef-215">Type of password that is required.</span></span> <span data-ttu-id="709ef-216">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="709ef-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="709ef-217">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="709ef-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="709ef-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-218">Boolean</span></span>|<span data-ttu-id="709ef-219">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="709ef-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="709ef-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="709ef-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="709ef-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-221">Boolean</span></span>|<span data-ttu-id="709ef-222">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="709ef-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="709ef-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="709ef-224">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-224">Int32</span></span>|<span data-ttu-id="709ef-225">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="709ef-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="709ef-226">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="709ef-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="709ef-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="709ef-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="709ef-228">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-228">Int32</span></span>|<span data-ttu-id="709ef-229">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-229">Minimum length of work profile password.</span></span> <span data-ttu-id="709ef-230">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="709ef-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="709ef-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="709ef-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="709ef-232">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-232">Int32</span></span>|<span data-ttu-id="709ef-233">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="709ef-234">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="709ef-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="709ef-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="709ef-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="709ef-236">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-236">Int32</span></span>|<span data-ttu-id="709ef-237">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="709ef-238">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="709ef-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="709ef-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="709ef-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="709ef-240">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-240">Int32</span></span>|<span data-ttu-id="709ef-241">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="709ef-242">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="709ef-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="709ef-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="709ef-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="709ef-244">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-244">Int32</span></span>|<span data-ttu-id="709ef-245">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="709ef-246">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="709ef-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="709ef-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="709ef-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="709ef-248">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-248">Int32</span></span>|<span data-ttu-id="709ef-249">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="709ef-250">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="709ef-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="709ef-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="709ef-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="709ef-252">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-252">Int32</span></span>|<span data-ttu-id="709ef-253">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="709ef-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="709ef-254">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="709ef-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="709ef-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="709ef-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="709ef-256">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-256">Int32</span></span>|<span data-ttu-id="709ef-257">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="709ef-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="709ef-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="709ef-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="709ef-259">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-259">Int32</span></span>|<span data-ttu-id="709ef-260">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="709ef-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="709ef-261">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="709ef-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="709ef-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="709ef-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="709ef-263">Int32</span><span class="sxs-lookup"><span data-stu-id="709ef-263">Int32</span></span>|<span data-ttu-id="709ef-264">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="709ef-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="709ef-265">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="709ef-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="709ef-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="709ef-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="709ef-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="709ef-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="709ef-268">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="709ef-268">Type of work profile password that is required.</span></span> <span data-ttu-id="709ef-269">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="709ef-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="709ef-270">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="709ef-270">workProfileRequirePassword</span></span>|<span data-ttu-id="709ef-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="709ef-271">Boolean</span></span>|<span data-ttu-id="709ef-272">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="709ef-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="709ef-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="709ef-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="709ef-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="709ef-274">Boolean</span></span>|<span data-ttu-id="709ef-275">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="709ef-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="709ef-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="709ef-276">Response</span></span>
<span data-ttu-id="709ef-277">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="709ef-277">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="709ef-278">Exemplo</span><span class="sxs-lookup"><span data-stu-id="709ef-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="709ef-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="709ef-279">Request</span></span>
<span data-ttu-id="709ef-280">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="709ef-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="709ef-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="709ef-281">Response</span></span>
<span data-ttu-id="709ef-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="709ef-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




