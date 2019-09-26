---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20dd4fa2ddb6caacb47458ff71a69d23358655e9
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182194"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="26ee1-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="26ee1-103">Update windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="26ee1-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="26ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="26ee1-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="26ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="26ee1-106">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26ee1-106">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="26ee1-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="26ee1-107">Prerequisites</span></span>
<span data-ttu-id="26ee1-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="26ee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="26ee1-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="26ee1-110">Permission type</span></span>|<span data-ttu-id="26ee1-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="26ee1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="26ee1-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="26ee1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="26ee1-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ee1-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="26ee1-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="26ee1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="26ee1-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="26ee1-115">Not supported.</span></span>|
|<span data-ttu-id="26ee1-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="26ee1-116">Application</span></span>|<span data-ttu-id="26ee1-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="26ee1-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="26ee1-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="26ee1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="26ee1-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="26ee1-119">Request headers</span></span>
|<span data-ttu-id="26ee1-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="26ee1-120">Header</span></span>|<span data-ttu-id="26ee1-121">Valor</span><span class="sxs-lookup"><span data-stu-id="26ee1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="26ee1-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="26ee1-122">Authorization</span></span>|<span data-ttu-id="26ee1-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="26ee1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="26ee1-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="26ee1-124">Accept</span></span>|<span data-ttu-id="26ee1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="26ee1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="26ee1-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="26ee1-126">Request body</span></span>
<span data-ttu-id="26ee1-127">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26ee1-127">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="26ee1-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="26ee1-128">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="26ee1-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="26ee1-129">Property</span></span>|<span data-ttu-id="26ee1-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="26ee1-130">Type</span></span>|<span data-ttu-id="26ee1-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="26ee1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="26ee1-132">id</span><span class="sxs-lookup"><span data-stu-id="26ee1-132">id</span></span>|<span data-ttu-id="26ee1-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="26ee1-133">String</span></span>|<span data-ttu-id="26ee1-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="26ee1-134">Key of the entity.</span></span> <span data-ttu-id="26ee1-135">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-135">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="26ee1-136">lastModifiedDateTime</span></span>|<span data-ttu-id="26ee1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26ee1-137">DateTimeOffset</span></span>|<span data-ttu-id="26ee1-138">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="26ee1-138">DateTime the object was last modified.</span></span> <span data-ttu-id="26ee1-139">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-139">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-140">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="26ee1-140">roleScopeTagIds</span></span>|<span data-ttu-id="26ee1-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="26ee1-141">String collection</span></span>|<span data-ttu-id="26ee1-142">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="26ee1-142">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="26ee1-143">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-143">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-144">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="26ee1-144">supportsScopeTags</span></span>|<span data-ttu-id="26ee1-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="26ee1-145">Boolean</span></span>|<span data-ttu-id="26ee1-146">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="26ee1-146">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="26ee1-147">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="26ee1-147">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="26ee1-148">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="26ee1-148">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="26ee1-149">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="26ee1-149">This property is read-only.</span></span> <span data-ttu-id="26ee1-150">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-150">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-151">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26ee1-151">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="26ee1-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="26ee1-152">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="26ee1-153">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="26ee1-153">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="26ee1-154">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-154">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-155">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26ee1-155">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="26ee1-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="26ee1-156">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="26ee1-157">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="26ee1-157">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="26ee1-158">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-158">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-159">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26ee1-159">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="26ee1-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="26ee1-160">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="26ee1-161">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="26ee1-161">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="26ee1-162">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-162">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-163">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="26ee1-163">createdDateTime</span></span>|<span data-ttu-id="26ee1-164">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="26ee1-164">DateTimeOffset</span></span>|<span data-ttu-id="26ee1-165">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="26ee1-165">DateTime the object was created.</span></span> <span data-ttu-id="26ee1-166">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-166">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-167">descrição</span><span class="sxs-lookup"><span data-stu-id="26ee1-167">description</span></span>|<span data-ttu-id="26ee1-168">String</span><span class="sxs-lookup"><span data-stu-id="26ee1-168">String</span></span>|<span data-ttu-id="26ee1-169">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26ee1-169">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="26ee1-170">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-170">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-171">displayName</span><span class="sxs-lookup"><span data-stu-id="26ee1-171">displayName</span></span>|<span data-ttu-id="26ee1-172">String</span><span class="sxs-lookup"><span data-stu-id="26ee1-172">String</span></span>|<span data-ttu-id="26ee1-173">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26ee1-173">Admin provided name of the device configuration.</span></span> <span data-ttu-id="26ee1-174">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-174">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-175">versão</span><span class="sxs-lookup"><span data-stu-id="26ee1-175">version</span></span>|<span data-ttu-id="26ee1-176">Int32</span><span class="sxs-lookup"><span data-stu-id="26ee1-176">Int32</span></span>|<span data-ttu-id="26ee1-177">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="26ee1-177">Version of the device configuration.</span></span> <span data-ttu-id="26ee1-178">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="26ee1-178">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="26ee1-179">launchUri</span><span class="sxs-lookup"><span data-stu-id="26ee1-179">launchUri</span></span>|<span data-ttu-id="26ee1-180">String</span><span class="sxs-lookup"><span data-stu-id="26ee1-180">String</span></span>|<span data-ttu-id="26ee1-181">Link de URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="26ee1-181">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="26ee1-182">Ele precisa ser um URL válido (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="26ee1-182">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="26ee1-183">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="26ee1-183">configurationAccount</span></span>|<span data-ttu-id="26ee1-184">String</span><span class="sxs-lookup"><span data-stu-id="26ee1-184">String</span></span>|<span data-ttu-id="26ee1-185">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="26ee1-185">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="26ee1-186">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="26ee1-186">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="26ee1-187">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="26ee1-187">configurationAccountType</span></span>|[<span data-ttu-id="26ee1-188">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="26ee1-188">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="26ee1-189">O tipo de conta usado pelo ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="26ee1-189">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="26ee1-190">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="26ee1-190">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="26ee1-191">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="26ee1-191">allowPrinting</span></span>|<span data-ttu-id="26ee1-192">Booliano</span><span class="sxs-lookup"><span data-stu-id="26ee1-192">Boolean</span></span>|<span data-ttu-id="26ee1-193">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="26ee1-193">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="26ee1-194">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="26ee1-194">allowScreenCapture</span></span>|<span data-ttu-id="26ee1-195">Booliano</span><span class="sxs-lookup"><span data-stu-id="26ee1-195">Boolean</span></span>|<span data-ttu-id="26ee1-196">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="26ee1-196">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="26ee1-197">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="26ee1-197">allowTextSuggestion</span></span>|<span data-ttu-id="26ee1-198">Boolean</span><span class="sxs-lookup"><span data-stu-id="26ee1-198">Boolean</span></span>|<span data-ttu-id="26ee1-199">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="26ee1-199">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="26ee1-200">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="26ee1-200">localGuestAccountName</span></span>|<span data-ttu-id="26ee1-201">String</span><span class="sxs-lookup"><span data-stu-id="26ee1-201">String</span></span>|<span data-ttu-id="26ee1-202">Especifica o texto de exibição da conta de convidado local mostrada na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="26ee1-202">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="26ee1-203">Normalmente é o nome de uma avaliação.</span><span class="sxs-lookup"><span data-stu-id="26ee1-203">Typically is the name of an assessment.</span></span> <span data-ttu-id="26ee1-204">Quando o usuário clica na conta de convidado local na tela de entrada, um aplicativo de avaliação é iniciado com uma URL de avaliação especificada.</span><span class="sxs-lookup"><span data-stu-id="26ee1-204">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="26ee1-205">As avaliações seguras só podem ser configuradas com a entrada de conta de convidado local em dispositivos que executam o Windows 10, versão 1903 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="26ee1-205">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="26ee1-206">Aviso importante: essa propriedade deve ser definida com o assessmentAppUserModelID para que a experiência de entrada da conta de convidado local funcione corretamente para avaliações seguras.</span><span class="sxs-lookup"><span data-stu-id="26ee1-206">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="26ee1-207">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="26ee1-207">assessmentAppUserModelId</span></span>|<span data-ttu-id="26ee1-208">String</span><span class="sxs-lookup"><span data-stu-id="26ee1-208">String</span></span>|<span data-ttu-id="26ee1-209">Especifica a ID do modelo de usuário do aplicativo do aplicativo de avaliação iniciado quando um usuário entrar em uma avaliação segura com uma conta de convidado local.</span><span class="sxs-lookup"><span data-stu-id="26ee1-209">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="26ee1-210">Aviso importante: essa propriedade deve ser definida com o localGuestAccountName para que a experiência de entrada da conta de convidado local funcione corretamente para avaliações seguras.</span><span class="sxs-lookup"><span data-stu-id="26ee1-210">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="26ee1-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ee1-211">Response</span></span>
<span data-ttu-id="26ee1-212">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="26ee1-212">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="26ee1-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="26ee1-213">Example</span></span>

### <a name="request"></a><span data-ttu-id="26ee1-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="26ee1-214">Request</span></span>
<span data-ttu-id="26ee1-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="26ee1-215">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 1403

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="26ee1-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="26ee1-216">Response</span></span>
<span data-ttu-id="26ee1-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="26ee1-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1575

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "supportsScopeTags": true,
  "deviceManagementApplicabilityRuleOsEdition": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsEdition",
    "osEditionTypes": [
      "windows10EnterpriseN"
    ],
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleOsVersion": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleOsVersion",
    "minOSVersion": "Min OSVersion value",
    "maxOSVersion": "Max OSVersion value",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "deviceManagementApplicabilityRuleDeviceMode": {
    "@odata.type": "microsoft.graph.deviceManagementApplicabilityRuleDeviceMode",
    "deviceMode": "sModeConfiguration",
    "name": "Name value",
    "ruleType": "exclude"
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "configurationAccountType": "domainAccount",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true,
  "localGuestAccountName": "Local Guest Account Name value",
  "assessmentAppUserModelId": "Assessment App User Model Id value"
}
```




