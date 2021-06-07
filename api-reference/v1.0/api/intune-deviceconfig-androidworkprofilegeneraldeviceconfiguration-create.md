---
title: Criar androidWorkProfileGeneralDeviceConfiguration
description: Crie um novo objeto androidWorkProfileGeneralDeviceConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0412305e90178662d1a88c0ec3114460e19583a4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52750256"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="e122c-103">Criar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="e122c-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="e122c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e122c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e122c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e122c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e122c-106">Crie um novo [objeto androidWorkProfileGeneralDeviceConfiguration.](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-106">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e122c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e122c-107">Prerequisites</span></span>
<span data-ttu-id="e122c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e122c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e122c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e122c-110">Permission type</span></span>|<span data-ttu-id="e122c-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="e122c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e122c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e122c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e122c-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e122c-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e122c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e122c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e122c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e122c-115">Not supported.</span></span>|
|<span data-ttu-id="e122c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e122c-116">Application</span></span>|<span data-ttu-id="e122c-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e122c-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e122c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e122c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e122c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e122c-119">Request headers</span></span>
|<span data-ttu-id="e122c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e122c-120">Header</span></span>|<span data-ttu-id="e122c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="e122c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e122c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="e122c-122">Authorization</span></span>|<span data-ttu-id="e122c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e122c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e122c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e122c-124">Accept</span></span>|<span data-ttu-id="e122c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e122c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e122c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e122c-126">Request body</span></span>
<span data-ttu-id="e122c-127">No corpo da solicitação, fornece uma representação JSON para o objeto androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e122c-127">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="e122c-128">A tabela a seguir mostra as propriedades necessárias ao criar o androidWorkProfileGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="e122c-128">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="e122c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e122c-129">Property</span></span>|<span data-ttu-id="e122c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="e122c-130">Type</span></span>|<span data-ttu-id="e122c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="e122c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e122c-132">id</span><span class="sxs-lookup"><span data-stu-id="e122c-132">id</span></span>|<span data-ttu-id="e122c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e122c-133">String</span></span>|<span data-ttu-id="e122c-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e122c-134">Key of the entity.</span></span> <span data-ttu-id="e122c-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e122c-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e122c-136">lastModifiedDateTime</span></span>|<span data-ttu-id="e122c-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e122c-137">DateTimeOffset</span></span>|<span data-ttu-id="e122c-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="e122c-138">DateTime the object was last modified.</span></span> <span data-ttu-id="e122c-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e122c-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e122c-140">createdDateTime</span></span>|<span data-ttu-id="e122c-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e122c-141">DateTimeOffset</span></span>|<span data-ttu-id="e122c-142">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="e122c-142">DateTime the object was created.</span></span> <span data-ttu-id="e122c-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e122c-144">descrição</span><span class="sxs-lookup"><span data-stu-id="e122c-144">description</span></span>|<span data-ttu-id="e122c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e122c-145">String</span></span>|<span data-ttu-id="e122c-146">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e122c-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="e122c-147">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e122c-148">displayName</span><span class="sxs-lookup"><span data-stu-id="e122c-148">displayName</span></span>|<span data-ttu-id="e122c-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e122c-149">String</span></span>|<span data-ttu-id="e122c-150">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e122c-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="e122c-151">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e122c-152">versão</span><span class="sxs-lookup"><span data-stu-id="e122c-152">version</span></span>|<span data-ttu-id="e122c-153">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-153">Int32</span></span>|<span data-ttu-id="e122c-154">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e122c-154">Version of the device configuration.</span></span> <span data-ttu-id="e122c-155">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="e122c-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="e122c-156">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e122c-156">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e122c-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="e122c-157">Boolean</span></span>|<span data-ttu-id="e122c-158">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e122c-158">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="e122c-159">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e122c-159">passwordBlockTrustAgents</span></span>|<span data-ttu-id="e122c-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="e122c-160">Boolean</span></span>|<span data-ttu-id="e122c-161">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="e122c-161">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="e122c-162">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e122c-162">passwordExpirationDays</span></span>|<span data-ttu-id="e122c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-163">Int32</span></span>|<span data-ttu-id="e122c-164">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="e122c-164">Number of days before the password expires.</span></span> <span data-ttu-id="e122c-165">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="e122c-165">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e122c-166">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e122c-166">passwordMinimumLength</span></span>|<span data-ttu-id="e122c-167">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-167">Int32</span></span>|<span data-ttu-id="e122c-168">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="e122c-168">Minimum length of passwords.</span></span> <span data-ttu-id="e122c-169">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="e122c-169">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e122c-170">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e122c-170">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e122c-171">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-171">Int32</span></span>|<span data-ttu-id="e122c-172">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e122c-172">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e122c-173">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e122c-173">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e122c-174">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-174">Int32</span></span>|<span data-ttu-id="e122c-175">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="e122c-175">Number of previous passwords to block.</span></span> <span data-ttu-id="e122c-176">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e122c-176">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e122c-177">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e122c-177">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e122c-178">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-178">Int32</span></span>|<span data-ttu-id="e122c-179">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="e122c-179">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="e122c-180">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="e122c-180">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e122c-181">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e122c-181">passwordRequiredType</span></span>|[<span data-ttu-id="e122c-182">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e122c-182">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e122c-183">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e122c-183">Type of password that is required.</span></span> <span data-ttu-id="e122c-184">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e122c-184">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e122c-185">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e122c-185">workProfileDataSharingType</span></span>|[<span data-ttu-id="e122c-186">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="e122c-186">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="e122c-187">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="e122c-187">Type of data sharing that is allowed.</span></span> <span data-ttu-id="e122c-188">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="e122c-188">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="e122c-189">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="e122c-189">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="e122c-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-190">Boolean</span></span>|<span data-ttu-id="e122c-191">Indica se as notificações são bloqueadas ou não enquanto o dispositivo está bloqueado.</span><span class="sxs-lookup"><span data-stu-id="e122c-191">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="e122c-192">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="e122c-192">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="e122c-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-193">Boolean</span></span>|<span data-ttu-id="e122c-194">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-194">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="e122c-195">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="e122c-195">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="e122c-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-196">Boolean</span></span>|<span data-ttu-id="e122c-197">Permitir que dispositivos bluetooth acessem contatos corporativos.</span><span class="sxs-lookup"><span data-stu-id="e122c-197">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="e122c-198">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="e122c-198">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="e122c-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-199">Boolean</span></span>|<span data-ttu-id="e122c-200">Bloquear captura de tela no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-200">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="e122c-201">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="e122c-201">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="e122c-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-202">Boolean</span></span>|<span data-ttu-id="e122c-203">Bloqueie a ID do chamador de perfil de trabalho de exibição no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e122c-203">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="e122c-204">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="e122c-204">workProfileBlockCamera</span></span>|<span data-ttu-id="e122c-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-205">Boolean</span></span>|<span data-ttu-id="e122c-206">Bloquear a câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-206">Block work profile camera.</span></span>|
|<span data-ttu-id="e122c-207">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="e122c-207">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="e122c-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-208">Boolean</span></span>|<span data-ttu-id="e122c-209">Bloquear a disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="e122c-209">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="e122c-210">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="e122c-210">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="e122c-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-211">Boolean</span></span>|<span data-ttu-id="e122c-212">Boolean que indica se a configuração não permitir cópia/colar entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="e122c-212">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="e122c-213">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="e122c-213">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="e122c-214">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="e122c-214">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="e122c-215">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="e122c-215">Type of password that is required.</span></span> <span data-ttu-id="e122c-216">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="e122c-216">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="e122c-217">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="e122c-217">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="e122c-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-218">Boolean</span></span>|<span data-ttu-id="e122c-219">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-219">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="e122c-220">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="e122c-220">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="e122c-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-221">Boolean</span></span>|<span data-ttu-id="e122c-222">Indica se o Smart Lock deve ou não ser bloqueado e outros agentes de confiança para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-222">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="e122c-223">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="e122c-223">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="e122c-224">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-224">Int32</span></span>|<span data-ttu-id="e122c-225">Número de dias antes que a senha do perfil de trabalho expire.</span><span class="sxs-lookup"><span data-stu-id="e122c-225">Number of days before the work profile password expires.</span></span> <span data-ttu-id="e122c-226">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="e122c-226">Valid values 1 to 365</span></span>|
|<span data-ttu-id="e122c-227">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="e122c-227">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="e122c-228">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-228">Int32</span></span>|<span data-ttu-id="e122c-229">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-229">Minimum length of work profile password.</span></span> <span data-ttu-id="e122c-230">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="e122c-230">Valid values 4 to 16</span></span>|
|<span data-ttu-id="e122c-231">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="e122c-231">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="e122c-232">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-232">Int32</span></span>|<span data-ttu-id="e122c-233">Mínimo # de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-233">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="e122c-234">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e122c-234">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e122c-235">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e122c-235">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="e122c-236">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-236">Int32</span></span>|<span data-ttu-id="e122c-237">Mínimo # de caracteres que não são letras exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-237">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="e122c-238">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e122c-238">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e122c-239">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="e122c-239">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="e122c-240">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-240">Int32</span></span>|<span data-ttu-id="e122c-241">Mínimo # de caracteres de letra necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-241">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="e122c-242">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e122c-242">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e122c-243">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e122c-243">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="e122c-244">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-244">Int32</span></span>|<span data-ttu-id="e122c-245">Mínimo # de caracteres de menor ocorrência exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-245">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="e122c-246">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e122c-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e122c-247">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="e122c-247">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="e122c-248">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-248">Int32</span></span>|<span data-ttu-id="e122c-249">Mínimo # de caracteres de maiúsculas e médias exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-249">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="e122c-250">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e122c-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e122c-251">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="e122c-251">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="e122c-252">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-252">Int32</span></span>|<span data-ttu-id="e122c-253">Mínimo # de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="e122c-253">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="e122c-254">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="e122c-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="e122c-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="e122c-255">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="e122c-256">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-256">Int32</span></span>|<span data-ttu-id="e122c-257">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="e122c-257">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="e122c-258">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="e122c-258">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="e122c-259">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-259">Int32</span></span>|<span data-ttu-id="e122c-260">Número de senhas de perfil de trabalho anteriores a bloquear.</span><span class="sxs-lookup"><span data-stu-id="e122c-260">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="e122c-261">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="e122c-261">Valid values 0 to 24</span></span>|
|<span data-ttu-id="e122c-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="e122c-262">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="e122c-263">Int32</span><span class="sxs-lookup"><span data-stu-id="e122c-263">Int32</span></span>|<span data-ttu-id="e122c-264">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="e122c-264">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="e122c-265">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="e122c-265">Valid values 1 to 16</span></span>|
|<span data-ttu-id="e122c-266">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="e122c-266">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="e122c-267">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="e122c-267">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="e122c-268">Tipo de senha de perfil de trabalho necessária.</span><span class="sxs-lookup"><span data-stu-id="e122c-268">Type of work profile password that is required.</span></span> <span data-ttu-id="e122c-269">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="e122c-269">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="e122c-270">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="e122c-270">workProfileRequirePassword</span></span>|<span data-ttu-id="e122c-271">Booliano</span><span class="sxs-lookup"><span data-stu-id="e122c-271">Boolean</span></span>|<span data-ttu-id="e122c-272">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="e122c-272">Password is required or not for work profile</span></span>|
|<span data-ttu-id="e122c-273">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="e122c-273">securityRequireVerifyApps</span></span>|<span data-ttu-id="e122c-274">Boolean</span><span class="sxs-lookup"><span data-stu-id="e122c-274">Boolean</span></span>|<span data-ttu-id="e122c-275">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="e122c-275">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="e122c-276">Resposta</span><span class="sxs-lookup"><span data-stu-id="e122c-276">Response</span></span>
<span data-ttu-id="e122c-277">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e122c-277">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e122c-278">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e122c-278">Example</span></span>

### <a name="request"></a><span data-ttu-id="e122c-279">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e122c-279">Request</span></span>
<span data-ttu-id="e122c-280">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e122c-280">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e122c-281">Resposta</span><span class="sxs-lookup"><span data-stu-id="e122c-281">Response</span></span>
<span data-ttu-id="e122c-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e122c-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




