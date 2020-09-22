---
title: Atualizar Entidadeandroidforworkprofiledeviceconfiguration
description: Atualiza as propriedades de um objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5be72c082b368ff8066de8b06aeed8cb8dbb1bc1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48083614"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="a2401-103">Atualizar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="a2401-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="a2401-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2401-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2401-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a2401-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2401-106">Atualiza as propriedades de um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a2401-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a2401-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a2401-107">Prerequisites</span></span>
<span data-ttu-id="a2401-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a2401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2401-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a2401-110">Permission type</span></span>|<span data-ttu-id="a2401-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a2401-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2401-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a2401-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a2401-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2401-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a2401-114">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a2401-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2401-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2401-115">Not supported.</span></span>|
|<span data-ttu-id="a2401-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a2401-116">Application</span></span>|<span data-ttu-id="a2401-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a2401-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2401-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a2401-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a2401-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a2401-119">Request headers</span></span>
|<span data-ttu-id="a2401-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a2401-120">Header</span></span>|<span data-ttu-id="a2401-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a2401-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2401-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a2401-122">Authorization</span></span>|<span data-ttu-id="a2401-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a2401-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2401-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a2401-124">Accept</span></span>|<span data-ttu-id="a2401-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a2401-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2401-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a2401-126">Request body</span></span>
<span data-ttu-id="a2401-127">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="a2401-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="a2401-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="a2401-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="a2401-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a2401-129">Property</span></span>|<span data-ttu-id="a2401-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a2401-130">Type</span></span>|<span data-ttu-id="a2401-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a2401-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2401-132">id</span><span class="sxs-lookup"><span data-stu-id="a2401-132">id</span></span>|<span data-ttu-id="a2401-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2401-133">String</span></span>|<span data-ttu-id="a2401-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a2401-134">Key of the entity.</span></span> <span data-ttu-id="a2401-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2401-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2401-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2401-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a2401-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2401-137">DateTimeOffset</span></span>|<span data-ttu-id="a2401-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="a2401-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a2401-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2401-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2401-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a2401-140">createdDateTime</span></span>|<span data-ttu-id="a2401-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2401-141">DateTimeOffset</span></span>|<span data-ttu-id="a2401-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="a2401-142">DateTime the object was created.</span></span> <span data-ttu-id="a2401-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2401-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2401-144">description</span><span class="sxs-lookup"><span data-stu-id="a2401-144">description</span></span>|<span data-ttu-id="a2401-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2401-145">String</span></span>|<span data-ttu-id="a2401-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2401-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a2401-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2401-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2401-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a2401-148">displayName</span></span>|<span data-ttu-id="a2401-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a2401-149">String</span></span>|<span data-ttu-id="a2401-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2401-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a2401-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2401-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2401-152">versão</span><span class="sxs-lookup"><span data-stu-id="a2401-152">version</span></span>|<span data-ttu-id="a2401-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-153">Int32</span></span>|<span data-ttu-id="a2401-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a2401-154">Version of the device configuration.</span></span> <span data-ttu-id="a2401-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a2401-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a2401-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="a2401-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a2401-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2401-157">Boolean</span></span>|<span data-ttu-id="a2401-158">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a2401-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="a2401-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a2401-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="a2401-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2401-160">Boolean</span></span>|<span data-ttu-id="a2401-161">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="a2401-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="a2401-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a2401-162">passwordExpirationDays</span></span>|<span data-ttu-id="a2401-163">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-163">Int32</span></span>|<span data-ttu-id="a2401-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="a2401-164">Number of days before the password expires.</span></span> <span data-ttu-id="a2401-165">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="a2401-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a2401-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2401-166">passwordMinimumLength</span></span>|<span data-ttu-id="a2401-167">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-167">Int32</span></span>|<span data-ttu-id="a2401-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="a2401-168">Minimum length of passwords.</span></span> <span data-ttu-id="a2401-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="a2401-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a2401-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a2401-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a2401-171">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-171">Int32</span></span>|<span data-ttu-id="a2401-172">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="a2401-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a2401-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a2401-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a2401-174">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-174">Int32</span></span>|<span data-ttu-id="a2401-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="a2401-175">Number of previous passwords to block.</span></span> <span data-ttu-id="a2401-176">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="a2401-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a2401-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a2401-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a2401-178">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-178">Int32</span></span>|<span data-ttu-id="a2401-179">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="a2401-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="a2401-180">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="a2401-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a2401-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a2401-181">passwordRequiredType</span></span>|[<span data-ttu-id="a2401-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a2401-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a2401-183">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="a2401-183">Type of password that is required.</span></span> <span data-ttu-id="a2401-184">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a2401-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a2401-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a2401-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="a2401-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="a2401-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="a2401-187">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="a2401-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="a2401-188">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="a2401-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="a2401-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="a2401-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="a2401-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-190">Boolean</span></span>|<span data-ttu-id="a2401-191">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a2401-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="a2401-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="a2401-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="a2401-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-193">Boolean</span></span>|<span data-ttu-id="a2401-194">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="a2401-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="a2401-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="a2401-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-196">Boolean</span></span>|<span data-ttu-id="a2401-197">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="a2401-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="a2401-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="a2401-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="a2401-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-199">Boolean</span></span>|<span data-ttu-id="a2401-200">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="a2401-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="a2401-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="a2401-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-202">Boolean</span></span>|<span data-ttu-id="a2401-203">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="a2401-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="a2401-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="a2401-204">workProfileBlockCamera</span></span>|<span data-ttu-id="a2401-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-205">Boolean</span></span>|<span data-ttu-id="a2401-206">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-206">Block work profile camera.</span></span>|
|<span data-ttu-id="a2401-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="a2401-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="a2401-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-208">Boolean</span></span>|<span data-ttu-id="a2401-209">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="a2401-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="a2401-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="a2401-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="a2401-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-211">Boolean</span></span>|<span data-ttu-id="a2401-212">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="a2401-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="a2401-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="a2401-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="a2401-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="a2401-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="a2401-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="a2401-215">Type of password that is required.</span></span> <span data-ttu-id="a2401-216">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="a2401-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="a2401-217">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="a2401-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="a2401-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-218">Boolean</span></span>|<span data-ttu-id="a2401-219">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="a2401-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="a2401-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="a2401-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="a2401-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-221">Boolean</span></span>|<span data-ttu-id="a2401-222">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="a2401-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="a2401-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="a2401-224">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-224">Int32</span></span>|<span data-ttu-id="a2401-225">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="a2401-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="a2401-226">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="a2401-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="a2401-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="a2401-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="a2401-228">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-228">Int32</span></span>|<span data-ttu-id="a2401-229">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-229">Minimum length of work profile password.</span></span> <span data-ttu-id="a2401-230">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="a2401-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="a2401-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="a2401-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="a2401-232">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-232">Int32</span></span>|<span data-ttu-id="a2401-233">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="a2401-234">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a2401-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a2401-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="a2401-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="a2401-236">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-236">Int32</span></span>|<span data-ttu-id="a2401-237">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="a2401-238">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a2401-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a2401-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="a2401-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="a2401-240">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-240">Int32</span></span>|<span data-ttu-id="a2401-241">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="a2401-242">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a2401-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a2401-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="a2401-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="a2401-244">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-244">Int32</span></span>|<span data-ttu-id="a2401-245">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="a2401-246">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a2401-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a2401-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="a2401-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="a2401-248">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-248">Int32</span></span>|<span data-ttu-id="a2401-249">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="a2401-250">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a2401-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a2401-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="a2401-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="a2401-252">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-252">Int32</span></span>|<span data-ttu-id="a2401-253">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a2401-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="a2401-254">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="a2401-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="a2401-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="a2401-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="a2401-256">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-256">Int32</span></span>|<span data-ttu-id="a2401-257">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="a2401-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="a2401-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="a2401-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="a2401-259">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-259">Int32</span></span>|<span data-ttu-id="a2401-260">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="a2401-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="a2401-261">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="a2401-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="a2401-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="a2401-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="a2401-263">Int32</span><span class="sxs-lookup"><span data-stu-id="a2401-263">Int32</span></span>|<span data-ttu-id="a2401-264">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="a2401-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="a2401-265">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="a2401-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="a2401-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="a2401-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="a2401-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="a2401-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="a2401-268">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="a2401-268">Type of work profile password that is required.</span></span> <span data-ttu-id="a2401-269">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="a2401-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="a2401-270">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="a2401-270">workProfileRequirePassword</span></span>|<span data-ttu-id="a2401-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="a2401-271">Boolean</span></span>|<span data-ttu-id="a2401-272">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="a2401-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="a2401-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="a2401-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="a2401-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="a2401-274">Boolean</span></span>|<span data-ttu-id="a2401-275">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="a2401-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="a2401-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2401-276">Response</span></span>
<span data-ttu-id="a2401-277">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a2401-277">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2401-278">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a2401-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="a2401-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a2401-279">Request</span></span>
<span data-ttu-id="a2401-280">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a2401-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a2401-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="a2401-281">Response</span></span>
<span data-ttu-id="a2401-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a2401-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









