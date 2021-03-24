---
title: Atualizar windows10SecureAssessmentConfiguration
description: Atualizar as propriedades de um objeto windows10SecureAssessmentConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fc91366f1d7ae9e827795f10b95cd352f9d97b42
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51127442"
---
# <a name="update-windows10secureassessmentconfiguration"></a><span data-ttu-id="51967-103">Atualizar windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="51967-103">Update windows10SecureAssessmentConfiguration</span></span>

<span data-ttu-id="51967-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51967-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51967-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="51967-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="51967-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="51967-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51967-107">Atualizar as propriedades de um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51967-107">Update the properties of a [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51967-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="51967-108">Prerequisites</span></span>
<span data-ttu-id="51967-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="51967-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51967-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="51967-111">Permission type</span></span>|<span data-ttu-id="51967-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="51967-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51967-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="51967-113">Delegated (work or school account)</span></span>|<span data-ttu-id="51967-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51967-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="51967-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="51967-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51967-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="51967-116">Not supported.</span></span>|
|<span data-ttu-id="51967-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="51967-117">Application</span></span>|<span data-ttu-id="51967-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51967-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51967-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="51967-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="51967-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="51967-120">Request headers</span></span>
|<span data-ttu-id="51967-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="51967-121">Header</span></span>|<span data-ttu-id="51967-122">Valor</span><span class="sxs-lookup"><span data-stu-id="51967-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51967-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="51967-123">Authorization</span></span>|<span data-ttu-id="51967-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="51967-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51967-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="51967-125">Accept</span></span>|<span data-ttu-id="51967-126">application/json</span><span class="sxs-lookup"><span data-stu-id="51967-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51967-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="51967-127">Request body</span></span>
<span data-ttu-id="51967-128">No corpo da solicitação, forneça uma representação JSON do objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51967-128">In the request body, supply a JSON representation for the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object.</span></span>

<span data-ttu-id="51967-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="51967-129">The following table shows the properties that are required when you create the [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md).</span></span>

|<span data-ttu-id="51967-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="51967-130">Property</span></span>|<span data-ttu-id="51967-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="51967-131">Type</span></span>|<span data-ttu-id="51967-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="51967-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51967-133">id</span><span class="sxs-lookup"><span data-stu-id="51967-133">id</span></span>|<span data-ttu-id="51967-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51967-134">String</span></span>|<span data-ttu-id="51967-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="51967-135">Key of the entity.</span></span> <span data-ttu-id="51967-136">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-136">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-137">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="51967-137">lastModifiedDateTime</span></span>|<span data-ttu-id="51967-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51967-138">DateTimeOffset</span></span>|<span data-ttu-id="51967-139">DateTime da última modificação do objeto.</span><span class="sxs-lookup"><span data-stu-id="51967-139">DateTime the object was last modified.</span></span> <span data-ttu-id="51967-140">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-140">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="51967-141">roleScopeTagIds</span></span>|<span data-ttu-id="51967-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="51967-142">String collection</span></span>|<span data-ttu-id="51967-143">Lista de marcas de escopo para esta instância entity.</span><span class="sxs-lookup"><span data-stu-id="51967-143">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="51967-144">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-144">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-145">supportsScopeTags</span><span class="sxs-lookup"><span data-stu-id="51967-145">supportsScopeTags</span></span>|<span data-ttu-id="51967-146">Booleano</span><span class="sxs-lookup"><span data-stu-id="51967-146">Boolean</span></span>|<span data-ttu-id="51967-147">Indica se a Configuração de Dispositivo subjacente dá suporte ou não à atribuição de marcas de escopo.</span><span class="sxs-lookup"><span data-stu-id="51967-147">Indicates whether or not the underlying Device Configuration supports the assignment of scope tags.</span></span> <span data-ttu-id="51967-148">A atribuição à propriedade ScopeTags não é permitida quando esse valor é falso e as entidades não estarão visíveis para usuários com escopo.</span><span class="sxs-lookup"><span data-stu-id="51967-148">Assigning to the ScopeTags property is not allowed when this value is false and entities will not be visible to scoped users.</span></span> <span data-ttu-id="51967-149">Isso ocorre para políticas herdadas criadas no Silverlight e podem ser resolvidas excluindo e recriando a política no Portal do Azure.</span><span class="sxs-lookup"><span data-stu-id="51967-149">This occurs for Legacy policies created in Silverlight and can be resolved by deleting and recreating the policy in the Azure Portal.</span></span> <span data-ttu-id="51967-150">Essa propriedade é somente leitura.</span><span class="sxs-lookup"><span data-stu-id="51967-150">This property is read-only.</span></span> <span data-ttu-id="51967-151">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-151">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-152">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51967-152">deviceManagementApplicabilityRuleOsEdition</span></span>|[<span data-ttu-id="51967-153">deviceManagementApplicabilityRuleOsEdition</span><span class="sxs-lookup"><span data-stu-id="51967-153">deviceManagementApplicabilityRuleOsEdition</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosedition.md)|<span data-ttu-id="51967-154">A aplicabilidade da edição do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="51967-154">The OS edition applicability for this Policy.</span></span> <span data-ttu-id="51967-155">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-155">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-156">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51967-156">deviceManagementApplicabilityRuleOsVersion</span></span>|[<span data-ttu-id="51967-157">deviceManagementApplicabilityRuleOsVersion</span><span class="sxs-lookup"><span data-stu-id="51967-157">deviceManagementApplicabilityRuleOsVersion</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruleosversion.md)|<span data-ttu-id="51967-158">A regra de aplicabilidade da versão do sistema operacional para esta Política.</span><span class="sxs-lookup"><span data-stu-id="51967-158">The OS version applicability rule for this Policy.</span></span> <span data-ttu-id="51967-159">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-159">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-160">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51967-160">deviceManagementApplicabilityRuleDeviceMode</span></span>|[<span data-ttu-id="51967-161">deviceManagementApplicabilityRuleDeviceMode</span><span class="sxs-lookup"><span data-stu-id="51967-161">deviceManagementApplicabilityRuleDeviceMode</span></span>](../resources/intune-deviceconfig-devicemanagementapplicabilityruledevicemode.md)|<span data-ttu-id="51967-162">A regra de aplicabilidade do modo de dispositivo para esta Política.</span><span class="sxs-lookup"><span data-stu-id="51967-162">The device mode applicability rule for this Policy.</span></span> <span data-ttu-id="51967-163">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-163">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-164">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="51967-164">createdDateTime</span></span>|<span data-ttu-id="51967-165">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="51967-165">DateTimeOffset</span></span>|<span data-ttu-id="51967-166">DateTime em que o objeto foi criado.</span><span class="sxs-lookup"><span data-stu-id="51967-166">DateTime the object was created.</span></span> <span data-ttu-id="51967-167">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-167">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-168">descrição</span><span class="sxs-lookup"><span data-stu-id="51967-168">description</span></span>|<span data-ttu-id="51967-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51967-169">String</span></span>|<span data-ttu-id="51967-170">O administrador forneceu a descrição da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51967-170">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="51967-171">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-171">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-172">displayName</span><span class="sxs-lookup"><span data-stu-id="51967-172">displayName</span></span>|<span data-ttu-id="51967-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51967-173">String</span></span>|<span data-ttu-id="51967-174">O administrador forneceu o nome da Configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51967-174">Admin provided name of the device configuration.</span></span> <span data-ttu-id="51967-175">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-175">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-176">versão</span><span class="sxs-lookup"><span data-stu-id="51967-176">version</span></span>|<span data-ttu-id="51967-177">Int32</span><span class="sxs-lookup"><span data-stu-id="51967-177">Int32</span></span>|<span data-ttu-id="51967-178">Versão da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="51967-178">Version of the device configuration.</span></span> <span data-ttu-id="51967-179">Herdada de [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="51967-179">Inherited from [deviceConfiguration](../resources/intune-shared-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="51967-180">launchUri</span><span class="sxs-lookup"><span data-stu-id="51967-180">launchUri</span></span>|<span data-ttu-id="51967-181">String</span><span class="sxs-lookup"><span data-stu-id="51967-181">String</span></span>|<span data-ttu-id="51967-182">Link de URL para uma avaliação que é carregada automaticamente quando o navegador de avaliação segura é iniciado.</span><span class="sxs-lookup"><span data-stu-id="51967-182">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="51967-183">Ele precisa ser um URL válido (http\[s\]://msdn.microsoft.com/).</span><span class="sxs-lookup"><span data-stu-id="51967-183">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="51967-184">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="51967-184">configurationAccount</span></span>|<span data-ttu-id="51967-185">String</span><span class="sxs-lookup"><span data-stu-id="51967-185">String</span></span>|<span data-ttu-id="51967-186">A conta usada para configurar o dispositivo Windows para realizar o teste.</span><span class="sxs-lookup"><span data-stu-id="51967-186">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="51967-187">O usuário pode ser uma conta de domínio (domínio\usuário), uma conta do AAD (nomedeusuário@locatário.com) ou uma conta local (nomedeusuário).</span><span class="sxs-lookup"><span data-stu-id="51967-187">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="51967-188">configurationAccountType</span><span class="sxs-lookup"><span data-stu-id="51967-188">configurationAccountType</span></span>|[<span data-ttu-id="51967-189">secureAssessmentAccountType</span><span class="sxs-lookup"><span data-stu-id="51967-189">secureAssessmentAccountType</span></span>](../resources/intune-deviceconfig-secureassessmentaccounttype.md)|<span data-ttu-id="51967-190">O tipo de conta usado por ConfigurationAccount.</span><span class="sxs-lookup"><span data-stu-id="51967-190">The account type used to by ConfigurationAccount.</span></span> <span data-ttu-id="51967-191">Os valores possíveis são: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span><span class="sxs-lookup"><span data-stu-id="51967-191">Possible values are: `azureADAccount`, `domainAccount`, `localAccount`, `localGuestAccount`.</span></span>|
|<span data-ttu-id="51967-192">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="51967-192">allowPrinting</span></span>|<span data-ttu-id="51967-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="51967-193">Boolean</span></span>|<span data-ttu-id="51967-194">Indica se o aplicativo deve ou não ter permissão de impressão durante o teste.</span><span class="sxs-lookup"><span data-stu-id="51967-194">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="51967-195">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="51967-195">allowScreenCapture</span></span>|<span data-ttu-id="51967-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="51967-196">Boolean</span></span>|<span data-ttu-id="51967-197">Indica se a capacidade de captura de tela deve ou não ser permitida durante um teste.</span><span class="sxs-lookup"><span data-stu-id="51967-197">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="51967-198">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="51967-198">allowTextSuggestion</span></span>|<span data-ttu-id="51967-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="51967-199">Boolean</span></span>|<span data-ttu-id="51967-200">Indica se sugestões de texto devem ou não ser permitidas durante o teste.</span><span class="sxs-lookup"><span data-stu-id="51967-200">Indicates whether or not to allow text suggestions during the test.</span></span>|
|<span data-ttu-id="51967-201">localGuestAccountName</span><span class="sxs-lookup"><span data-stu-id="51967-201">localGuestAccountName</span></span>|<span data-ttu-id="51967-202">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51967-202">String</span></span>|<span data-ttu-id="51967-203">Especifica o texto de exibição da conta de convidado local mostrada na tela de login.</span><span class="sxs-lookup"><span data-stu-id="51967-203">Specifies the display text for the local guest account shown on the sign-in screen.</span></span> <span data-ttu-id="51967-204">Normalmente é o nome de uma avaliação.</span><span class="sxs-lookup"><span data-stu-id="51967-204">Typically is the name of an assessment.</span></span> <span data-ttu-id="51967-205">Quando o usuário clica na conta de convidado local na tela de login, um aplicativo de avaliação é lançado com uma URL de avaliação especificada.</span><span class="sxs-lookup"><span data-stu-id="51967-205">When the user clicks the local guest account on the sign-in screen, an assessment app is launched with a specified assessment URL.</span></span> <span data-ttu-id="51967-206">Avaliações seguras só podem ser configuradas com entrada de conta de convidado local em dispositivos que executam o Windows 10, versão 1903 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="51967-206">Secure assessments can only be configured with local guest account sign-in on devices running Windows 10, version 1903 or later.</span></span> <span data-ttu-id="51967-207">Aviso importante: essa propriedade deve ser definida com assessmentAppUserModelID para fazer com que a experiência de login da conta de convidado local funcione corretamente para avaliações seguras.</span><span class="sxs-lookup"><span data-stu-id="51967-207">Important notice: this property must be set with assessmentAppUserModelID in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|
|<span data-ttu-id="51967-208">assessmentAppUserModelId</span><span class="sxs-lookup"><span data-stu-id="51967-208">assessmentAppUserModelId</span></span>|<span data-ttu-id="51967-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="51967-209">String</span></span>|<span data-ttu-id="51967-210">Especifica a ID do modelo de usuário do aplicativo de avaliação lançado quando um usuário entrar em uma avaliação segura com uma conta de convidado local.</span><span class="sxs-lookup"><span data-stu-id="51967-210">Specifies the application user model ID of the assessment app launched when a user signs in to a secure assessment with a local guest account.</span></span> <span data-ttu-id="51967-211">Aviso importante: essa propriedade deve ser definida com localGuestAccountName para fazer com que a experiência de login da conta de convidado local funcione corretamente para avaliações seguras.</span><span class="sxs-lookup"><span data-stu-id="51967-211">Important notice: this property must be set with localGuestAccountName in order to make the local guest account sign-in experience work properly for secure assessments.</span></span>|



## <a name="response"></a><span data-ttu-id="51967-212">Resposta</span><span class="sxs-lookup"><span data-stu-id="51967-212">Response</span></span>
<span data-ttu-id="51967-213">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="51967-213">If successful, this method returns a `200 OK` response code and an updated [windows10SecureAssessmentConfiguration](../resources/intune-deviceconfig-windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51967-214">Exemplo</span><span class="sxs-lookup"><span data-stu-id="51967-214">Example</span></span>

### <a name="request"></a><span data-ttu-id="51967-215">Solicitação</span><span class="sxs-lookup"><span data-stu-id="51967-215">Request</span></span>
<span data-ttu-id="51967-216">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="51967-216">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="51967-217">Resposta</span><span class="sxs-lookup"><span data-stu-id="51967-217">Response</span></span>
<span data-ttu-id="51967-p118">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="51967-p118">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




