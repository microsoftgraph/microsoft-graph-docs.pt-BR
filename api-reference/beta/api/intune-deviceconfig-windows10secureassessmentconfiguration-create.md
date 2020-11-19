---
title: Criar windows10SecureAssessmentConfiguration
description: Cria um novo objeto windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a4abcc012db78bbc92c318d0c77ef2b053e66927
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287001"
---
# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="87f05-103">Criar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="87f05-103">Create windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="87f05-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="87f05-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="87f05-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="87f05-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="87f05-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="87f05-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87f05-107">Cria um novo objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="87f05-107">Create a new [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="87f05-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="87f05-108">Prerequisites</span></span>
<span data-ttu-id="87f05-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="87f05-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87f05-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="87f05-111">Permission type</span></span>|<span data-ttu-id="87f05-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="87f05-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87f05-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="87f05-113">Delegated (work or school account)</span></span>|<span data-ttu-id="87f05-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87f05-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="87f05-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="87f05-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87f05-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="87f05-116">Not supported.</span></span>|
|<span data-ttu-id="87f05-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="87f05-117">Application</span></span>|<span data-ttu-id="87f05-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87f05-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="87f05-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="87f05-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="87f05-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="87f05-120">Request headers</span></span>
|<span data-ttu-id="87f05-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="87f05-121">Header</span></span>|<span data-ttu-id="87f05-122">Valor</span><span class="sxs-lookup"><span data-stu-id="87f05-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87f05-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="87f05-123">Authorization</span></span>|<span data-ttu-id="87f05-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="87f05-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87f05-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="87f05-125">Accept</span></span>|<span data-ttu-id="87f05-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87f05-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87f05-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="87f05-127">Request body</span></span>
<span data-ttu-id="87f05-128">No corpo da solicitação, forneça uma representação JSON do objeto windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="87f05-128">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="87f05-129">A tabela a seguir mostra as propriedades que são necessárias ao criar windows10SecureAssessmentConfiguration.</span><span class="sxs-lookup"><span data-stu-id="87f05-129">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="87f05-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="87f05-130">Property</span></span>|<span data-ttu-id="87f05-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="87f05-131">Type</span></span>|<span data-ttu-id="87f05-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="87f05-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87f05-133">id</span><span class="sxs-lookup"><span data-stu-id="87f05-133">id</span></span>|<span data-ttu-id="87f05-134">String</span><span class="sxs-lookup"><span data-stu-id="87f05-134">String</span></span>|<span data-ttu-id="87f05-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="87f05-135">Key of the entity.</span></span> <span data-ttu-id="87f05-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87f05-137">lastModifiedDateTime</span></span>|<span data-ttu-id="87f05-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87f05-138">DateTimeOffset</span></span>|<span data-ttu-id="87f05-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="87f05-139">DateTime the object was last modified.</span></span> <span data-ttu-id="87f05-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="87f05-141">roleScopeTagIds</span></span>|<span data-ttu-id="87f05-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="87f05-142">String collection</span></span>|<span data-ttu-id="87f05-143">Lista de marcas de escopo para esta instância de entidade.</span><span class="sxs-lookup"><span data-stu-id="87f05-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="87f05-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="87f05-145">supportsScopeTags</span></span>|<span data-ttu-id="87f05-146">Booliano</span><span class="sxs-lookup"><span data-stu-id="87f05-146">Boolean</span></span>|<span data-ttu-id="87f05-147">Indica se a configuração de dispositivo subjacente é ou não compatível com a atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="87f05-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="87f05-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é false e as entidades não serão visíveis aos usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="87f05-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="87f05-149">Isso ocorre para políticas herdadas criadas no Silverlight e pode ser resolvido excluindo e recriando a política no portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="87f05-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="87f05-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="87f05-150">This property is read-only.</span></span> <span data-ttu-id="87f05-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87f05-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="87f05-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="87f05-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="87f05-154">A aplicabilidade da edição do sistema operacional para essa política.</span><span class="sxs-lookup"><span data-stu-id="87f05-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="87f05-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87f05-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="87f05-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="87f05-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="87f05-158">A regra de aplicabilidade da versão do sistema operacional para esta política.</span><span class="sxs-lookup"><span data-stu-id="87f05-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="87f05-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87f05-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="87f05-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="87f05-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="87f05-162">A regra de aplicabilidade do modo de dispositivo para essa política.</span><span class="sxs-lookup"><span data-stu-id="87f05-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="87f05-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87f05-164">createdDateTime</span></span>|<span data-ttu-id="87f05-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87f05-165">DateTimeOffset</span></span>|<span data-ttu-id="87f05-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="87f05-166">DateTime the object was created.</span></span> <span data-ttu-id="87f05-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-168">description</span><span class="sxs-lookup"><span data-stu-id="87f05-168">description</span></span>|<span data-ttu-id="87f05-169">String</span><span class="sxs-lookup"><span data-stu-id="87f05-169">String</span></span>|<span data-ttu-id="87f05-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f05-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="87f05-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-172">displayName</span><span class="sxs-lookup"><span data-stu-id="87f05-172">displayName</span></span>|<span data-ttu-id="87f05-173">String</span><span class="sxs-lookup"><span data-stu-id="87f05-173">String</span></span>|<span data-ttu-id="87f05-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f05-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="87f05-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-176">versão</span><span class="sxs-lookup"><span data-stu-id="87f05-176">version</span></span>|<span data-ttu-id="87f05-177">Int32</span><span class="sxs-lookup"><span data-stu-id="87f05-177">Int32</span></span>|<span data-ttu-id="87f05-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="87f05-178">Version of the device configuration.</span></span> <span data-ttu-id="87f05-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="87f05-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="87f05-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="87f05-180">launchUri</span></span>|<span data-ttu-id="87f05-181">String</span><span class="sxs-lookup"><span data-stu-id="87f05-181">String</span></span>|<span data-ttu-id="87f05-182">Link de URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="87f05-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="87f05-183">Ele precisa ser um URL válido (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="87f05-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="87f05-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="87f05-184">configurationAccount</span></span>|<span data-ttu-id="87f05-185">String</span><span class="sxs-lookup"><span data-stu-id="87f05-185">String</span></span>|<span data-ttu-id="87f05-186">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="87f05-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="87f05-187">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="87f05-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="87f05-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="87f05-188">configurationAccountType</span></span>|[<span data-ttu-id="87f05-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="87f05-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="87f05-190">O tipo de conta usado pelo ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="87f05-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="87f05-191">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="87f05-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="87f05-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="87f05-192">allowPrinting</span></span>|<span data-ttu-id="87f05-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="87f05-193">Boolean</span></span>|<span data-ttu-id="87f05-194">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="87f05-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="87f05-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="87f05-195">allowScreenCapture</span></span>|<span data-ttu-id="87f05-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="87f05-196">Boolean</span></span>|<span data-ttu-id="87f05-197">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="87f05-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="87f05-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="87f05-198">allowTextSuggestion</span></span>|<span data-ttu-id="87f05-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="87f05-199">Boolean</span></span>|<span data-ttu-id="87f05-200">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="87f05-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="87f05-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="87f05-201">localGuestAccountName</span></span>|<span data-ttu-id="87f05-202">String</span><span class="sxs-lookup"><span data-stu-id="87f05-202">String</span></span>|<span data-ttu-id="87f05-203">Especifica o texto de exibição da conta de convidado local mostrada na tela de entrada.</span><span class="sxs-lookup"><span data-stu-id="87f05-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="87f05-204">Normalmente é o nome de uma avaliação.</span><span class="sxs-lookup"><span data-stu-id="87f05-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="87f05-205">Quando o usuário clica na conta de convidado local na tela de entrada, um aplicativo de avaliação é iniciado com uma URL de avaliação especificada.</span><span class="sxs-lookup"><span data-stu-id="87f05-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="87f05-206">As avaliações seguras só podem ser configuradas com a entrada de conta de convidado local em dispositivos que executam o Windows 10, versão 1903 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="87f05-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="87f05-207">Aviso importante: essa propriedade deve ser definida com o assessmentAppUserModelID para que a experiência de entrada da conta de convidado local funcione corretamente para avaliações seguras.</span><span class="sxs-lookup"><span data-stu-id="87f05-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="87f05-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="87f05-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="87f05-209">String</span><span class="sxs-lookup"><span data-stu-id="87f05-209">String</span></span>|<span data-ttu-id="87f05-210">Especifica a ID do modelo de usuário do aplicativo do aplicativo de avaliação iniciado quando um usuário entrar em uma avaliação segura com uma conta de convidado local.</span><span class="sxs-lookup"><span data-stu-id="87f05-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="87f05-211">Aviso importante: essa propriedade deve ser definida com o localGuestAccountName para que a experiência de entrada da conta de convidado local funcione corretamente para avaliações seguras.</span><span class="sxs-lookup"><span data-stu-id="87f05-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="87f05-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="87f05-212">Response</span></span>
<span data-ttu-id="87f05-213">Se bem-sucedido, este método retornará um código de resposta `201 Created` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="87f05-213">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87f05-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="87f05-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="87f05-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="87f05-215">Request</span></span>
<span data-ttu-id="87f05-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="87f05-216">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="87f05-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="87f05-217">Response</span></span>
<span data-ttu-id="87f05-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="87f05-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




