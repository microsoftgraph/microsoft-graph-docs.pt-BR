---
title: Criar Entidadeandroidforworkprofiledeviceconfiguration
description: Criar um novo objeto Entidadeandroidforworkprofiledeviceconfiguration.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b0e1ae2e8eed358054163295dc8608a1bbaba68f
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30960199"
---
# <a name="create-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="1e4b5-103">Criar Entidadeandroidforworkprofiledeviceconfiguration</span><span class="sxs-lookup"><span data-stu-id="1e4b5-103">Create androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="1e4b5-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e4b5-105">Criar um novo objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="1e4b5-105">Create a new [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e4b5-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1e4b5-106">Prerequisites</span></span>
<span data-ttu-id="1e4b5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1e4b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e4b5-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1e4b5-109">Permission type</span></span>|<span data-ttu-id="1e4b5-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e4b5-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1e4b5-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e4b5-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1e4b5-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e4b5-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-114">Not supported.</span></span>|
|<span data-ttu-id="1e4b5-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="1e4b5-115">Application</span></span>|<span data-ttu-id="1e4b5-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e4b5-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1e4b5-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="1e4b5-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4b5-118">Request headers</span></span>
|<span data-ttu-id="1e4b5-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1e4b5-119">Header</span></span>|<span data-ttu-id="1e4b5-120">Valor</span><span class="sxs-lookup"><span data-stu-id="1e4b5-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e4b5-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="1e4b5-121">Authorization</span></span>|<span data-ttu-id="1e4b5-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e4b5-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1e4b5-123">Accept</span></span>|<span data-ttu-id="1e4b5-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1e4b5-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e4b5-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4b5-125">Request body</span></span>
<span data-ttu-id="1e4b5-126">No corpo da solicitação, forneça uma representação JSON do objeto Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-126">In the request body, supply a JSON representation for the androidWorkProfileGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="1e4b5-127">A tabela a seguir mostra as propriedades que são necessárias ao criar Entidadeandroidforworkprofiledeviceconfiguration.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-127">The following table shows the properties that are required when you create the androidWorkProfileGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="1e4b5-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1e4b5-128">Property</span></span>|<span data-ttu-id="1e4b5-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="1e4b5-129">Type</span></span>|<span data-ttu-id="1e4b5-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="1e4b5-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e4b5-131">id</span><span class="sxs-lookup"><span data-stu-id="1e4b5-131">id</span></span>|<span data-ttu-id="1e4b5-132">String</span><span class="sxs-lookup"><span data-stu-id="1e4b5-132">String</span></span>|<span data-ttu-id="1e4b5-133">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-133">Key of the entity.</span></span> <span data-ttu-id="1e4b5-134">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e4b5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4b5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="1e4b5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4b5-136">DateTimeOffset</span></span>|<span data-ttu-id="1e4b5-137">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-137">DateTime the object was last modified.</span></span> <span data-ttu-id="1e4b5-138">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e4b5-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1e4b5-139">createdDateTime</span></span>|<span data-ttu-id="1e4b5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1e4b5-140">DateTimeOffset</span></span>|<span data-ttu-id="1e4b5-141">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-141">DateTime the object was created.</span></span> <span data-ttu-id="1e4b5-142">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e4b5-143">descrição</span><span class="sxs-lookup"><span data-stu-id="1e4b5-143">description</span></span>|<span data-ttu-id="1e4b5-144">String</span><span class="sxs-lookup"><span data-stu-id="1e4b5-144">String</span></span>|<span data-ttu-id="1e4b5-145">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="1e4b5-146">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e4b5-147">displayName</span><span class="sxs-lookup"><span data-stu-id="1e4b5-147">displayName</span></span>|<span data-ttu-id="1e4b5-148">String</span><span class="sxs-lookup"><span data-stu-id="1e4b5-148">String</span></span>|<span data-ttu-id="1e4b5-149">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="1e4b5-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e4b5-151">versão</span><span class="sxs-lookup"><span data-stu-id="1e4b5-151">version</span></span>|<span data-ttu-id="1e4b5-152">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-152">Int32</span></span>|<span data-ttu-id="1e4b5-153">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-153">Version of the device configuration.</span></span> <span data-ttu-id="1e4b5-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="1e4b5-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="1e4b5-155">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="1e4b5-155">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1e4b5-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-156">Boolean</span></span>|<span data-ttu-id="1e4b5-157">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-157">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="1e4b5-158">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="1e4b5-158">passwordBlockTrustAgents</span></span>|<span data-ttu-id="1e4b5-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-159">Boolean</span></span>|<span data-ttu-id="1e4b5-160">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-160">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="1e4b5-161">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1e4b5-161">passwordExpirationDays</span></span>|<span data-ttu-id="1e4b5-162">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-162">Int32</span></span>|<span data-ttu-id="1e4b5-163">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-163">Number of days before the password expires.</span></span> <span data-ttu-id="1e4b5-164">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="1e4b5-164">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1e4b5-165">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1e4b5-165">passwordMinimumLength</span></span>|<span data-ttu-id="1e4b5-166">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-166">Int32</span></span>|<span data-ttu-id="1e4b5-167">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-167">Minimum length of passwords.</span></span> <span data-ttu-id="1e4b5-168">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="1e4b5-168">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1e4b5-169">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1e4b5-169">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1e4b5-170">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-170">Int32</span></span>|<span data-ttu-id="1e4b5-171">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-171">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1e4b5-172">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1e4b5-172">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1e4b5-173">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-173">Int32</span></span>|<span data-ttu-id="1e4b5-174">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-174">Number of previous passwords to block.</span></span> <span data-ttu-id="1e4b5-175">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="1e4b5-175">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1e4b5-176">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1e4b5-176">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1e4b5-177">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-177">Int32</span></span>|<span data-ttu-id="1e4b5-178">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-178">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="1e4b5-179">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="1e4b5-179">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1e4b5-180">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-180">passwordRequiredType</span></span>|[<span data-ttu-id="1e4b5-181">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-181">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="1e4b5-182">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-182">Type of password that is required.</span></span> <span data-ttu-id="1e4b5-183">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-183">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1e4b5-184">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-184">workProfileDataSharingType</span></span>|[<span data-ttu-id="1e4b5-185">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-185">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="1e4b5-186">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-186">Type of data sharing that is allowed.</span></span> <span data-ttu-id="1e4b5-187">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-187">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="1e4b5-188">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="1e4b5-188">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="1e4b5-189">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-189">Boolean</span></span>|<span data-ttu-id="1e4b5-190">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-190">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="1e4b5-191">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="1e4b5-191">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="1e4b5-192">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-192">Boolean</span></span>|<span data-ttu-id="1e4b5-193">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-193">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="1e4b5-194">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="1e4b5-194">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="1e4b5-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-195">Boolean</span></span>|<span data-ttu-id="1e4b5-196">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-196">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="1e4b5-197">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="1e4b5-197">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="1e4b5-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-198">Boolean</span></span>|<span data-ttu-id="1e4b5-199">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-199">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="1e4b5-200">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="1e4b5-200">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="1e4b5-201">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-201">Boolean</span></span>|<span data-ttu-id="1e4b5-202">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-202">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="1e4b5-203">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="1e4b5-203">workProfileBlockCamera</span></span>|<span data-ttu-id="1e4b5-204">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-204">Boolean</span></span>|<span data-ttu-id="1e4b5-205">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-205">Block work profile camera.</span></span>|
|<span data-ttu-id="1e4b5-206">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="1e4b5-206">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="1e4b5-207">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-207">Boolean</span></span>|<span data-ttu-id="1e4b5-208">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-208">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="1e4b5-209">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="1e4b5-209">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="1e4b5-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-210">Boolean</span></span>|<span data-ttu-id="1e4b5-211">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-211">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="1e4b5-212">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="1e4b5-212">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="1e4b5-213">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-213">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="1e4b5-214">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-214">Type of password that is required.</span></span> <span data-ttu-id="1e4b5-215">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-215">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="1e4b5-216">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="1e4b5-216">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="1e4b5-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-217">Boolean</span></span>|<span data-ttu-id="1e4b5-218">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-218">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="1e4b5-219">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="1e4b5-219">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="1e4b5-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-220">Boolean</span></span>|<span data-ttu-id="1e4b5-221">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-221">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="1e4b5-222">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="1e4b5-222">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="1e4b5-223">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-223">Int32</span></span>|<span data-ttu-id="1e4b5-224">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-224">Number of days before the work profile password expires.</span></span> <span data-ttu-id="1e4b5-225">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="1e4b5-225">Valid values 1 to 365</span></span>|
|<span data-ttu-id="1e4b5-226">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="1e4b5-226">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="1e4b5-227">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-227">Int32</span></span>|<span data-ttu-id="1e4b5-228">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-228">Minimum length of work profile password.</span></span> <span data-ttu-id="1e4b5-229">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="1e4b5-229">Valid values 4 to 16</span></span>|
|<span data-ttu-id="1e4b5-230">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="1e4b5-230">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="1e4b5-231">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-231">Int32</span></span>|<span data-ttu-id="1e4b5-232">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-232">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="1e4b5-233">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1e4b5-233">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e4b5-234">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1e4b5-234">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="1e4b5-235">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-235">Int32</span></span>|<span data-ttu-id="1e4b5-236">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-236">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="1e4b5-237">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1e4b5-237">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e4b5-238">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="1e4b5-238">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="1e4b5-239">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-239">Int32</span></span>|<span data-ttu-id="1e4b5-240">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-240">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="1e4b5-241">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1e4b5-241">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e4b5-242">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1e4b5-242">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="1e4b5-243">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-243">Int32</span></span>|<span data-ttu-id="1e4b5-244">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-244">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="1e4b5-245">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1e4b5-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e4b5-246">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="1e4b5-246">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="1e4b5-247">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-247">Int32</span></span>|<span data-ttu-id="1e4b5-248">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-248">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="1e4b5-249">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1e4b5-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e4b5-250">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="1e4b5-250">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="1e4b5-251">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-251">Int32</span></span>|<span data-ttu-id="1e4b5-252">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-252">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="1e4b5-253">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="1e4b5-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="1e4b5-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="1e4b5-254">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="1e4b5-255">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-255">Int32</span></span>|<span data-ttu-id="1e4b5-256">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-256">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="1e4b5-257">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="1e4b5-257">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="1e4b5-258">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-258">Int32</span></span>|<span data-ttu-id="1e4b5-259">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-259">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="1e4b5-260">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="1e4b5-260">Valid values 0 to 24</span></span>|
|<span data-ttu-id="1e4b5-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="1e4b5-261">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="1e4b5-262">Int32</span><span class="sxs-lookup"><span data-stu-id="1e4b5-262">Int32</span></span>|<span data-ttu-id="1e4b5-263">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-263">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="1e4b5-264">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="1e4b5-264">Valid values 1 to 16</span></span>|
|<span data-ttu-id="1e4b5-265">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-265">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="1e4b5-266">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="1e4b5-266">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="1e4b5-267">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-267">Type of work profile password that is required.</span></span> <span data-ttu-id="1e4b5-268">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-268">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="1e4b5-269">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="1e4b5-269">workProfileRequirePassword</span></span>|<span data-ttu-id="1e4b5-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-270">Boolean</span></span>|<span data-ttu-id="1e4b5-271">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="1e4b5-271">Password is required or not for work profile</span></span>|
|<span data-ttu-id="1e4b5-272">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="1e4b5-272">securityRequireVerifyApps</span></span>|<span data-ttu-id="1e4b5-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e4b5-273">Boolean</span></span>|<span data-ttu-id="1e4b5-274">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-274">Require the Android Verify apps feature is turned on.</span></span>|



## <a name="response"></a><span data-ttu-id="1e4b5-275">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4b5-275">Response</span></span>
<span data-ttu-id="1e4b5-276">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [entidadeandroidforworkprofiledeviceconfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-276">If successful, this method returns a `201 Created` response code and a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1e4b5-277">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1e4b5-277">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e4b5-278">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1e4b5-278">Request</span></span>
<span data-ttu-id="1e4b5-279">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-279">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1e4b5-280">Resposta</span><span class="sxs-lookup"><span data-stu-id="1e4b5-280">Response</span></span>
<span data-ttu-id="1e4b5-p126">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1e4b5-p126">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



