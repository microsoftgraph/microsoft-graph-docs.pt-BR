---
title: Atualizar Entidadeandroidforworkprofiledeviceconfiguration
description: Atualiza as propriedades de um objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dd4fd11e3941fc45bea38f8ba600b91d84ca18d4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35997824"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="76f3c-103">Atualizar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="76f3c-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="76f3c-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="76f3c-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76f3c-105">Atualiza as propriedades de um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="76f3c-105">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76f3c-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="76f3c-106">Prerequisites</span></span>
<span data-ttu-id="76f3c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="76f3c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76f3c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="76f3c-109">Permission type</span></span>|<span data-ttu-id="76f3c-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="76f3c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76f3c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="76f3c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="76f3c-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76f3c-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="76f3c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="76f3c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76f3c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76f3c-114">Not supported.</span></span>|
|<span data-ttu-id="76f3c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="76f3c-115">Application</span></span>|<span data-ttu-id="76f3c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="76f3c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="76f3c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="76f3c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="76f3c-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="76f3c-118">Request headers</span></span>
|<span data-ttu-id="76f3c-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="76f3c-119">Header</span></span>|<span data-ttu-id="76f3c-120">Valor</span><span class="sxs-lookup"><span data-stu-id="76f3c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76f3c-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="76f3c-121">Authorization</span></span>|<span data-ttu-id="76f3c-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="76f3c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76f3c-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="76f3c-123">Accept</span></span>|<span data-ttu-id="76f3c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="76f3c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76f3c-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="76f3c-125">Request body</span></span>
<span data-ttu-id="76f3c-126">No corpo da solicitação, forneça uma representação JSON do objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="76f3c-126">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="76f3c-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="76f3c-127">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="76f3c-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76f3c-128">Property</span></span>|<span data-ttu-id="76f3c-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="76f3c-129">Type</span></span>|<span data-ttu-id="76f3c-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="76f3c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76f3c-131">id</span><span class="sxs-lookup"><span data-stu-id="76f3c-131">id</span></span>|<span data-ttu-id="76f3c-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="76f3c-132">String</span></span>|<span data-ttu-id="76f3c-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="76f3c-133">Key of the entity.</span></span> <span data-ttu-id="76f3c-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76f3c-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76f3c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="76f3c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="76f3c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76f3c-136">DateTimeOffset</span></span>|<span data-ttu-id="76f3c-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="76f3c-137">DateTime the object was last modified.</span></span> <span data-ttu-id="76f3c-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76f3c-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76f3c-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76f3c-139">createdDateTime</span></span>|<span data-ttu-id="76f3c-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76f3c-140">DateTimeOffset</span></span>|<span data-ttu-id="76f3c-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="76f3c-141">DateTime the object was created.</span></span> <span data-ttu-id="76f3c-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76f3c-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76f3c-143">descrição</span><span class="sxs-lookup"><span data-stu-id="76f3c-143">description</span></span>|<span data-ttu-id="76f3c-144">String</span><span class="sxs-lookup"><span data-stu-id="76f3c-144">String</span></span>|<span data-ttu-id="76f3c-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76f3c-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="76f3c-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76f3c-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76f3c-147">displayName</span><span class="sxs-lookup"><span data-stu-id="76f3c-147">displayName</span></span>|<span data-ttu-id="76f3c-148">String</span><span class="sxs-lookup"><span data-stu-id="76f3c-148">String</span></span>|<span data-ttu-id="76f3c-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76f3c-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="76f3c-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76f3c-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76f3c-151">versão</span><span class="sxs-lookup"><span data-stu-id="76f3c-151">version</span></span>|<span data-ttu-id="76f3c-152">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-152">Int32</span></span>|<span data-ttu-id="76f3c-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="76f3c-153">Version of the device configuration.</span></span> <span data-ttu-id="76f3c-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="76f3c-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="76f3c-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="76f3c-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="76f3c-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-156">Boolean</span></span>|<span data-ttu-id="76f3c-157">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="76f3c-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="76f3c-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="76f3c-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="76f3c-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="76f3c-159">Boolean</span></span>|<span data-ttu-id="76f3c-160">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="76f3c-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="76f3c-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="76f3c-161">passwordExpirationDays</span></span>|<span data-ttu-id="76f3c-162">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-162">Int32</span></span>|<span data-ttu-id="76f3c-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="76f3c-163">Number of days before the password expires.</span></span> <span data-ttu-id="76f3c-164">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="76f3c-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="76f3c-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="76f3c-165">passwordMinimumLength</span></span>|<span data-ttu-id="76f3c-166">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-166">Int32</span></span>|<span data-ttu-id="76f3c-167">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="76f3c-167">Minimum length of passwords.</span></span> <span data-ttu-id="76f3c-168">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="76f3c-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="76f3c-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="76f3c-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="76f3c-170">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-170">Int32</span></span>|<span data-ttu-id="76f3c-171">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="76f3c-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="76f3c-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="76f3c-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="76f3c-173">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-173">Int32</span></span>|<span data-ttu-id="76f3c-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="76f3c-174">Number of previous passwords to block.</span></span> <span data-ttu-id="76f3c-175">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="76f3c-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="76f3c-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="76f3c-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="76f3c-177">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-177">Int32</span></span>|<span data-ttu-id="76f3c-178">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="76f3c-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="76f3c-179">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="76f3c-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="76f3c-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="76f3c-180">passwordRequiredType</span></span>|[<span data-ttu-id="76f3c-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="76f3c-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="76f3c-182">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="76f3c-182">Type of password that is required.</span></span> <span data-ttu-id="76f3c-183">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="76f3c-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="76f3c-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="76f3c-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="76f3c-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="76f3c-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="76f3c-186">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="76f3c-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="76f3c-187">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="76f3c-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="76f3c-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="76f3c-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="76f3c-189">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-189">Boolean</span></span>|<span data-ttu-id="76f3c-190">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="76f3c-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="76f3c-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="76f3c-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="76f3c-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-192">Boolean</span></span>|<span data-ttu-id="76f3c-193">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="76f3c-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="76f3c-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="76f3c-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-195">Boolean</span></span>|<span data-ttu-id="76f3c-196">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="76f3c-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="76f3c-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="76f3c-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="76f3c-198">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-198">Boolean</span></span>|<span data-ttu-id="76f3c-199">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="76f3c-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="76f3c-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="76f3c-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-201">Boolean</span></span>|<span data-ttu-id="76f3c-202">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="76f3c-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="76f3c-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="76f3c-203">workProfileBlockCamera</span></span>|<span data-ttu-id="76f3c-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-204">Boolean</span></span>|<span data-ttu-id="76f3c-205">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-205">Block work profile camera.</span></span>|
|<span data-ttu-id="76f3c-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="76f3c-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="76f3c-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-207">Boolean</span></span>|<span data-ttu-id="76f3c-208">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="76f3c-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="76f3c-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="76f3c-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="76f3c-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-210">Boolean</span></span>|<span data-ttu-id="76f3c-211">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="76f3c-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="76f3c-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="76f3c-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="76f3c-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="76f3c-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="76f3c-214">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="76f3c-214">Type of password that is required.</span></span> <span data-ttu-id="76f3c-215">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="76f3c-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="76f3c-216">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="76f3c-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="76f3c-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-217">Boolean</span></span>|<span data-ttu-id="76f3c-218">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="76f3c-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="76f3c-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="76f3c-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="76f3c-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-220">Boolean</span></span>|<span data-ttu-id="76f3c-221">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="76f3c-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="76f3c-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="76f3c-223">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-223">Int32</span></span>|<span data-ttu-id="76f3c-224">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="76f3c-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="76f3c-225">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="76f3c-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="76f3c-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="76f3c-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="76f3c-227">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-227">Int32</span></span>|<span data-ttu-id="76f3c-228">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-228">Minimum length of work profile password.</span></span> <span data-ttu-id="76f3c-229">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="76f3c-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="76f3c-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="76f3c-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="76f3c-231">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-231">Int32</span></span>|<span data-ttu-id="76f3c-232">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="76f3c-233">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="76f3c-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="76f3c-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="76f3c-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="76f3c-235">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-235">Int32</span></span>|<span data-ttu-id="76f3c-236">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="76f3c-237">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="76f3c-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="76f3c-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="76f3c-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="76f3c-239">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-239">Int32</span></span>|<span data-ttu-id="76f3c-240">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="76f3c-241">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="76f3c-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="76f3c-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="76f3c-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="76f3c-243">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-243">Int32</span></span>|<span data-ttu-id="76f3c-244">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="76f3c-245">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="76f3c-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="76f3c-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="76f3c-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="76f3c-247">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-247">Int32</span></span>|<span data-ttu-id="76f3c-248">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="76f3c-249">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="76f3c-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="76f3c-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="76f3c-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="76f3c-251">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-251">Int32</span></span>|<span data-ttu-id="76f3c-252">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="76f3c-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="76f3c-253">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="76f3c-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="76f3c-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="76f3c-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="76f3c-255">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-255">Int32</span></span>|<span data-ttu-id="76f3c-256">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="76f3c-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="76f3c-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="76f3c-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="76f3c-258">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-258">Int32</span></span>|<span data-ttu-id="76f3c-259">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="76f3c-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="76f3c-260">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="76f3c-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="76f3c-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="76f3c-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="76f3c-262">Int32</span><span class="sxs-lookup"><span data-stu-id="76f3c-262">Int32</span></span>|<span data-ttu-id="76f3c-263">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="76f3c-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="76f3c-264">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="76f3c-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="76f3c-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="76f3c-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="76f3c-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="76f3c-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="76f3c-267">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="76f3c-267">Type of work profile password that is required.</span></span> <span data-ttu-id="76f3c-268">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="76f3c-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="76f3c-269">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="76f3c-269">workProfileRequirePassword</span></span>|<span data-ttu-id="76f3c-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="76f3c-270">Boolean</span></span>|<span data-ttu-id="76f3c-271">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="76f3c-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="76f3c-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="76f3c-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="76f3c-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="76f3c-273">Boolean</span></span>|<span data-ttu-id="76f3c-274">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="76f3c-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="76f3c-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="76f3c-275">Response</span></span>
<span data-ttu-id="76f3c-276">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="76f3c-276">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="76f3c-277">Exemplo</span><span class="sxs-lookup"><span data-stu-id="76f3c-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="76f3c-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="76f3c-278">Request</span></span>
<span data-ttu-id="76f3c-279">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="76f3c-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="76f3c-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="76f3c-280">Response</span></span>
<span data-ttu-id="76f3c-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="76f3c-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



