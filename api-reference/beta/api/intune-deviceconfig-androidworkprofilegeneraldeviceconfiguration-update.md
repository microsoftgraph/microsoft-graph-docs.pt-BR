---
title: Atualizar androidWorkProfileGeneralDeviceConfiguration
description: Atualize as propriedades de um objeto androidWorkProfileGeneralDeviceConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0cec0b230b9e8735b5071920ccba8639ea58de2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410032"
---
# <a name="update-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="c582b-103">Atualizar androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="c582b-103">Update androidWorkProfileGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="c582b-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c582b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c582b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c582b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c582b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c582b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c582b-107">Atualize as propriedades de um objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c582b-107">Update the properties of a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c582b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="c582b-108">Prerequisites</span></span>
<span data-ttu-id="c582b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="c582b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="c582b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="c582b-111">Permission type</span></span>|<span data-ttu-id="c582b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="c582b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c582b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="c582b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c582b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c582b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c582b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="c582b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c582b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c582b-116">Not supported.</span></span>|
|<span data-ttu-id="c582b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="c582b-117">Application</span></span>|<span data-ttu-id="c582b-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="c582b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c582b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="c582b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="c582b-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="c582b-120">Request headers</span></span>
|<span data-ttu-id="c582b-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="c582b-121">Header</span></span>|<span data-ttu-id="c582b-122">Valor</span><span class="sxs-lookup"><span data-stu-id="c582b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c582b-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="c582b-123">Authorization</span></span>|<span data-ttu-id="c582b-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="c582b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c582b-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="c582b-125">Accept</span></span>|<span data-ttu-id="c582b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c582b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c582b-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="c582b-127">Request body</span></span>
<span data-ttu-id="c582b-128">No corpo da solicitação, fornece uma representação JSON para o objeto [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) .</span><span class="sxs-lookup"><span data-stu-id="c582b-128">In the request body, supply a JSON representation for the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="c582b-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="c582b-129">The following table shows the properties that are required when you create the [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="c582b-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c582b-130">Property</span></span>|<span data-ttu-id="c582b-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="c582b-131">Type</span></span>|<span data-ttu-id="c582b-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="c582b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c582b-133">id</span><span class="sxs-lookup"><span data-stu-id="c582b-133">id</span></span>|<span data-ttu-id="c582b-134">String</span><span class="sxs-lookup"><span data-stu-id="c582b-134">String</span></span>|<span data-ttu-id="c582b-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="c582b-135">Key of the entity.</span></span> <span data-ttu-id="c582b-136">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-136">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c582b-137">lastModifiedDateTime</span></span>|<span data-ttu-id="c582b-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c582b-138">DateTimeOffset</span></span>|<span data-ttu-id="c582b-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="c582b-139">DateTime the object was last modified.</span></span> <span data-ttu-id="c582b-140">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-140">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="c582b-141">roleScopeTagIds</span></span>|<span data-ttu-id="c582b-142">String collection</span><span class="sxs-lookup"><span data-stu-id="c582b-142">String collection</span></span>|<span data-ttu-id="c582b-143">Lista de escopo marcas para essa instância da entidade.</span><span class="sxs-lookup"><span data-stu-id="c582b-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="c582b-144">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-144">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="c582b-145">supportsScopeTags</span></span>|<span data-ttu-id="c582b-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-146">Boolean</span></span>|<span data-ttu-id="c582b-147">Indica se ou não a configuração de dispositivo subjacente suporta a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="c582b-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="c582b-148">Atribuir à propriedade ScopeTags não é permitida quando esse valor for false e entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="c582b-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="c582b-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no Portal do Windows Azure.</span><span class="sxs-lookup"><span data-stu-id="c582b-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="c582b-150">Esta propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="c582b-150">This property is read-only.</span></span> <span data-ttu-id="c582b-151">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c582b-152">createdDateTime</span></span>|<span data-ttu-id="c582b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c582b-153">DateTimeOffset</span></span>|<span data-ttu-id="c582b-154">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="c582b-154">DateTime the object was created.</span></span> <span data-ttu-id="c582b-155">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-156">description</span><span class="sxs-lookup"><span data-stu-id="c582b-156">description</span></span>|<span data-ttu-id="c582b-157">String</span><span class="sxs-lookup"><span data-stu-id="c582b-157">String</span></span>|<span data-ttu-id="c582b-158">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c582b-158">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="c582b-159">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-159">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-160">displayName</span><span class="sxs-lookup"><span data-stu-id="c582b-160">displayName</span></span>|<span data-ttu-id="c582b-161">String</span><span class="sxs-lookup"><span data-stu-id="c582b-161">String</span></span>|<span data-ttu-id="c582b-162">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c582b-162">Admin provided name of the device configuration.</span></span> <span data-ttu-id="c582b-163">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-163">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-164">version</span><span class="sxs-lookup"><span data-stu-id="c582b-164">version</span></span>|<span data-ttu-id="c582b-165">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-165">Int32</span></span>|<span data-ttu-id="c582b-166">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="c582b-166">Version of the device configuration.</span></span> <span data-ttu-id="c582b-167">Herdado de [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="c582b-167">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="c582b-168">passwordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c582b-168">passwordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c582b-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-169">Boolean</span></span>|<span data-ttu-id="c582b-170">Indica se o desbloqueio de impressão digital deve ou não ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c582b-170">Indicates whether or not to block fingerprint unlock.</span></span>|
|<span data-ttu-id="c582b-171">passwordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c582b-171">passwordBlockTrustAgents</span></span>|<span data-ttu-id="c582b-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-172">Boolean</span></span>|<span data-ttu-id="c582b-173">Indica se o Smart Lock e outros agentes confiáveis devem ou não ser bloqueados.</span><span class="sxs-lookup"><span data-stu-id="c582b-173">Indicates whether or not to block Smart Lock and other trust agents.</span></span>|
|<span data-ttu-id="c582b-174">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c582b-174">passwordExpirationDays</span></span>|<span data-ttu-id="c582b-175">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-175">Int32</span></span>|<span data-ttu-id="c582b-176">Número de dias antes da expiração da senha.</span><span class="sxs-lookup"><span data-stu-id="c582b-176">Number of days before the password expires.</span></span> <span data-ttu-id="c582b-177">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="c582b-177">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c582b-178">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c582b-178">passwordMinimumLength</span></span>|<span data-ttu-id="c582b-179">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-179">Int32</span></span>|<span data-ttu-id="c582b-180">Comprimento mínimo das senhas.</span><span class="sxs-lookup"><span data-stu-id="c582b-180">Minimum length of passwords.</span></span> <span data-ttu-id="c582b-181">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="c582b-181">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c582b-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c582b-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c582b-183">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-183">Int32</span></span>|<span data-ttu-id="c582b-184">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="c582b-184">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c582b-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c582b-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c582b-186">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-186">Int32</span></span>|<span data-ttu-id="c582b-187">Número de senhas anteriores para bloquear.</span><span class="sxs-lookup"><span data-stu-id="c582b-187">Number of previous passwords to block.</span></span> <span data-ttu-id="c582b-188">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="c582b-188">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c582b-189">passwordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c582b-189">passwordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c582b-190">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-190">Int32</span></span>|<span data-ttu-id="c582b-191">Número permitido de falhas de entrada antes da redefinição de fábrica.</span><span class="sxs-lookup"><span data-stu-id="c582b-191">Number of sign in failures allowed before factory reset.</span></span> <span data-ttu-id="c582b-192">Valores válidos 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c582b-192">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c582b-193">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c582b-193">passwordRequiredType</span></span>|[<span data-ttu-id="c582b-194">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c582b-194">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="c582b-195">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="c582b-195">Type of password that is required.</span></span> <span data-ttu-id="c582b-196">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="c582b-196">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c582b-197">workProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="c582b-197">workProfileDataSharingType</span></span>|[<span data-ttu-id="c582b-198">androidWorkProfileCrossProfileDataSharingType</span><span class="sxs-lookup"><span data-stu-id="c582b-198">androidWorkProfileCrossProfileDataSharingType</span></span>](../resources/intune-deviceconfig-androidworkprofilecrossprofiledatasharingtype.md)|<span data-ttu-id="c582b-199">Tipo de dados de compartilhamento que é permitido.</span><span class="sxs-lookup"><span data-stu-id="c582b-199">Type of data sharing that is allowed.</span></span> <span data-ttu-id="c582b-200">Os valores possíveis são: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span><span class="sxs-lookup"><span data-stu-id="c582b-200">Possible values are: `deviceDefault`, `preventAny`, `allowPersonalToWork`, `noRestrictions`.</span></span>|
|<span data-ttu-id="c582b-201">workProfileBlockNotificationsWhileDeviceLocked</span><span class="sxs-lookup"><span data-stu-id="c582b-201">workProfileBlockNotificationsWhileDeviceLocked</span></span>|<span data-ttu-id="c582b-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-202">Boolean</span></span>|<span data-ttu-id="c582b-203">Indica se deve ou não bloquear notificações de dispositivo bloqueado.</span><span class="sxs-lookup"><span data-stu-id="c582b-203">Indicates whether or not to block notifications while device locked.</span></span>|
|<span data-ttu-id="c582b-204">workProfileBlockAddingAccounts</span><span class="sxs-lookup"><span data-stu-id="c582b-204">workProfileBlockAddingAccounts</span></span>|<span data-ttu-id="c582b-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-205">Boolean</span></span>|<span data-ttu-id="c582b-206">Impedir que os usuários de adicionar/remover contas no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-206">Block users from adding/removing accounts in work profile.</span></span>|
|<span data-ttu-id="c582b-207">workProfileBluetoothEnableContactSharing</span><span class="sxs-lookup"><span data-stu-id="c582b-207">workProfileBluetoothEnableContactSharing</span></span>|<span data-ttu-id="c582b-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-208">Boolean</span></span>|<span data-ttu-id="c582b-209">Permitir que os dispositivos bluetooth acessar contatos da empresa.</span><span class="sxs-lookup"><span data-stu-id="c582b-209">Allow bluetooth devices to access enterprise contacts.</span></span>|
|<span data-ttu-id="c582b-210">workProfileBlockScreenCapture</span><span class="sxs-lookup"><span data-stu-id="c582b-210">workProfileBlockScreenCapture</span></span>|<span data-ttu-id="c582b-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-211">Boolean</span></span>|<span data-ttu-id="c582b-212">Captura de tela de bloqueio no perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-212">Block screen capture in work profile.</span></span>|
|<span data-ttu-id="c582b-213">workProfileBlockCrossProfileCallerId</span><span class="sxs-lookup"><span data-stu-id="c582b-213">workProfileBlockCrossProfileCallerId</span></span>|<span data-ttu-id="c582b-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-214">Boolean</span></span>|<span data-ttu-id="c582b-215">Bloquear exibição trabalho perfil ID do chamador no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="c582b-215">Block display work profile caller ID in personal profile.</span></span>|
|<span data-ttu-id="c582b-216">workProfileBlockCamera</span><span class="sxs-lookup"><span data-stu-id="c582b-216">workProfileBlockCamera</span></span>|<span data-ttu-id="c582b-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-217">Boolean</span></span>|<span data-ttu-id="c582b-218">Câmera de perfil de trabalho de bloco.</span><span class="sxs-lookup"><span data-stu-id="c582b-218">Block work profile camera.</span></span>|
|<span data-ttu-id="c582b-219">workProfileBlockCrossProfileContactsSearch</span><span class="sxs-lookup"><span data-stu-id="c582b-219">workProfileBlockCrossProfileContactsSearch</span></span>|<span data-ttu-id="c582b-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-220">Boolean</span></span>|<span data-ttu-id="c582b-221">Disponibilidade do bloco trabalho perfil contatos no perfil pessoal.</span><span class="sxs-lookup"><span data-stu-id="c582b-221">Block work profile contacts availability in personal profile.</span></span>|
|<span data-ttu-id="c582b-222">workProfileBlockCrossProfileCopyPaste</span><span class="sxs-lookup"><span data-stu-id="c582b-222">workProfileBlockCrossProfileCopyPaste</span></span>|<span data-ttu-id="c582b-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-223">Boolean</span></span>|<span data-ttu-id="c582b-224">Boolean que indica se a configuração não permitir cruzado perfil copiar/colar está habilitada.</span><span class="sxs-lookup"><span data-stu-id="c582b-224">Boolean that indicates if the setting disallow cross profile copy/paste is enabled.</span></span>|
|<span data-ttu-id="c582b-225">workProfileDefaultAppPermissionPolicy</span><span class="sxs-lookup"><span data-stu-id="c582b-225">workProfileDefaultAppPermissionPolicy</span></span>|[<span data-ttu-id="c582b-226">androidWorkProfileDefaultAppPermissionPolicyType</span><span class="sxs-lookup"><span data-stu-id="c582b-226">androidWorkProfileDefaultAppPermissionPolicyType</span></span>](../resources/intune-deviceconfig-androidworkprofiledefaultapppermissionpolicytype.md)|<span data-ttu-id="c582b-227">Tipo de senha necessário.</span><span class="sxs-lookup"><span data-stu-id="c582b-227">Type of password that is required.</span></span> <span data-ttu-id="c582b-228">Os valores possíveis são: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span><span class="sxs-lookup"><span data-stu-id="c582b-228">Possible values are: `deviceDefault`, `prompt`, `autoGrant`, `autoDeny`.</span></span>|
|<span data-ttu-id="c582b-229">workProfilePasswordBlockFingerprintUnlock</span><span class="sxs-lookup"><span data-stu-id="c582b-229">workProfilePasswordBlockFingerprintUnlock</span></span>|<span data-ttu-id="c582b-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-230">Boolean</span></span>|<span data-ttu-id="c582b-231">Indica se o bloqueio da impressão digital ou não desbloquear para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-231">Indicates whether or not to block fingerprint unlock for work profile.</span></span>|
|<span data-ttu-id="c582b-232">workProfilePasswordBlockTrustAgents</span><span class="sxs-lookup"><span data-stu-id="c582b-232">workProfilePasswordBlockTrustAgents</span></span>|<span data-ttu-id="c582b-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-233">Boolean</span></span>|<span data-ttu-id="c582b-234">Indica se deve ou não bloquear bloqueio inteligente e outros operadores de confiabilidade para o perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-234">Indicates whether or not to block Smart Lock and other trust agents for work profile.</span></span>|
|<span data-ttu-id="c582b-235">workProfilePasswordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="c582b-235">workProfilePasswordExpirationDays</span></span>|<span data-ttu-id="c582b-236">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-236">Int32</span></span>|<span data-ttu-id="c582b-237">Número de dias até a senha do perfil de trabalho expira.</span><span class="sxs-lookup"><span data-stu-id="c582b-237">Number of days before the work profile password expires.</span></span> <span data-ttu-id="c582b-238">Valores válidos de 1 a 365</span><span class="sxs-lookup"><span data-stu-id="c582b-238">Valid values 1 to 365</span></span>|
|<span data-ttu-id="c582b-239">workProfilePasswordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="c582b-239">workProfilePasswordMinimumLength</span></span>|<span data-ttu-id="c582b-240">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-240">Int32</span></span>|<span data-ttu-id="c582b-241">Comprimento mínimo da senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-241">Minimum length of work profile password.</span></span> <span data-ttu-id="c582b-242">Valores válidos de 4 a 16</span><span class="sxs-lookup"><span data-stu-id="c582b-242">Valid values 4 to 16</span></span>|
|<span data-ttu-id="c582b-243">workProfilePasswordMinNumericCharacters</span><span class="sxs-lookup"><span data-stu-id="c582b-243">workProfilePasswordMinNumericCharacters</span></span>|<span data-ttu-id="c582b-244">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-244">Int32</span></span>|<span data-ttu-id="c582b-245">Número mínimo de caracteres numéricos necessários em senha do perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-245">Minimum # of numeric characters required in work profile password.</span></span> <span data-ttu-id="c582b-246">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="c582b-246">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c582b-247">workProfilePasswordMinNonLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="c582b-247">workProfilePasswordMinNonLetterCharacters</span></span>|<span data-ttu-id="c582b-248">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-248">Int32</span></span>|<span data-ttu-id="c582b-249">Número mínimo de caracteres não alfabéticos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-249">Minimum # of non-letter characters required in work profile password.</span></span> <span data-ttu-id="c582b-250">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="c582b-250">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c582b-251">workProfilePasswordMinLetterCharacters</span><span class="sxs-lookup"><span data-stu-id="c582b-251">workProfilePasswordMinLetterCharacters</span></span>|<span data-ttu-id="c582b-252">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-252">Int32</span></span>|<span data-ttu-id="c582b-253">Número mínimo de caracteres de carta necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-253">Minimum # of letter characters required in work profile password.</span></span> <span data-ttu-id="c582b-254">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="c582b-254">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c582b-255">workProfilePasswordMinLowerCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="c582b-255">workProfilePasswordMinLowerCaseCharacters</span></span>|<span data-ttu-id="c582b-256">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-256">Int32</span></span>|<span data-ttu-id="c582b-257">Número mínimo de caracteres minúscula necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-257">Minimum # of lower-case characters required in work profile password.</span></span> <span data-ttu-id="c582b-258">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="c582b-258">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c582b-259">workProfilePasswordMinUpperCaseCharacters</span><span class="sxs-lookup"><span data-stu-id="c582b-259">workProfilePasswordMinUpperCaseCharacters</span></span>|<span data-ttu-id="c582b-260">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-260">Int32</span></span>|<span data-ttu-id="c582b-261">Número mínimo de caracteres de maiusculas necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-261">Minimum # of upper-case characters required in work profile password.</span></span> <span data-ttu-id="c582b-262">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="c582b-262">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c582b-263">workProfilePasswordMinSymbolCharacters</span><span class="sxs-lookup"><span data-stu-id="c582b-263">workProfilePasswordMinSymbolCharacters</span></span>|<span data-ttu-id="c582b-264">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-264">Int32</span></span>|<span data-ttu-id="c582b-265">Número mínimo de símbolos necessários em senha de perfil de trabalho.</span><span class="sxs-lookup"><span data-stu-id="c582b-265">Minimum # of symbols required in work profile password.</span></span> <span data-ttu-id="c582b-266">Valores válidos 1 a 10</span><span class="sxs-lookup"><span data-stu-id="c582b-266">Valid values 1 to 10</span></span>|
|<span data-ttu-id="c582b-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="c582b-267">workProfilePasswordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="c582b-268">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-268">Int32</span></span>|<span data-ttu-id="c582b-269">Minutos de inatividade antes que a tela atinja o tempo limite.</span><span class="sxs-lookup"><span data-stu-id="c582b-269">Minutes of inactivity before the screen times out.</span></span>|
|<span data-ttu-id="c582b-270">workProfilePasswordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="c582b-270">workProfilePasswordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="c582b-271">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-271">Int32</span></span>|<span data-ttu-id="c582b-272">Número de senhas anteriores de perfil de trabalho para bloquear.</span><span class="sxs-lookup"><span data-stu-id="c582b-272">Number of previous work profile passwords to block.</span></span> <span data-ttu-id="c582b-273">Valores válidos de 0 a 24</span><span class="sxs-lookup"><span data-stu-id="c582b-273">Valid values 0 to 24</span></span>|
|<span data-ttu-id="c582b-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span><span class="sxs-lookup"><span data-stu-id="c582b-274">workProfilePasswordSignInFailureCountBeforeFactoryReset</span></span>|<span data-ttu-id="c582b-275">Int32</span><span class="sxs-lookup"><span data-stu-id="c582b-275">Int32</span></span>|<span data-ttu-id="c582b-276">Número de falhas permitidas antes que o perfil de trabalho é removido e todos os dados corporativos excluídos de entrada.</span><span class="sxs-lookup"><span data-stu-id="c582b-276">Number of sign in failures allowed before work profile is removed and all corporate data deleted.</span></span> <span data-ttu-id="c582b-277">Valores válidos 1 a 16</span><span class="sxs-lookup"><span data-stu-id="c582b-277">Valid values 1 to 16</span></span>|
|<span data-ttu-id="c582b-278">workProfilePasswordRequiredType</span><span class="sxs-lookup"><span data-stu-id="c582b-278">workProfilePasswordRequiredType</span></span>|[<span data-ttu-id="c582b-279">androidWorkProfileRequiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="c582b-279">androidWorkProfileRequiredPasswordType</span></span>](../resources/intune-deviceconfig-androidworkprofilerequiredpasswordtype.md)|<span data-ttu-id="c582b-280">Tipo de senha de perfil de trabalho que é necessário.</span><span class="sxs-lookup"><span data-stu-id="c582b-280">Type of work profile password that is required.</span></span> <span data-ttu-id="c582b-281">Os valores possíveis são: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span><span class="sxs-lookup"><span data-stu-id="c582b-281">Possible values are: `deviceDefault`, `lowSecurityBiometric`, `required`, `atLeastNumeric`, `numericComplex`, `atLeastAlphabetic`, `atLeastAlphanumeric`, `alphanumericWithSymbols`.</span></span>|
|<span data-ttu-id="c582b-282">workProfileRequirePassword</span><span class="sxs-lookup"><span data-stu-id="c582b-282">workProfileRequirePassword</span></span>|<span data-ttu-id="c582b-283">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-283">Boolean</span></span>|<span data-ttu-id="c582b-284">A senha é necessária ou não para o perfil de trabalho</span><span class="sxs-lookup"><span data-stu-id="c582b-284">Password is required or not for work profile</span></span>|
|<span data-ttu-id="c582b-285">securityRequireVerifyApps</span><span class="sxs-lookup"><span data-stu-id="c582b-285">securityRequireVerifyApps</span></span>|<span data-ttu-id="c582b-286">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-286">Boolean</span></span>|<span data-ttu-id="c582b-287">Exige que o recurso de verificação de aplicativos Android esteja ativado.</span><span class="sxs-lookup"><span data-stu-id="c582b-287">Require the Android Verify apps feature is turned on.</span></span>|
|<span data-ttu-id="c582b-288">vpnAlwaysOnPackageIdentifier</span><span class="sxs-lookup"><span data-stu-id="c582b-288">vpnAlwaysOnPackageIdentifier</span></span>|<span data-ttu-id="c582b-289">String</span><span class="sxs-lookup"><span data-stu-id="c582b-289">String</span></span>|<span data-ttu-id="c582b-290">Habilite o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="c582b-290">Enable lockdown mode for always-on VPN.</span></span>|
|<span data-ttu-id="c582b-291">vpnEnableAlwaysOnLockdownMode</span><span class="sxs-lookup"><span data-stu-id="c582b-291">vpnEnableAlwaysOnLockdownMode</span></span>|<span data-ttu-id="c582b-292">Boolean</span><span class="sxs-lookup"><span data-stu-id="c582b-292">Boolean</span></span>|<span data-ttu-id="c582b-293">Habilite o modo de bloqueio para VPN sempre ativada.</span><span class="sxs-lookup"><span data-stu-id="c582b-293">Enable lockdown mode for always-on VPN.</span></span>|



## <a name="response"></a><span data-ttu-id="c582b-294">Resposta</span><span class="sxs-lookup"><span data-stu-id="c582b-294">Response</span></span>
<span data-ttu-id="c582b-295">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="c582b-295">If successful, this method returns a `200 OK` response code and an updated [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c582b-296">Exemplo</span><span class="sxs-lookup"><span data-stu-id="c582b-296">Example</span></span>

### <a name="request"></a><span data-ttu-id="c582b-297">Solicitação</span><span class="sxs-lookup"><span data-stu-id="c582b-297">Request</span></span>
<span data-ttu-id="c582b-298">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="c582b-298">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 2042

{
  "@odata.type": "#microsoft.graph.androidWorkProfileGeneralDeviceConfiguration",
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

### <a name="response"></a><span data-ttu-id="c582b-299">Resposta</span><span class="sxs-lookup"><span data-stu-id="c582b-299">Response</span></span>
<span data-ttu-id="c582b-p129">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="c582b-p129">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




