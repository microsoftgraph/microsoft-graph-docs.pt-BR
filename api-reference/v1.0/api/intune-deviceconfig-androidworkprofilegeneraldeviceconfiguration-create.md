---
title: Criar Entidadeandroidforworkprofiledeviceconfiguration
description: Criar um novo objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b482e574782548721a8fe7dd957df2ec5932d21
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083649"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="34ccd-103">Criar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="34ccd-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="34ccd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34ccd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34ccd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34ccd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34ccd-106">Criar um novo objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="34ccd-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="34ccd-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="34ccd-107">Prerequisites</span></span>
<span data-ttu-id="34ccd-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="34ccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="34ccd-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="34ccd-110">Permission type</span></span>|<span data-ttu-id="34ccd-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="34ccd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="34ccd-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="34ccd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="34ccd-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="34ccd-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="34ccd-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="34ccd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="34ccd-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ccd-115">Not supported.</span></span>|
|<span data-ttu-id="34ccd-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="34ccd-116">Application</span></span>|<span data-ttu-id="34ccd-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="34ccd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="34ccd-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="34ccd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="34ccd-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="34ccd-119">Request headers</span></span>
|<span data-ttu-id="34ccd-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="34ccd-120">Header</span></span>|<span data-ttu-id="34ccd-121">Valor</span><span class="sxs-lookup"><span data-stu-id="34ccd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="34ccd-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="34ccd-122">Authorization</span></span>|<span data-ttu-id="34ccd-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="34ccd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="34ccd-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="34ccd-124">Accept</span></span>|<span data-ttu-id="34ccd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="34ccd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="34ccd-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="34ccd-126">Request body</span></span>
<span data-ttu-id="34ccd-127">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="34ccd-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="34ccd-128">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="34ccd-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="34ccd-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34ccd-129">Property</span></span>|<span data-ttu-id="34ccd-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="34ccd-130">Type</span></span>|<span data-ttu-id="34ccd-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="34ccd-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34ccd-132">id</span><span class="sxs-lookup"><span data-stu-id="34ccd-132">id</span></span>|<span data-ttu-id="34ccd-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34ccd-133">String</span></span>|<span data-ttu-id="34ccd-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="34ccd-134">Key of the entity.</span></span> <span data-ttu-id="34ccd-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ccd-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ccd-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="34ccd-136">lastModifiedDateTime</span></span>|<span data-ttu-id="34ccd-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ccd-137">DateTimeOffset</span></span>|<span data-ttu-id="34ccd-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="34ccd-138">DateTime the object was last modified.</span></span> <span data-ttu-id="34ccd-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ccd-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ccd-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="34ccd-140">createdDateTime</span></span>|<span data-ttu-id="34ccd-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34ccd-141">DateTimeOffset</span></span>|<span data-ttu-id="34ccd-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="34ccd-142">DateTime the object was created.</span></span> <span data-ttu-id="34ccd-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ccd-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ccd-144">description</span><span class="sxs-lookup"><span data-stu-id="34ccd-144">description</span></span>|<span data-ttu-id="34ccd-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34ccd-145">String</span></span>|<span data-ttu-id="34ccd-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34ccd-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="34ccd-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ccd-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ccd-148">displayName</span><span class="sxs-lookup"><span data-stu-id="34ccd-148">displayName</span></span>|<span data-ttu-id="34ccd-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34ccd-149">String</span></span>|<span data-ttu-id="34ccd-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34ccd-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="34ccd-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ccd-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ccd-152">versão</span><span class="sxs-lookup"><span data-stu-id="34ccd-152">version</span></span>|<span data-ttu-id="34ccd-153">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-153">Int32</span></span>|<span data-ttu-id="34ccd-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="34ccd-154">Version of the device configuration.</span></span> <span data-ttu-id="34ccd-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="34ccd-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="34ccd-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="34ccd-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="34ccd-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ccd-157">Boolean</span></span>|<span data-ttu-id="34ccd-158">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="34ccd-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="34ccd-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="34ccd-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="34ccd-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ccd-160">Boolean</span></span>|<span data-ttu-id="34ccd-161">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="34ccd-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="34ccd-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="34ccd-162">passwordExpirationDays</span></span>|<span data-ttu-id="34ccd-163">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-163">Int32</span></span>|<span data-ttu-id="34ccd-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="34ccd-164">Number of days before the password expires.</span></span> <span data-ttu-id="34ccd-165">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="34ccd-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="34ccd-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="34ccd-166">passwordMinimumLength</span></span>|<span data-ttu-id="34ccd-167">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-167">Int32</span></span>|<span data-ttu-id="34ccd-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="34ccd-168">Minimum length of passwords.</span></span> <span data-ttu-id="34ccd-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="34ccd-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="34ccd-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="34ccd-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="34ccd-171">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-171">Int32</span></span>|<span data-ttu-id="34ccd-172">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="34ccd-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="34ccd-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="34ccd-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="34ccd-174">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-174">Int32</span></span>|<span data-ttu-id="34ccd-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="34ccd-175">Number of previous passwords to block.</span></span> <span data-ttu-id="34ccd-176">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="34ccd-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="34ccd-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="34ccd-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="34ccd-178">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-178">Int32</span></span>|<span data-ttu-id="34ccd-179">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="34ccd-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="34ccd-180">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="34ccd-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="34ccd-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="34ccd-181">passwordRequiredType</span></span>|[<span data-ttu-id="34ccd-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34ccd-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="34ccd-183">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="34ccd-183">Type of password that is required.</span></span> <span data-ttu-id="34ccd-184">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="34ccd-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="34ccd-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="34ccd-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="34ccd-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="34ccd-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="34ccd-187">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="34ccd-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="34ccd-188">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="34ccd-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="34ccd-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="34ccd-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="34ccd-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-190">Boolean</span></span>|<span data-ttu-id="34ccd-191">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="34ccd-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="34ccd-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="34ccd-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="34ccd-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-193">Boolean</span></span>|<span data-ttu-id="34ccd-194">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="34ccd-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="34ccd-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="34ccd-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-196">Boolean</span></span>|<span data-ttu-id="34ccd-197">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="34ccd-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="34ccd-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="34ccd-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="34ccd-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-199">Boolean</span></span>|<span data-ttu-id="34ccd-200">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="34ccd-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="34ccd-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="34ccd-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-202">Boolean</span></span>|<span data-ttu-id="34ccd-203">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="34ccd-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="34ccd-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="34ccd-204">workProfileBlockCamera</span></span>|<span data-ttu-id="34ccd-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-205">Boolean</span></span>|<span data-ttu-id="34ccd-206">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-206">Block work profile camera.</span></span>|
|<span data-ttu-id="34ccd-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="34ccd-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="34ccd-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-208">Boolean</span></span>|<span data-ttu-id="34ccd-209">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="34ccd-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="34ccd-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="34ccd-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="34ccd-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-211">Boolean</span></span>|<span data-ttu-id="34ccd-212">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="34ccd-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="34ccd-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="34ccd-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="34ccd-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="34ccd-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="34ccd-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="34ccd-215">Type of password that is required.</span></span> <span data-ttu-id="34ccd-216">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="34ccd-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="34ccd-217">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="34ccd-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="34ccd-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-218">Boolean</span></span>|<span data-ttu-id="34ccd-219">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="34ccd-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="34ccd-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="34ccd-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="34ccd-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-221">Boolean</span></span>|<span data-ttu-id="34ccd-222">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="34ccd-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="34ccd-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="34ccd-224">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-224">Int32</span></span>|<span data-ttu-id="34ccd-225">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="34ccd-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="34ccd-226">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="34ccd-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="34ccd-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="34ccd-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="34ccd-228">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-228">Int32</span></span>|<span data-ttu-id="34ccd-229">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-229">Minimum length of work profile password.</span></span> <span data-ttu-id="34ccd-230">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="34ccd-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="34ccd-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="34ccd-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="34ccd-232">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-232">Int32</span></span>|<span data-ttu-id="34ccd-233">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="34ccd-234">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="34ccd-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="34ccd-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="34ccd-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="34ccd-236">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-236">Int32</span></span>|<span data-ttu-id="34ccd-237">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="34ccd-238">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="34ccd-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="34ccd-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="34ccd-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="34ccd-240">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-240">Int32</span></span>|<span data-ttu-id="34ccd-241">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="34ccd-242">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="34ccd-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="34ccd-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="34ccd-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="34ccd-244">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-244">Int32</span></span>|<span data-ttu-id="34ccd-245">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="34ccd-246">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="34ccd-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="34ccd-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="34ccd-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="34ccd-248">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-248">Int32</span></span>|<span data-ttu-id="34ccd-249">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="34ccd-250">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="34ccd-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="34ccd-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="34ccd-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="34ccd-252">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-252">Int32</span></span>|<span data-ttu-id="34ccd-253">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34ccd-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="34ccd-254">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="34ccd-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="34ccd-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="34ccd-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="34ccd-256">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-256">Int32</span></span>|<span data-ttu-id="34ccd-257">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="34ccd-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="34ccd-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="34ccd-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="34ccd-259">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-259">Int32</span></span>|<span data-ttu-id="34ccd-260">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="34ccd-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="34ccd-261">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="34ccd-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="34ccd-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="34ccd-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="34ccd-263">Int32</span><span class="sxs-lookup"><span data-stu-id="34ccd-263">Int32</span></span>|<span data-ttu-id="34ccd-264">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="34ccd-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="34ccd-265">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="34ccd-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="34ccd-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="34ccd-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="34ccd-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="34ccd-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="34ccd-268">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="34ccd-268">Type of work profile password that is required.</span></span> <span data-ttu-id="34ccd-269">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="34ccd-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="34ccd-270">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="34ccd-270">workProfileRequirePassword</span></span>|<span data-ttu-id="34ccd-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="34ccd-271">Boolean</span></span>|<span data-ttu-id="34ccd-272">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="34ccd-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="34ccd-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="34ccd-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="34ccd-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="34ccd-274">Boolean</span></span>|<span data-ttu-id="34ccd-275">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="34ccd-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="34ccd-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ccd-276">Response</span></span>
<span data-ttu-id="34ccd-277">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="34ccd-277">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="34ccd-278">Exemplo</span><span class="sxs-lookup"><span data-stu-id="34ccd-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="34ccd-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="34ccd-279">Request</span></span>
<span data-ttu-id="34ccd-280">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="34ccd-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="34ccd-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="34ccd-281">Response</span></span>
<span data-ttu-id="34ccd-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="34ccd-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









