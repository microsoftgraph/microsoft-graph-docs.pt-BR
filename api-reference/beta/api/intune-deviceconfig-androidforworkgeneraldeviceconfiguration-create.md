---
title: Criar androidForWorkGeneralDeviceConfiguration
description: Crie um novo objeto de androidForWorkGeneralDeviceConfiguration.
ms.openlocfilehash: e04f2071fff39e8030d38203d3c2fc8bb550ac48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039398"
---
# <a name="create-androidforworkgeneraldeviceconfiguration"></a><span data-ttu-id="f0aac-103">Criar androidForWorkGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f0aac-103">Create androidForWorkGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f0aac-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f0aac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0aac-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f0aac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f0aac-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f0aac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f0aac-107">Crie um novo objeto de [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f0aac-107">Create a new [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f0aac-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0aac-108">Prerequisites</span></span>
<span data-ttu-id="f0aac-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0aac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0aac-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0aac-111">Permission type</span></span>|<span data-ttu-id="f0aac-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0aac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0aac-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0aac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f0aac-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0aac-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f0aac-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0aac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0aac-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0aac-116">Not supported.</span></span>|
|<span data-ttu-id="f0aac-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f0aac-117">Application</span></span>|<span data-ttu-id="f0aac-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0aac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0aac-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0aac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="f0aac-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aac-120">Request headers</span></span>
|<span data-ttu-id="f0aac-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0aac-121">Header</span></span>|<span data-ttu-id="f0aac-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f0aac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0aac-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0aac-123">Authorization</span></span>|<span data-ttu-id="f0aac-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0aac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0aac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f0aac-125">Accept</span></span>|<span data-ttu-id="f0aac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f0aac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0aac-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aac-127">Request body</span></span>
<span data-ttu-id="f0aac-128">No corpo da solicitação, fornece uma representação JSON para o objeto androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0aac-128">In the request body, supply a JSON representation for the androidForWorkGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="f0aac-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o androidForWorkGeneralDeviceConfiguration.</span><span class="sxs-lookup"><span data-stu-id="f0aac-129">The following table shows the properties that are required when you create the androidForWorkGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="f0aac-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0aac-130">Property</span></span>|<span data-ttu-id="f0aac-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0aac-131">Type</span></span>|<span data-ttu-id="f0aac-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0aac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0aac-133">id</span><span class="sxs-lookup"><span data-stu-id="f0aac-133">id</span></span>|<span data-ttu-id="f0aac-134">String</span><span class="sxs-lookup"><span data-stu-id="f0aac-134">String</span></span>|<span data-ttu-id="f0aac-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0aac-135">Key of the entity.</span></span> <span data-ttu-id="f0aac-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f0aac-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f0aac-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0aac-138">DateTimeOffset</span></span>|<span data-ttu-id="f0aac-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f0aac-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f0aac-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f0aac-141">roleScopeTagIds</span></span>|<span data-ttu-id="f0aac-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f0aac-142">String collection</span></span>|<span data-ttu-id="f0aac-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f0aac-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f0aac-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f0aac-145">supportsScopeTags</span></span>|<span data-ttu-id="f0aac-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-146">Boolean</span></span>|<span data-ttu-id="f0aac-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f0aac-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f0aac-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f0aac-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f0aac-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f0aac-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f0aac-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f0aac-150">This property is read-only.</span></span> <span data-ttu-id="f0aac-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f0aac-152">createdDateTime</span></span>|<span data-ttu-id="f0aac-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f0aac-153">DateTimeOffset</span></span>|<span data-ttu-id="f0aac-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f0aac-154">DateTime the object was created.</span></span> <span data-ttu-id="f0aac-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-156">description</span><span class="sxs-lookup"><span data-stu-id="f0aac-156">description</span></span>|<span data-ttu-id="f0aac-157">String</span><span class="sxs-lookup"><span data-stu-id="f0aac-157">String</span></span>|<span data-ttu-id="f0aac-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0aac-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f0aac-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f0aac-160">displayName</span></span>|<span data-ttu-id="f0aac-161">String</span><span class="sxs-lookup"><span data-stu-id="f0aac-161">String</span></span>|<span data-ttu-id="f0aac-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0aac-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f0aac-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-164">version</span><span class="sxs-lookup"><span data-stu-id="f0aac-164">version</span></span>|<span data-ttu-id="f0aac-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-165">Int32</span></span>|<span data-ttu-id="f0aac-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f0aac-166">Version of the device configuration.</span></span> <span data-ttu-id="f0aac-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f0aac-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f0aac-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f0aac-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f0aac-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-169">Boolean</span></span>|<span data-ttu-id="f0aac-170">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f0aac-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f0aac-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="f0aac-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="f0aac-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-172">Boolean</span></span>|<span data-ttu-id="f0aac-173">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="f0aac-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="f0aac-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f0aac-174">passwordExpirationDays</span></span>|<span data-ttu-id="f0aac-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-175">Int32</span></span>|<span data-ttu-id="f0aac-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f0aac-176">Number of days before the password expires.</span></span> <span data-ttu-id="f0aac-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="f0aac-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f0aac-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f0aac-178">passwordMinimumLength</span></span>|<span data-ttu-id="f0aac-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-179">Int32</span></span>|<span data-ttu-id="f0aac-180">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="f0aac-180">Minimum length of passwords.</span></span> <span data-ttu-id="f0aac-181">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="f0aac-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f0aac-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f0aac-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f0aac-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-183">Int32</span></span>|<span data-ttu-id="f0aac-184">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f0aac-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f0aac-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f0aac-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f0aac-186">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-186">Int32</span></span>|<span data-ttu-id="f0aac-187">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f0aac-187">Number of previous passwords to block.</span></span> <span data-ttu-id="f0aac-188">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f0aac-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f0aac-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f0aac-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f0aac-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-190">Int32</span></span>|<span data-ttu-id="f0aac-191">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="f0aac-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="f0aac-192">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="f0aac-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f0aac-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f0aac-193">passwordRequiredType</span></span>|[<span data-ttu-id="f0aac-194">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f0aac-194">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="f0aac-195">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f0aac-195">Type of password that is required.</span></span> <span data-ttu-id="f0aac-196">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="f0aac-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f0aac-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="f0aac-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="f0aac-198">androidForWorkCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="f0aac-198">androidForWorkCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidforworkcrossprofiledatasharingtype.md)|<span data-ttu-id="f0aac-199">Tipo de dados de compartilhamento que é permitido.</span><span class="sxs-lookup"><span data-stu-id="f0aac-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="f0aac-200">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="f0aac-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="f0aac-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="f0aac-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="f0aac-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-202">Boolean</span></span>|<span data-ttu-id="f0aac-203">Indica se deve ou não bloquear notificações de dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f0aac-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="f0aac-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="f0aac-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="f0aac-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-205">Boolean</span></span>|<span data-ttu-id="f0aac-206">Impedir que os usuários de adicionar/remover contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="f0aac-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="f0aac-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="f0aac-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-208">Boolean</span></span>|<span data-ttu-id="f0aac-209">Permitir que os dispositivos bluetooth acessar contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0aac-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="f0aac-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f0aac-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="f0aac-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-211">Boolean</span></span>|<span data-ttu-id="f0aac-212">Captura de tela de bloqueio no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="f0aac-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="f0aac-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="f0aac-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-214">Boolean</span></span>|<span data-ttu-id="f0aac-215">Bloquear exibição trabalho perfil ID do chamador no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="f0aac-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="f0aac-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="f0aac-216">workProfileBlockCamera</span></span>|<span data-ttu-id="f0aac-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-217">Boolean</span></span>|<span data-ttu-id="f0aac-218">Câmera de perfil de trabalho de bloco.</span><span class="sxs-lookup"><span data-stu-id="f0aac-218">Block work profile camera.</span></span>|
|<span data-ttu-id="f0aac-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="f0aac-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="f0aac-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-220">Boolean</span></span>|<span data-ttu-id="f0aac-221">Disponibilidade do bloco trabalho perfil contatos no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="f0aac-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="f0aac-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="f0aac-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="f0aac-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-223">Boolean</span></span>|<span data-ttu-id="f0aac-224">Boolean que indica se a configuração não permitir cruzado perfil copiar/colar está habilitada.</span><span class="sxs-lookup"><span data-stu-id="f0aac-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="f0aac-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="f0aac-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="f0aac-226">androidForWorkDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="f0aac-226">androidForWorkDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidforworkdefaultapppermissionpolicytype.md)|<span data-ttu-id="f0aac-227">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f0aac-227">Type of password that is required.</span></span> <span data-ttu-id="f0aac-228">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="f0aac-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="f0aac-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f0aac-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f0aac-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-230">Boolean</span></span>|<span data-ttu-id="f0aac-231">Indica se o bloqueio da impressão digital ou não desbloquear para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="f0aac-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="f0aac-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="f0aac-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-233">Boolean</span></span>|<span data-ttu-id="f0aac-234">Indica se deve ou não bloquear bloqueio inteligente e outros operadores de confiabilidade para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="f0aac-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f0aac-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="f0aac-236">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-236">Int32</span></span>|<span data-ttu-id="f0aac-237">Número de dias até a senha do perfil de trabalho expira.</span><span class="sxs-lookup"><span data-stu-id="f0aac-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="f0aac-238">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="f0aac-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f0aac-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f0aac-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="f0aac-240">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-240">Int32</span></span>|<span data-ttu-id="f0aac-241">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-241">Minimum length of work profile password.</span></span> <span data-ttu-id="f0aac-242">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="f0aac-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f0aac-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="f0aac-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="f0aac-244">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-244">Int32</span></span>|<span data-ttu-id="f0aac-245">Número mínimo de caracteres numéricos necessários em senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="f0aac-246">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f0aac-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f0aac-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f0aac-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="f0aac-248">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-248">Int32</span></span>|<span data-ttu-id="f0aac-249">Número mínimo de caracteres não alfabéticos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="f0aac-250">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f0aac-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f0aac-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f0aac-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="f0aac-252">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-252">Int32</span></span>|<span data-ttu-id="f0aac-253">Número mínimo de caracteres de carta necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="f0aac-254">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f0aac-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f0aac-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f0aac-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="f0aac-256">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-256">Int32</span></span>|<span data-ttu-id="f0aac-257">Número mínimo de caracteres minúscula necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="f0aac-258">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f0aac-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f0aac-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f0aac-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="f0aac-260">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-260">Int32</span></span>|<span data-ttu-id="f0aac-261">Número mínimo de caracteres de maiusculas necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="f0aac-262">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f0aac-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f0aac-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="f0aac-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="f0aac-264">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-264">Int32</span></span>|<span data-ttu-id="f0aac-265">Número mínimo de símbolos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f0aac-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="f0aac-266">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f0aac-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f0aac-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f0aac-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f0aac-268">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-268">Int32</span></span>|<span data-ttu-id="f0aac-269">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f0aac-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f0aac-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f0aac-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f0aac-271">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-271">Int32</span></span>|<span data-ttu-id="f0aac-272">Número de senhas anteriores de perfil de trabalho para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f0aac-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="f0aac-273">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f0aac-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f0aac-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f0aac-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f0aac-275">Int32</span><span class="sxs-lookup"><span data-stu-id="f0aac-275">Int32</span></span>|<span data-ttu-id="f0aac-276">Número de falhas permitidas antes que o perfil de trabalho é removido e todos os dados corporativos excluídos de entrada.</span><span class="sxs-lookup"><span data-stu-id="f0aac-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="f0aac-277">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="f0aac-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f0aac-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f0aac-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="f0aac-279">androidForWorkRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f0aac-279">androidForWorkRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidforworkrequiredpasswordtype.md)|<span data-ttu-id="f0aac-280">Tipo de senha de perfil de trabalho que é necessário.</span><span class="sxs-lookup"><span data-stu-id="f0aac-280">Type of work profile password that is required.</span></span> <span data-ttu-id="f0aac-281">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="f0aac-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f0aac-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="f0aac-282">workProfileRequirePassword</span></span>|<span data-ttu-id="f0aac-283">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-283">Boolean</span></span>|<span data-ttu-id="f0aac-284">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="f0aac-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="f0aac-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f0aac-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="f0aac-286">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-286">Boolean</span></span>|<span data-ttu-id="f0aac-287">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="f0aac-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f0aac-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="f0aac-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="f0aac-289">String</span><span class="sxs-lookup"><span data-stu-id="f0aac-289">String</span></span>|<span data-ttu-id="f0aac-290">Habilite o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="f0aac-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="f0aac-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="f0aac-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="f0aac-292">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0aac-292">Boolean</span></span>|<span data-ttu-id="f0aac-293">Habilite o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="f0aac-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="f0aac-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aac-294">Response</span></span>
<span data-ttu-id="f0aac-295">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0aac-295">If successful, this method returns a `201 Created` response code and a [androidForWorkGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidforworkgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0aac-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0aac-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="f0aac-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0aac-297">Request</span></span>
<span data-ttu-id="f0aac-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0aac-298">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 2102

{
  "@odata.type": "#microsoft.graph.androidForWorkGeneralDeviceConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
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

### <a name="response"></a><span data-ttu-id="f0aac-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0aac-299">Response</span></span>
<span data-ttu-id="f0aac-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0aac-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





