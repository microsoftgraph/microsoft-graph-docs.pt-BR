---
title: Atualizar Entidadeandroidforworkprofiledeviceconfiguration
description: Atualiza as propriedades de um objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6968e62a3c1fb3e86dc4329e569cea5eeda4722
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515193"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="5ef8a-103">Atualizar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="5ef8a-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="5ef8a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ef8a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5ef8a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5ef8a-106">Atualiza as propriedades de um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ef8a-106">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5ef8a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5ef8a-107">Prerequisites</span></span>
<span data-ttu-id="5ef8a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5ef8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ef8a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5ef8a-110">Permission type</span></span>|<span data-ttu-id="5ef8a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ef8a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5ef8a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ef8a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5ef8a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ef8a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-115">Not supported.</span></span>|
|<span data-ttu-id="5ef8a-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5ef8a-116">Application</span></span>|<span data-ttu-id="5ef8a-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ef8a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5ef8a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="5ef8a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5ef8a-119">Request headers</span></span>
|<span data-ttu-id="5ef8a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5ef8a-120">Header</span></span>|<span data-ttu-id="5ef8a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="5ef8a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ef8a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="5ef8a-122">Authorization</span></span>|<span data-ttu-id="5ef8a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ef8a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5ef8a-124">Accept</span></span>|<span data-ttu-id="5ef8a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5ef8a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ef8a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5ef8a-126">Request body</span></span>
<span data-ttu-id="5ef8a-127">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="5ef8a-127">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="5ef8a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="5ef8a-128">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="5ef8a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5ef8a-129">Property</span></span>|<span data-ttu-id="5ef8a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="5ef8a-130">Type</span></span>|<span data-ttu-id="5ef8a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="5ef8a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ef8a-132">id</span><span class="sxs-lookup"><span data-stu-id="5ef8a-132">id</span></span>|<span data-ttu-id="5ef8a-133">String</span><span class="sxs-lookup"><span data-stu-id="5ef8a-133">String</span></span>|<span data-ttu-id="5ef8a-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-134">Key of the entity.</span></span> <span data-ttu-id="5ef8a-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ef8a-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5ef8a-136">lastModifiedDateTime</span></span>|<span data-ttu-id="5ef8a-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ef8a-137">DateTimeOffset</span></span>|<span data-ttu-id="5ef8a-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-138">DateTime the object was last modified.</span></span> <span data-ttu-id="5ef8a-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ef8a-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5ef8a-140">createdDateTime</span></span>|<span data-ttu-id="5ef8a-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5ef8a-141">DateTimeOffset</span></span>|<span data-ttu-id="5ef8a-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-142">DateTime the object was created.</span></span> <span data-ttu-id="5ef8a-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ef8a-144">description</span><span class="sxs-lookup"><span data-stu-id="5ef8a-144">description</span></span>|<span data-ttu-id="5ef8a-145">String</span><span class="sxs-lookup"><span data-stu-id="5ef8a-145">String</span></span>|<span data-ttu-id="5ef8a-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="5ef8a-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ef8a-148">displayName</span><span class="sxs-lookup"><span data-stu-id="5ef8a-148">displayName</span></span>|<span data-ttu-id="5ef8a-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5ef8a-149">String</span></span>|<span data-ttu-id="5ef8a-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="5ef8a-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ef8a-152">versão</span><span class="sxs-lookup"><span data-stu-id="5ef8a-152">version</span></span>|<span data-ttu-id="5ef8a-153">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-153">Int32</span></span>|<span data-ttu-id="5ef8a-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-154">Version of the device configuration.</span></span> <span data-ttu-id="5ef8a-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="5ef8a-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="5ef8a-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="5ef8a-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="5ef8a-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-157">Boolean</span></span>|<span data-ttu-id="5ef8a-158">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="5ef8a-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="5ef8a-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="5ef8a-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ef8a-160">Boolean</span></span>|<span data-ttu-id="5ef8a-161">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="5ef8a-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5ef8a-162">passwordExpirationDays</span></span>|<span data-ttu-id="5ef8a-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-163">Int32</span></span>|<span data-ttu-id="5ef8a-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-164">Number of days before the password expires.</span></span> <span data-ttu-id="5ef8a-165">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="5ef8a-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5ef8a-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5ef8a-166">passwordMinimumLength</span></span>|<span data-ttu-id="5ef8a-167">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-167">Int32</span></span>|<span data-ttu-id="5ef8a-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-168">Minimum length of passwords.</span></span> <span data-ttu-id="5ef8a-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="5ef8a-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5ef8a-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5ef8a-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5ef8a-171">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-171">Int32</span></span>|<span data-ttu-id="5ef8a-172">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="5ef8a-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5ef8a-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5ef8a-174">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-174">Int32</span></span>|<span data-ttu-id="5ef8a-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-175">Number of previous passwords to block.</span></span> <span data-ttu-id="5ef8a-176">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="5ef8a-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5ef8a-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5ef8a-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5ef8a-178">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-178">Int32</span></span>|<span data-ttu-id="5ef8a-179">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="5ef8a-180">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5ef8a-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5ef8a-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-181">passwordRequiredType</span></span>|[<span data-ttu-id="5ef8a-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="5ef8a-183">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-183">Type of password that is required.</span></span> <span data-ttu-id="5ef8a-184">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="5ef8a-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="5ef8a-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="5ef8a-187">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="5ef8a-188">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="5ef8a-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="5ef8a-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="5ef8a-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-190">Boolean</span></span>|<span data-ttu-id="5ef8a-191">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="5ef8a-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="5ef8a-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="5ef8a-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-193">Boolean</span></span>|<span data-ttu-id="5ef8a-194">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="5ef8a-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="5ef8a-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="5ef8a-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-196">Boolean</span></span>|<span data-ttu-id="5ef8a-197">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="5ef8a-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="5ef8a-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="5ef8a-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-199">Boolean</span></span>|<span data-ttu-id="5ef8a-200">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="5ef8a-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="5ef8a-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="5ef8a-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-202">Boolean</span></span>|<span data-ttu-id="5ef8a-203">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="5ef8a-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="5ef8a-204">workProfileBlockCamera</span></span>|<span data-ttu-id="5ef8a-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-205">Boolean</span></span>|<span data-ttu-id="5ef8a-206">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-206">Block work profile camera.</span></span>|
|<span data-ttu-id="5ef8a-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="5ef8a-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="5ef8a-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-208">Boolean</span></span>|<span data-ttu-id="5ef8a-209">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="5ef8a-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="5ef8a-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="5ef8a-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-211">Boolean</span></span>|<span data-ttu-id="5ef8a-212">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="5ef8a-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="5ef8a-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="5ef8a-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="5ef8a-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-215">Type of password that is required.</span></span> <span data-ttu-id="5ef8a-216">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="5ef8a-217">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="5ef8a-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="5ef8a-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-218">Boolean</span></span>|<span data-ttu-id="5ef8a-219">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="5ef8a-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="5ef8a-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="5ef8a-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-221">Boolean</span></span>|<span data-ttu-id="5ef8a-222">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="5ef8a-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="5ef8a-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="5ef8a-224">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-224">Int32</span></span>|<span data-ttu-id="5ef8a-225">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="5ef8a-226">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="5ef8a-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="5ef8a-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="5ef8a-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="5ef8a-228">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-228">Int32</span></span>|<span data-ttu-id="5ef8a-229">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-229">Minimum length of work profile password.</span></span> <span data-ttu-id="5ef8a-230">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="5ef8a-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="5ef8a-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="5ef8a-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="5ef8a-232">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-232">Int32</span></span>|<span data-ttu-id="5ef8a-233">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="5ef8a-234">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="5ef8a-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="5ef8a-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="5ef8a-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="5ef8a-236">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-236">Int32</span></span>|<span data-ttu-id="5ef8a-237">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="5ef8a-238">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="5ef8a-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="5ef8a-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="5ef8a-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="5ef8a-240">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-240">Int32</span></span>|<span data-ttu-id="5ef8a-241">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="5ef8a-242">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="5ef8a-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="5ef8a-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="5ef8a-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="5ef8a-244">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-244">Int32</span></span>|<span data-ttu-id="5ef8a-245">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="5ef8a-246">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="5ef8a-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="5ef8a-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="5ef8a-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="5ef8a-248">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-248">Int32</span></span>|<span data-ttu-id="5ef8a-249">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="5ef8a-250">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="5ef8a-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="5ef8a-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="5ef8a-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="5ef8a-252">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-252">Int32</span></span>|<span data-ttu-id="5ef8a-253">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="5ef8a-254">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="5ef8a-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="5ef8a-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="5ef8a-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="5ef8a-256">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-256">Int32</span></span>|<span data-ttu-id="5ef8a-257">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="5ef8a-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="5ef8a-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="5ef8a-259">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-259">Int32</span></span>|<span data-ttu-id="5ef8a-260">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="5ef8a-261">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="5ef8a-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="5ef8a-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="5ef8a-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="5ef8a-263">Int32</span><span class="sxs-lookup"><span data-stu-id="5ef8a-263">Int32</span></span>|<span data-ttu-id="5ef8a-264">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="5ef8a-265">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="5ef8a-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="5ef8a-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="5ef8a-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="5ef8a-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="5ef8a-268">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-268">Type of work profile password that is required.</span></span> <span data-ttu-id="5ef8a-269">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="5ef8a-270">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="5ef8a-270">workProfileRequirePassword</span></span>|<span data-ttu-id="5ef8a-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="5ef8a-271">Boolean</span></span>|<span data-ttu-id="5ef8a-272">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="5ef8a-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="5ef8a-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="5ef8a-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="5ef8a-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="5ef8a-274">Boolean</span></span>|<span data-ttu-id="5ef8a-275">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="5ef8a-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ef8a-276">Response</span></span>
<span data-ttu-id="5ef8a-277">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-277">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ef8a-278">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5ef8a-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="5ef8a-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5ef8a-279">Request</span></span>
<span data-ttu-id="5ef8a-280">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5ef8a-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="5ef8a-281">Response</span></span>
<span data-ttu-id="5ef8a-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5ef8a-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




