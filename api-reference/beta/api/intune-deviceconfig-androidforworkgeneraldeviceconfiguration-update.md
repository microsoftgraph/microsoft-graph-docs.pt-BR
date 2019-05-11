---
title: Atualizar androidForWorkGeneralDeviceConfiguration
description: Atualiza as propriedades de um objeto androidForWorkGeneralDeviceConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1159ab365d927e7a506bd42951b1c89dff0e30cf
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933435"
---
# <a name="update-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="95478-103">Atualizar androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="95478-103">Update androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="95478-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="95478-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95478-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="95478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95478-106">Atualiza as propriedades de um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="95478-106">Update the properties of a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95478-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="95478-107">Prerequisites</span></span>
<span data-ttu-id="95478-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="95478-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95478-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="95478-110">Permission type</span></span>|<span data-ttu-id="95478-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="95478-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95478-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="95478-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95478-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95478-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95478-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="95478-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95478-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95478-115">Not supported.</span></span>|
|<span data-ttu-id="95478-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="95478-116">Application</span></span>|<span data-ttu-id="95478-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="95478-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="95478-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="95478-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="95478-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="95478-119">Request headers</span></span>
|<span data-ttu-id="95478-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="95478-120">Header</span></span>|<span data-ttu-id="95478-121">Valor</span><span class="sxs-lookup"><span data-stu-id="95478-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95478-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="95478-122">Authorization</span></span>|<span data-ttu-id="95478-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="95478-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95478-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="95478-124">Accept</span></span>|<span data-ttu-id="95478-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95478-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95478-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="95478-126">Request body</span></span>
<span data-ttu-id="95478-127">No corpo da solicitação, forneça uma representação JSON do objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="95478-127">In the request body, supply a JSON representation for the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="95478-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="95478-128">The following table shows the properties that are required when you create the [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="95478-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="95478-129">Property</span></span>|<span data-ttu-id="95478-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="95478-130">Type</span></span>|<span data-ttu-id="95478-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="95478-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95478-132">id</span><span class="sxs-lookup"><span data-stu-id="95478-132">id</span></span>|<span data-ttu-id="95478-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95478-133">String</span></span>|<span data-ttu-id="95478-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="95478-134">Key of the entity.</span></span> <span data-ttu-id="95478-135">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95478-136">lastModifiedDateTime</span></span>|<span data-ttu-id="95478-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95478-137">DateTimeOffset</span></span>|<span data-ttu-id="95478-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="95478-138">DateTime the object was last modified.</span></span> <span data-ttu-id="95478-139">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="95478-140">roleScopeTagIds</span></span>|<span data-ttu-id="95478-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="95478-141">String collection</span></span>|<span data-ttu-id="95478-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="95478-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="95478-143">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="95478-144">supportsScopeTags</span></span>|<span data-ttu-id="95478-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-145">Boolean</span></span>|<span data-ttu-id="95478-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="95478-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="95478-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="95478-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="95478-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="95478-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="95478-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="95478-149">This property is read-only.</span></span> <span data-ttu-id="95478-150">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95478-151">createdDateTime</span></span>|<span data-ttu-id="95478-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95478-152">DateTimeOffset</span></span>|<span data-ttu-id="95478-153">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="95478-153">DateTime the object was created.</span></span> <span data-ttu-id="95478-154">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-155">description</span><span class="sxs-lookup"><span data-stu-id="95478-155">description</span></span>|<span data-ttu-id="95478-156">String</span><span class="sxs-lookup"><span data-stu-id="95478-156">String</span></span>|<span data-ttu-id="95478-157">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95478-157">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="95478-158">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-158">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-159">displayName</span><span class="sxs-lookup"><span data-stu-id="95478-159">displayName</span></span>|<span data-ttu-id="95478-160">String</span><span class="sxs-lookup"><span data-stu-id="95478-160">String</span></span>|<span data-ttu-id="95478-161">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95478-161">Admin provided name of the device configuration.</span></span> <span data-ttu-id="95478-162">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-162">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-163">versão</span><span class="sxs-lookup"><span data-stu-id="95478-163">version</span></span>|<span data-ttu-id="95478-164">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-164">Int32</span></span>|<span data-ttu-id="95478-165">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="95478-165">Version of the device configuration.</span></span> <span data-ttu-id="95478-166">Herdada de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="95478-166">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="95478-167">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="95478-167">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="95478-168">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-168">Boolean</span></span>|<span data-ttu-id="95478-169">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95478-169">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="95478-170">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="95478-170">passwordBlockTrustAgents</span></span>|<span data-ttu-id="95478-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="95478-171">Boolean</span></span>|<span data-ttu-id="95478-172">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="95478-172">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="95478-173">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="95478-173">passwordExpirationDays</span></span>|<span data-ttu-id="95478-174">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-174">Int32</span></span>|<span data-ttu-id="95478-175">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="95478-175">Number of days before the password expires.</span></span> <span data-ttu-id="95478-176">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="95478-176">Valid values 1 to 365</span></span>|
|<span data-ttu-id="95478-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="95478-177">passwordMinimumLength</span></span>|<span data-ttu-id="95478-178">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-178">Int32</span></span>|<span data-ttu-id="95478-179">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="95478-179">Minimum length of passwords.</span></span> <span data-ttu-id="95478-180">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="95478-180">Valid values 4 to 16</span></span>|
|<span data-ttu-id="95478-181">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="95478-181">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="95478-182">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-182">Int32</span></span>|<span data-ttu-id="95478-183">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="95478-183">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="95478-184">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="95478-184">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="95478-185">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-185">Int32</span></span>|<span data-ttu-id="95478-186">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="95478-186">Number of previous passwords to block.</span></span> <span data-ttu-id="95478-187">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="95478-187">Valid values 0 to 24</span></span>|
|<span data-ttu-id="95478-188">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="95478-188">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="95478-189">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-189">Int32</span></span>|<span data-ttu-id="95478-190">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="95478-190">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="95478-191">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="95478-191">Valid values 1 to 16</span></span>|
|<span data-ttu-id="95478-192">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="95478-192">passwordRequiredType</span></span>|[<span data-ttu-id="95478-193">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="95478-193">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="95478-194">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="95478-194">Type of password that is required.</span></span> <span data-ttu-id="95478-195">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="95478-195">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="95478-196">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="95478-196">workProfileDataSharingType</span></span>|[<span data-ttu-id="95478-197">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="95478-197">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="95478-198">Tipo de compartilhamento de dados permitido.</span><span class="sxs-lookup"><span data-stu-id="95478-198">Type of data sharing that is allowed.</span></span> <span data-ttu-id="95478-199">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="95478-199">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="95478-200">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="95478-200">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="95478-201">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-201">Boolean</span></span>|<span data-ttu-id="95478-202">Indica se as notificações devem ou não ser bloqueadas enquanto o dispositivo estiver bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95478-202">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="95478-203">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="95478-203">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="95478-204">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-204">Boolean</span></span>|<span data-ttu-id="95478-205">Impedir que os usuários adicionem/removam contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-205">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="95478-206">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="95478-206">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="95478-207">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-207">Boolean</span></span>|<span data-ttu-id="95478-208">Permitir que dispositivos Bluetooth acessem contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="95478-208">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="95478-209">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="95478-209">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="95478-210">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-210">Boolean</span></span>|<span data-ttu-id="95478-211">Bloquear captura de tela em perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-211">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="95478-212">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="95478-212">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="95478-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-213">Boolean</span></span>|<span data-ttu-id="95478-214">Bloquear exibir ID de chamadas de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="95478-214">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="95478-215">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="95478-215">workProfileBlockCamera</span></span>|<span data-ttu-id="95478-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-216">Boolean</span></span>|<span data-ttu-id="95478-217">Bloquear câmera de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-217">Block work profile camera.</span></span>|
|<span data-ttu-id="95478-218">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="95478-218">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="95478-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-219">Boolean</span></span>|<span data-ttu-id="95478-220">Bloquear disponibilidade de contatos de perfil de trabalho no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="95478-220">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="95478-221">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="95478-221">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="95478-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-222">Boolean</span></span>|<span data-ttu-id="95478-223">Booliano que indica se a configuração de desautorizar a cópia/colagem entre perfis está habilitada.</span><span class="sxs-lookup"><span data-stu-id="95478-223">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="95478-224">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="95478-224">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="95478-225">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="95478-225">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="95478-226">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="95478-226">Type of password that is required.</span></span> <span data-ttu-id="95478-227">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="95478-227">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="95478-228">Propriedades workprofilepasswordblockfingerprintunlock</span><span class="sxs-lookup"><span data-stu-id="95478-228">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="95478-229">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-229">Boolean</span></span>|<span data-ttu-id="95478-230">Indica se o desbloqueio de impressão digital para o perfil de trabalho deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="95478-230">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="95478-231">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="95478-231">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="95478-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-232">Boolean</span></span>|<span data-ttu-id="95478-233">Indica se o bloqueio inteligente e outros agentes de confiança devem ou não ser bloqueados para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-233">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="95478-234">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="95478-234">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="95478-235">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-235">Int32</span></span>|<span data-ttu-id="95478-236">Número de dias antes da senha do perfil de trabalho expirar.</span><span class="sxs-lookup"><span data-stu-id="95478-236">Number of days before the work profile password expires.</span></span> <span data-ttu-id="95478-237">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="95478-237">Valid values 1 to 365</span></span>|
|<span data-ttu-id="95478-238">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="95478-238">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="95478-239">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-239">Int32</span></span>|<span data-ttu-id="95478-240">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-240">Minimum length of work profile password.</span></span> <span data-ttu-id="95478-241">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="95478-241">Valid values 4 to 16</span></span>|
|<span data-ttu-id="95478-242">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="95478-242">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="95478-243">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-243">Int32</span></span>|<span data-ttu-id="95478-244">Mínimo de caracteres numéricos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-244">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="95478-245">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="95478-245">Valid values 1 to 10</span></span>|
|<span data-ttu-id="95478-246">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="95478-246">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="95478-247">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-247">Int32</span></span>|<span data-ttu-id="95478-248">Número mínimo de caracteres não carta necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-248">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="95478-249">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="95478-249">Valid values 1 to 10</span></span>|
|<span data-ttu-id="95478-250">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="95478-250">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="95478-251">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-251">Int32</span></span>|<span data-ttu-id="95478-252">Número mínimo de caracteres de letras necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-252">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="95478-253">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="95478-253">Valid values 1 to 10</span></span>|
|<span data-ttu-id="95478-254">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="95478-254">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="95478-255">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-255">Int32</span></span>|<span data-ttu-id="95478-256">Número mínimo de caracteres em minúsculas exigidos na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-256">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="95478-257">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="95478-257">Valid values 1 to 10</span></span>|
|<span data-ttu-id="95478-258">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="95478-258">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="95478-259">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-259">Int32</span></span>|<span data-ttu-id="95478-260">Número mínimo de caracteres em maiúsculas obrigatórios na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-260">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="95478-261">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="95478-261">Valid values 1 to 10</span></span>|
|<span data-ttu-id="95478-262">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="95478-262">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="95478-263">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-263">Int32</span></span>|<span data-ttu-id="95478-264">Número mínimo de símbolos necessários na senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="95478-264">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="95478-265">Valores válidos de 1 a 10</span><span class="sxs-lookup"><span data-stu-id="95478-265">Valid values 1 to 10</span></span>|
|<span data-ttu-id="95478-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="95478-266">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="95478-267">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-267">Int32</span></span>|<span data-ttu-id="95478-268">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="95478-268">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="95478-269">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="95478-269">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="95478-270">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-270">Int32</span></span>|<span data-ttu-id="95478-271">Número de senhas de perfil de trabalho anteriores a serem bloqueadas.</span><span class="sxs-lookup"><span data-stu-id="95478-271">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="95478-272">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="95478-272">Valid values 0 to 24</span></span>|
|<span data-ttu-id="95478-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="95478-273">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="95478-274">Int32</span><span class="sxs-lookup"><span data-stu-id="95478-274">Int32</span></span>|<span data-ttu-id="95478-275">Número de falhas de entrada permitidas antes que o perfil de trabalho seja removido e todos os dados corporativos excluídos.</span><span class="sxs-lookup"><span data-stu-id="95478-275">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="95478-276">Valores válidos de 1 a 16</span><span class="sxs-lookup"><span data-stu-id="95478-276">Valid values 1 to 16</span></span>|
|<span data-ttu-id="95478-277">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="95478-277">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="95478-278">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="95478-278">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="95478-279">Tipo de senha de perfil de trabalho necessário.</span><span class="sxs-lookup"><span data-stu-id="95478-279">Type of work profile password that is required.</span></span> <span data-ttu-id="95478-280">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="95478-280">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="95478-281">Workprofilerequirepassword foram adicionadas</span><span class="sxs-lookup"><span data-stu-id="95478-281">workProfileRequirePassword</span></span>|<span data-ttu-id="95478-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-282">Boolean</span></span>|<span data-ttu-id="95478-283">A senha é obrigatória ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="95478-283">Password is required or not for work profile</span></span>|
|<span data-ttu-id="95478-284">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="95478-284">securityRequireVerifyApps</span></span>|<span data-ttu-id="95478-285">Boolean</span><span class="sxs-lookup"><span data-stu-id="95478-285">Boolean</span></span>|<span data-ttu-id="95478-286">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="95478-286">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="95478-287">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="95478-287">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="95478-288">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="95478-288">String</span></span>|<span data-ttu-id="95478-289">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="95478-289">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="95478-290">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="95478-290">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="95478-291">Booliano</span><span class="sxs-lookup"><span data-stu-id="95478-291">Boolean</span></span>|<span data-ttu-id="95478-292">Habilitar o modo de bloqueio para VPN Always-on.</span><span class="sxs-lookup"><span data-stu-id="95478-292">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="95478-293">Resposta</span><span class="sxs-lookup"><span data-stu-id="95478-293">Response</span></span>
<span data-ttu-id="95478-294">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="95478-294">If successful, this method returns a `200 OK` response code and an updated [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95478-295">Exemplo</span><span class="sxs-lookup"><span data-stu-id="95478-295">Example</span></span>

### <a name="request"></a><span data-ttu-id="95478-296">Solicitação</span><span class="sxs-lookup"><span data-stu-id="95478-296">Request</span></span>
<span data-ttu-id="95478-297">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="95478-297">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2038

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```

### <a name="response"></a><span data-ttu-id="95478-298">Resposta</span><span class="sxs-lookup"><span data-stu-id="95478-298">Response</span></span>
<span data-ttu-id="95478-p128">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="95478-p128">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2210

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "id": "a931a366-a366-a931-66a3-31a966a331a9",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
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
  "securityRequireVerifyApps": true,
  "vpnAlwaysOnPackageIdentifier": "Vpn Always On Package Identifier value",
  "vpnEnableAlwaysOnLockdownMode": true
}
```




