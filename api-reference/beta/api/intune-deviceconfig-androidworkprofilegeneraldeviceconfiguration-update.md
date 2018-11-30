---
title: Atualizar androidWorkProfileGeneralDeviceConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileGeneralDeviceConfiguration.
ms.openlocfilehash: 002a4008f4e4b40ef733df486a87d9b2f2f450b7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038078"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="f7cd2-103">Atualizar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="f7cd2-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="f7cd2-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f7cd2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f7cd2-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f7cd2-107">Atualize as propriedades de um objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7cd2-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f7cd2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f7cd2-108">Prerequisites</span></span>
<span data-ttu-id="f7cd2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f7cd2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7cd2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f7cd2-111">Permission type</span></span>|<span data-ttu-id="f7cd2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7cd2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f7cd2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7cd2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7cd2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7cd2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-116">Not supported.</span></span>|
|<span data-ttu-id="f7cd2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f7cd2-117">Application</span></span>|<span data-ttu-id="f7cd2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7cd2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f7cd2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="f7cd2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f7cd2-120">Request headers</span></span>
|<span data-ttu-id="f7cd2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f7cd2-121">Header</span></span>|<span data-ttu-id="f7cd2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f7cd2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7cd2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f7cd2-123">Authorization</span></span>|<span data-ttu-id="f7cd2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7cd2-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f7cd2-125">Accept</span></span>|<span data-ttu-id="f7cd2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f7cd2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7cd2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f7cd2-127">Request body</span></span>
<span data-ttu-id="f7cd2-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="f7cd2-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="f7cd2-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="f7cd2-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="f7cd2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f7cd2-130">Property</span></span>|<span data-ttu-id="f7cd2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f7cd2-131">Type</span></span>|<span data-ttu-id="f7cd2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f7cd2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7cd2-133">id</span><span class="sxs-lookup"><span data-stu-id="f7cd2-133">id</span></span>|<span data-ttu-id="f7cd2-134">String</span><span class="sxs-lookup"><span data-stu-id="f7cd2-134">String</span></span>|<span data-ttu-id="f7cd2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-135">Key of the entity.</span></span> <span data-ttu-id="f7cd2-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f7cd2-137">lastModifiedDateTime</span></span>|<span data-ttu-id="f7cd2-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7cd2-138">DateTimeOffset</span></span>|<span data-ttu-id="f7cd2-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-139">DateTime the object was last modified.</span></span> <span data-ttu-id="f7cd2-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="f7cd2-141">roleScopeTagIds</span></span>|<span data-ttu-id="f7cd2-142">String collection</span><span class="sxs-lookup"><span data-stu-id="f7cd2-142">String collection</span></span>|<span data-ttu-id="f7cd2-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="f7cd2-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="f7cd2-145">supportsScopeTags</span></span>|<span data-ttu-id="f7cd2-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-146">Boolean</span></span>|<span data-ttu-id="f7cd2-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="f7cd2-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="f7cd2-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="f7cd2-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-150">This property is read-only.</span></span> <span data-ttu-id="f7cd2-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f7cd2-152">createdDateTime</span></span>|<span data-ttu-id="f7cd2-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f7cd2-153">DateTimeOffset</span></span>|<span data-ttu-id="f7cd2-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-154">DateTime the object was created.</span></span> <span data-ttu-id="f7cd2-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-156">description</span><span class="sxs-lookup"><span data-stu-id="f7cd2-156">description</span></span>|<span data-ttu-id="f7cd2-157">String</span><span class="sxs-lookup"><span data-stu-id="f7cd2-157">String</span></span>|<span data-ttu-id="f7cd2-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="f7cd2-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-160">displayName</span><span class="sxs-lookup"><span data-stu-id="f7cd2-160">displayName</span></span>|<span data-ttu-id="f7cd2-161">String</span><span class="sxs-lookup"><span data-stu-id="f7cd2-161">String</span></span>|<span data-ttu-id="f7cd2-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="f7cd2-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-164">version</span><span class="sxs-lookup"><span data-stu-id="f7cd2-164">version</span></span>|<span data-ttu-id="f7cd2-165">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-165">Int32</span></span>|<span data-ttu-id="f7cd2-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-166">Version of the device configuration.</span></span> <span data-ttu-id="f7cd2-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="f7cd2-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="f7cd2-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f7cd2-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f7cd2-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-169">Boolean</span></span>|<span data-ttu-id="f7cd2-170">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="f7cd2-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="f7cd2-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="f7cd2-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-172">Boolean</span></span>|<span data-ttu-id="f7cd2-173">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="f7cd2-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f7cd2-174">passwordExpirationDays</span></span>|<span data-ttu-id="f7cd2-175">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-175">Int32</span></span>|<span data-ttu-id="f7cd2-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-176">Number of days before the password expires.</span></span> <span data-ttu-id="f7cd2-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="f7cd2-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f7cd2-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f7cd2-178">passwordMinimumLength</span></span>|<span data-ttu-id="f7cd2-179">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-179">Int32</span></span>|<span data-ttu-id="f7cd2-180">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-180">Minimum length of passwords.</span></span> <span data-ttu-id="f7cd2-181">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="f7cd2-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f7cd2-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f7cd2-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f7cd2-183">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-183">Int32</span></span>|<span data-ttu-id="f7cd2-184">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f7cd2-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f7cd2-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f7cd2-186">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-186">Int32</span></span>|<span data-ttu-id="f7cd2-187">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-187">Number of previous passwords to block.</span></span> <span data-ttu-id="f7cd2-188">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f7cd2-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f7cd2-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f7cd2-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f7cd2-190">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-190">Int32</span></span>|<span data-ttu-id="f7cd2-191">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="f7cd2-192">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="f7cd2-192">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f7cd2-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-193">passwordRequiredType</span></span>|[<span data-ttu-id="f7cd2-194">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-194">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="f7cd2-195">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-195">Type of password that is required.</span></span> <span data-ttu-id="f7cd2-196">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f7cd2-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="f7cd2-198">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-198">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="f7cd2-199">Tipo de dados de compartilhamento que é permitido.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="f7cd2-200">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="f7cd2-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="f7cd2-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="f7cd2-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-202">Boolean</span></span>|<span data-ttu-id="f7cd2-203">Indica se deve ou não bloquear notificações de dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="f7cd2-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="f7cd2-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="f7cd2-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-205">Boolean</span></span>|<span data-ttu-id="f7cd2-206">Impedir que os usuários de adicionar/remover contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="f7cd2-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="f7cd2-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="f7cd2-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-208">Boolean</span></span>|<span data-ttu-id="f7cd2-209">Permitir que os dispositivos bluetooth acessar contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="f7cd2-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="f7cd2-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="f7cd2-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-211">Boolean</span></span>|<span data-ttu-id="f7cd2-212">Captura de tela de bloqueio no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="f7cd2-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="f7cd2-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="f7cd2-214">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-214">Boolean</span></span>|<span data-ttu-id="f7cd2-215">Bloquear exibição trabalho perfil ID do chamador no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="f7cd2-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="f7cd2-216">workProfileBlockCamera</span></span>|<span data-ttu-id="f7cd2-217">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-217">Boolean</span></span>|<span data-ttu-id="f7cd2-218">Câmera de perfil de trabalho de bloco.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-218">Block work profile camera.</span></span>|
|<span data-ttu-id="f7cd2-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="f7cd2-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="f7cd2-220">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-220">Boolean</span></span>|<span data-ttu-id="f7cd2-221">Disponibilidade do bloco trabalho perfil contatos no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="f7cd2-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="f7cd2-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="f7cd2-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-223">Boolean</span></span>|<span data-ttu-id="f7cd2-224">Boolean que indica se a configuração não permitir cruzado perfil copiar/colar está habilitada.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="f7cd2-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="f7cd2-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="f7cd2-226">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-226">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="f7cd2-227">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-227">Type of password that is required.</span></span> <span data-ttu-id="f7cd2-228">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="f7cd2-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="f7cd2-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="f7cd2-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-230">Boolean</span></span>|<span data-ttu-id="f7cd2-231">Indica se o bloqueio da impressão digital ou não desbloquear para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="f7cd2-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="f7cd2-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="f7cd2-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-233">Boolean</span></span>|<span data-ttu-id="f7cd2-234">Indica se deve ou não bloquear bloqueio inteligente e outros operadores de confiabilidade para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="f7cd2-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="f7cd2-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="f7cd2-236">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-236">Int32</span></span>|<span data-ttu-id="f7cd2-237">Número de dias até a senha do perfil de trabalho expira.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="f7cd2-238">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="f7cd2-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="f7cd2-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="f7cd2-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="f7cd2-240">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-240">Int32</span></span>|<span data-ttu-id="f7cd2-241">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-241">Minimum length of work profile password.</span></span> <span data-ttu-id="f7cd2-242">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="f7cd2-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="f7cd2-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="f7cd2-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="f7cd2-244">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-244">Int32</span></span>|<span data-ttu-id="f7cd2-245">Número mínimo de caracteres numéricos necessários em senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="f7cd2-246">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f7cd2-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f7cd2-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f7cd2-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="f7cd2-248">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-248">Int32</span></span>|<span data-ttu-id="f7cd2-249">Número mínimo de caracteres não alfabéticos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="f7cd2-250">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f7cd2-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f7cd2-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="f7cd2-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="f7cd2-252">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-252">Int32</span></span>|<span data-ttu-id="f7cd2-253">Número mínimo de caracteres de carta necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="f7cd2-254">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f7cd2-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f7cd2-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f7cd2-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="f7cd2-256">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-256">Int32</span></span>|<span data-ttu-id="f7cd2-257">Número mínimo de caracteres minúscula necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="f7cd2-258">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f7cd2-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f7cd2-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="f7cd2-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="f7cd2-260">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-260">Int32</span></span>|<span data-ttu-id="f7cd2-261">Número mínimo de caracteres de maiusculas necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="f7cd2-262">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f7cd2-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f7cd2-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="f7cd2-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="f7cd2-264">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-264">Int32</span></span>|<span data-ttu-id="f7cd2-265">Número mínimo de símbolos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="f7cd2-266">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="f7cd2-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="f7cd2-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="f7cd2-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="f7cd2-268">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-268">Int32</span></span>|<span data-ttu-id="f7cd2-269">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="f7cd2-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="f7cd2-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="f7cd2-271">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-271">Int32</span></span>|<span data-ttu-id="f7cd2-272">Número de senhas anteriores de perfil de trabalho para bloquear.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="f7cd2-273">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="f7cd2-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="f7cd2-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="f7cd2-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="f7cd2-275">Int32</span><span class="sxs-lookup"><span data-stu-id="f7cd2-275">Int32</span></span>|<span data-ttu-id="f7cd2-276">Número de falhas permitidas antes que o perfil de trabalho é removido e todos os dados corporativos excluídos de entrada.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="f7cd2-277">Valores válidos de 4 a 11</span><span class="sxs-lookup"><span data-stu-id="f7cd2-277">Valid values 4 to 11</span></span>|
|<span data-ttu-id="f7cd2-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="f7cd2-279">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="f7cd2-279">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="f7cd2-280">Tipo de senha de perfil de trabalho que é necessário.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-280">Type of work profile password that is required.</span></span> <span data-ttu-id="f7cd2-281">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="f7cd2-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="f7cd2-282">workProfileRequirePassword</span></span>|<span data-ttu-id="f7cd2-283">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-283">Boolean</span></span>|<span data-ttu-id="f7cd2-284">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="f7cd2-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="f7cd2-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="f7cd2-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="f7cd2-286">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-286">Boolean</span></span>|<span data-ttu-id="f7cd2-287">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="f7cd2-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="f7cd2-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="f7cd2-289">String</span><span class="sxs-lookup"><span data-stu-id="f7cd2-289">String</span></span>|<span data-ttu-id="f7cd2-290">Habilite o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="f7cd2-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="f7cd2-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="f7cd2-292">Booliano</span><span class="sxs-lookup"><span data-stu-id="f7cd2-292">Boolean</span></span>|<span data-ttu-id="f7cd2-293">Habilite o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="f7cd2-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7cd2-294">Response</span></span>
<span data-ttu-id="f7cd2-295">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-295">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7cd2-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f7cd2-296">Example</span></span>
### <a name="request"></a><span data-ttu-id="f7cd2-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f7cd2-297">Request</span></span>
<span data-ttu-id="f7cd2-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2023

{
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

### <a name="response"></a><span data-ttu-id="f7cd2-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="f7cd2-299">Response</span></span>
<span data-ttu-id="f7cd2-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f7cd2-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2214

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
  "id": "6decda7e-da7e-6dec-7eda-ec6d7edaec6d",
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





