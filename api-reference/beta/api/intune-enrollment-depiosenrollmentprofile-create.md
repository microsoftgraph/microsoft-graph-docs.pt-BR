---
title: Criar depIOSEnrollmentProfile
description: Crie um novo objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3a8f3e63b84132f5547c450b21a3cc8a44149369
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145982"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="67faa-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="67faa-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="67faa-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67faa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67faa-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67faa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67faa-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67faa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67faa-107">Crie um novo [objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67faa-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="67faa-108">Prerequisites</span></span>
<span data-ttu-id="67faa-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="67faa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67faa-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="67faa-111">Permission type</span></span>|<span data-ttu-id="67faa-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="67faa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67faa-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="67faa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="67faa-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67faa-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="67faa-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="67faa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67faa-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="67faa-116">Not supported.</span></span>|
|<span data-ttu-id="67faa-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="67faa-117">Application</span></span>|<span data-ttu-id="67faa-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67faa-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="67faa-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="67faa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="67faa-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="67faa-120">Request headers</span></span>
|<span data-ttu-id="67faa-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="67faa-121">Header</span></span>|<span data-ttu-id="67faa-122">Valor</span><span class="sxs-lookup"><span data-stu-id="67faa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67faa-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="67faa-123">Authorization</span></span>|<span data-ttu-id="67faa-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="67faa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67faa-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="67faa-125">Accept</span></span>|<span data-ttu-id="67faa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="67faa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67faa-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="67faa-127">Request body</span></span>
<span data-ttu-id="67faa-128">No corpo da solicitação, fornece uma representação JSON para o objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="67faa-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="67faa-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="67faa-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="67faa-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67faa-130">Property</span></span>|<span data-ttu-id="67faa-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="67faa-131">Type</span></span>|<span data-ttu-id="67faa-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="67faa-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67faa-133">id</span><span class="sxs-lookup"><span data-stu-id="67faa-133">id</span></span>|<span data-ttu-id="67faa-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-134">String</span></span>|<span data-ttu-id="67faa-135">O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-136">displayName</span><span class="sxs-lookup"><span data-stu-id="67faa-136">displayName</span></span>|<span data-ttu-id="67faa-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-137">String</span></span>|<span data-ttu-id="67faa-138">Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-139">descrição</span><span class="sxs-lookup"><span data-stu-id="67faa-139">description</span></span>|<span data-ttu-id="67faa-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-140">String</span></span>|<span data-ttu-id="67faa-141">Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="67faa-142">requiresUserAuthentication</span></span>|<span data-ttu-id="67faa-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-143">Boolean</span></span>|<span data-ttu-id="67faa-144">Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="67faa-145">configurationEndpointUrl</span></span>|<span data-ttu-id="67faa-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-146">String</span></span>|<span data-ttu-id="67faa-147">URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="67faa-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="67faa-149">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-149">Boolean</span></span>|<span data-ttu-id="67faa-150">Indica a autenticação com o Assistente de Instalação da Apple em vez do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="67faa-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="67faa-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="67faa-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="67faa-153">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-153">Boolean</span></span>|<span data-ttu-id="67faa-154">Indica que o Portal da Empresa é necessário em dispositivos inscritos pelo assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="67faa-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="67faa-155">isDefault</span></span>|<span data-ttu-id="67faa-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="67faa-156">Boolean</span></span>|<span data-ttu-id="67faa-157">Indica se esse é o perfil padrão Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="67faa-158">supervisedModeEnabled</span></span>|<span data-ttu-id="67faa-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-159">Boolean</span></span>|<span data-ttu-id="67faa-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="67faa-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="67faa-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="67faa-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="67faa-162">Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="67faa-163">supportDepartment</span></span>|<span data-ttu-id="67faa-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-164">String</span></span>|<span data-ttu-id="67faa-165">Informações do departamento de suporte Herdadas [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="67faa-166">isMandatory</span></span>|<span data-ttu-id="67faa-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-167">Boolean</span></span>|<span data-ttu-id="67faa-168">Indica se o perfil é obrigatório Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-169">locationDisabled</span></span>|<span data-ttu-id="67faa-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-170">Boolean</span></span>|<span data-ttu-id="67faa-171">Indica se o painel de configuração do serviço de local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="67faa-172">supportPhoneNumber</span></span>|<span data-ttu-id="67faa-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-173">String</span></span>|<span data-ttu-id="67faa-174">Número de telefone de suporte Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-175">profileRemovalDisabled</span></span>|<span data-ttu-id="67faa-176">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-176">Boolean</span></span>|<span data-ttu-id="67faa-177">Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="67faa-178">restoreBlocked</span></span>|<span data-ttu-id="67faa-179">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-179">Boolean</span></span>|<span data-ttu-id="67faa-180">Indica se o painel restaurar instalação está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-181">appleIdDisabled</span></span>|<span data-ttu-id="67faa-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-182">Boolean</span></span>|<span data-ttu-id="67faa-183">Indica se o painel de configuração de ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="67faa-185">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-185">Boolean</span></span>|<span data-ttu-id="67faa-186">Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-187">touchIdDisabled</span></span>|<span data-ttu-id="67faa-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-188">Boolean</span></span>|<span data-ttu-id="67faa-189">Indica se o painel de configuração de id por toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-190">applePayDisabled</span></span>|<span data-ttu-id="67faa-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-191">Boolean</span></span>|<span data-ttu-id="67faa-192">Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-193">siriDisabled</span></span>|<span data-ttu-id="67faa-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-194">Boolean</span></span>|<span data-ttu-id="67faa-195">Indica se o painel de configuração de siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-196">diagnosticsDisabled</span></span>|<span data-ttu-id="67faa-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-197">Boolean</span></span>|<span data-ttu-id="67faa-198">Indica se o painel de configuração de diagnósticos está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="67faa-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-200">Boolean</span></span>|<span data-ttu-id="67faa-201">Indica se a tela de instalação de displaytone está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-202">privacyPaneDisabled</span></span>|<span data-ttu-id="67faa-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-203">Boolean</span></span>|<span data-ttu-id="67faa-204">Indica se a tela de privacidade está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="67faa-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-206">Boolean</span></span>|<span data-ttu-id="67faa-207">Indica se a configuração do tempo de tempo de tela está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="67faa-208">deviceNameTemplate</span></span>|<span data-ttu-id="67faa-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-209">String</span></span>|<span data-ttu-id="67faa-210">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="67faa-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="67faa-211">Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="67faa-212">configurationWebUrl</span></span>|<span data-ttu-id="67faa-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-213">Boolean</span></span>|<span data-ttu-id="67faa-214">URL para logon do assistente de instalação Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="67faa-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="67faa-215">iTunesPairingMode</span></span>|[<span data-ttu-id="67faa-216">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="67faa-216">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="67faa-217">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="67faa-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="67faa-218">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="67faa-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="67faa-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="67faa-219">managementCertificates</span></span>|<span data-ttu-id="67faa-220">[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="67faa-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="67faa-221">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="67faa-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="67faa-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="67faa-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-223">Boolean</span></span>|<span data-ttu-id="67faa-224">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="67faa-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="67faa-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="67faa-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-226">Boolean</span></span>|<span data-ttu-id="67faa-227">Indica se o dispositivo precisará aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="67faa-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="67faa-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="67faa-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="67faa-229">Int32</span><span class="sxs-lookup"><span data-stu-id="67faa-229">Int32</span></span>|<span data-ttu-id="67faa-230">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="67faa-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="67faa-231">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="67faa-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="67faa-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="67faa-232">enableSharedIPad</span></span>|<span data-ttu-id="67faa-233">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-233">Boolean</span></span>|<span data-ttu-id="67faa-234">Isso indica se o dispositivo deve ser inscrito em um modo que habilita cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="67faa-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="67faa-235">Aplicável somente em iPads compartilhados.</span><span class="sxs-lookup"><span data-stu-id="67faa-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="67faa-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="67faa-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="67faa-237">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67faa-237">String</span></span>|<span data-ttu-id="67faa-238">Se definido, indica qual token Vpp deve ser usado para implantar o licenciamento de dispositivo do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="67faa-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="67faa-239">'enableAuthenticationViaCompanyPortal' deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="67faa-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="67faa-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="67faa-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="67faa-241">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-241">Boolean</span></span>|<span data-ttu-id="67faa-242">Informa ao dispositivo para habilitar o modo de aplicativo único e aplicar o bloqueio de aplicativo durante o registro.</span><span class="sxs-lookup"><span data-stu-id="67faa-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="67faa-243">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="67faa-243">Default is false.</span></span> <span data-ttu-id="67faa-244">'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="67faa-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="67faa-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="67faa-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-246">Boolean</span></span>|<span data-ttu-id="67faa-247">Indica se a tela de sensibilidade do botão inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="67faa-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="67faa-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-249">Boolean</span></span>|<span data-ttu-id="67faa-250">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="67faa-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="67faa-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-252">Boolean</span></span>|<span data-ttu-id="67faa-253">Indica se a tela de instalação de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="67faa-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="67faa-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-255">Boolean</span></span>|<span data-ttu-id="67faa-256">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="67faa-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="67faa-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-258">Boolean</span></span>|<span data-ttu-id="67faa-259">Indica se a tela de atualização de sofware obrigatória está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="67faa-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="67faa-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-261">Boolean</span></span>|<span data-ttu-id="67faa-262">Indica se a tela de migração do relógio está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="67faa-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="67faa-264">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-264">Boolean</span></span>|<span data-ttu-id="67faa-265">Indica se a tela do Apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="67faa-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="67faa-267">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-267">Boolean</span></span>|<span data-ttu-id="67faa-268">Indica se a tela linguagem expressa está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="67faa-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="67faa-270">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-270">Boolean</span></span>|<span data-ttu-id="67faa-271">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="67faa-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="67faa-273">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-273">Boolean</span></span>|<span data-ttu-id="67faa-274">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="67faa-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="67faa-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-276">Boolean</span></span>|<span data-ttu-id="67faa-277">Indica se a tela Weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="67faa-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-278">passCodeDisabled</span></span>|<span data-ttu-id="67faa-279">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-279">Boolean</span></span>|<span data-ttu-id="67faa-280">Indica se o painel de configuração senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="67faa-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="67faa-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-281">zoomDisabled</span></span>|<span data-ttu-id="67faa-282">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-282">Boolean</span></span>|<span data-ttu-id="67faa-283">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="67faa-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="67faa-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="67faa-285">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-285">Boolean</span></span>|<span data-ttu-id="67faa-286">Indica se a tela Weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="67faa-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="67faa-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="67faa-288">Booleano</span><span class="sxs-lookup"><span data-stu-id="67faa-288">Boolean</span></span>|<span data-ttu-id="67faa-289">Indica se a tela Weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="67faa-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="67faa-290">Resposta</span><span class="sxs-lookup"><span data-stu-id="67faa-290">Response</span></span>
<span data-ttu-id="67faa-291">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="67faa-291">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67faa-292">Exemplo</span><span class="sxs-lookup"><span data-stu-id="67faa-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="67faa-293">Solicitação</span><span class="sxs-lookup"><span data-stu-id="67faa-293">Request</span></span>
<span data-ttu-id="67faa-294">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="67faa-294">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 2108

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="67faa-295">Resposta</span><span class="sxs-lookup"><span data-stu-id="67faa-295">Response</span></span>
<span data-ttu-id="67faa-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="67faa-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 2157

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "Support Department value",
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
  "iTunesPairingMode": "allow",
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreFromAndroidDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true,
  "companyPortalVppTokenId": "Company Portal Vpp Token Id value",
  "enableSingleAppEnrollmentMode": true,
  "homeButtonScreenDisabled": true,
  "iMessageAndFaceTimeScreenDisabled": true,
  "onBoardingScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```




