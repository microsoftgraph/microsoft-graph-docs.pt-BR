---
title: Criar depMacOSEnrollmentProfile
description: Crie um novo objeto depMacOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c83dfda95a05dea3699deccacee8ca77eef38e26
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145940"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="a237e-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="a237e-103">Create depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="a237e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a237e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a237e-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a237e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a237e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a237e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a237e-107">Crie um novo [objeto depMacOSEnrollmentProfile.](../resources/intune-enrollment-depmacosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a237e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a237e-108">Prerequisites</span></span>
<span data-ttu-id="a237e-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a237e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a237e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a237e-111">Permission type</span></span>|<span data-ttu-id="a237e-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a237e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a237e-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a237e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a237e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a237e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="a237e-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a237e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a237e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a237e-116">Not supported.</span></span>|
|<span data-ttu-id="a237e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a237e-117">Application</span></span>|<span data-ttu-id="a237e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a237e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a237e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a237e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="a237e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a237e-120">Request headers</span></span>
|<span data-ttu-id="a237e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a237e-121">Header</span></span>|<span data-ttu-id="a237e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a237e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a237e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a237e-123">Authorization</span></span>|<span data-ttu-id="a237e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a237e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a237e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a237e-125">Accept</span></span>|<span data-ttu-id="a237e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a237e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a237e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a237e-127">Request body</span></span>
<span data-ttu-id="a237e-128">No corpo da solicitação, fornece uma representação JSON para o objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a237e-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="a237e-129">A tabela a seguir mostra as propriedades necessárias ao criar o depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="a237e-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="a237e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a237e-130">Property</span></span>|<span data-ttu-id="a237e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a237e-131">Type</span></span>|<span data-ttu-id="a237e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a237e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a237e-133">id</span><span class="sxs-lookup"><span data-stu-id="a237e-133">id</span></span>|<span data-ttu-id="a237e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-134">String</span></span>|<span data-ttu-id="a237e-135">O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a237e-136">displayName</span></span>|<span data-ttu-id="a237e-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-137">String</span></span>|<span data-ttu-id="a237e-138">Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-139">descrição</span><span class="sxs-lookup"><span data-stu-id="a237e-139">description</span></span>|<span data-ttu-id="a237e-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-140">String</span></span>|<span data-ttu-id="a237e-141">Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="a237e-142">requiresUserAuthentication</span></span>|<span data-ttu-id="a237e-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-143">Boolean</span></span>|<span data-ttu-id="a237e-144">Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="a237e-145">configurationEndpointUrl</span></span>|<span data-ttu-id="a237e-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-146">String</span></span>|<span data-ttu-id="a237e-147">URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="a237e-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="a237e-149">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-149">Boolean</span></span>|<span data-ttu-id="a237e-150">Indica a autenticação com o Assistente de Instalação da Apple em vez do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="a237e-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="a237e-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="a237e-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="a237e-153">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-153">Boolean</span></span>|<span data-ttu-id="a237e-154">Indica que o Portal da Empresa é necessário em dispositivos inscritos pelo assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="a237e-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="a237e-155">isDefault</span></span>|<span data-ttu-id="a237e-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="a237e-156">Boolean</span></span>|<span data-ttu-id="a237e-157">Indica se esse é o perfil padrão Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="a237e-158">supervisedModeEnabled</span></span>|<span data-ttu-id="a237e-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-159">Boolean</span></span>|<span data-ttu-id="a237e-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="a237e-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="a237e-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a237e-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="a237e-162">Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="a237e-163">supportDepartment</span></span>|<span data-ttu-id="a237e-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-164">String</span></span>|<span data-ttu-id="a237e-165">Informações do departamento de suporte Herdadas [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="a237e-166">isMandatory</span></span>|<span data-ttu-id="a237e-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-167">Boolean</span></span>|<span data-ttu-id="a237e-168">Indica se o perfil é obrigatório Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-169">locationDisabled</span></span>|<span data-ttu-id="a237e-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-170">Boolean</span></span>|<span data-ttu-id="a237e-171">Indica se o painel de configuração do serviço de local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="a237e-172">supportPhoneNumber</span></span>|<span data-ttu-id="a237e-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-173">String</span></span>|<span data-ttu-id="a237e-174">Número de telefone de suporte Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-175">profileRemovalDisabled</span></span>|<span data-ttu-id="a237e-176">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-176">Boolean</span></span>|<span data-ttu-id="a237e-177">Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="a237e-178">restoreBlocked</span></span>|<span data-ttu-id="a237e-179">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-179">Boolean</span></span>|<span data-ttu-id="a237e-180">Indica se o painel restaurar instalação está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-181">appleIdDisabled</span></span>|<span data-ttu-id="a237e-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-182">Boolean</span></span>|<span data-ttu-id="a237e-183">Indica se o painel de configuração de ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="a237e-185">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-185">Boolean</span></span>|<span data-ttu-id="a237e-186">Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-187">touchIdDisabled</span></span>|<span data-ttu-id="a237e-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-188">Boolean</span></span>|<span data-ttu-id="a237e-189">Indica se o painel de configuração de id por toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-190">applePayDisabled</span></span>|<span data-ttu-id="a237e-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-191">Boolean</span></span>|<span data-ttu-id="a237e-192">Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-193">siriDisabled</span></span>|<span data-ttu-id="a237e-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-194">Boolean</span></span>|<span data-ttu-id="a237e-195">Indica se o painel de configuração de siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-196">diagnosticsDisabled</span></span>|<span data-ttu-id="a237e-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-197">Boolean</span></span>|<span data-ttu-id="a237e-198">Indica se o painel de configuração de diagnósticos está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="a237e-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-200">Boolean</span></span>|<span data-ttu-id="a237e-201">Indica se a tela de instalação de displaytone está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-202">privacyPaneDisabled</span></span>|<span data-ttu-id="a237e-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-203">Boolean</span></span>|<span data-ttu-id="a237e-204">Indica se a tela de privacidade está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="a237e-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-206">Boolean</span></span>|<span data-ttu-id="a237e-207">Indica se a configuração do tempo de tempo de tela está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="a237e-208">deviceNameTemplate</span></span>|<span data-ttu-id="a237e-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a237e-209">String</span></span>|<span data-ttu-id="a237e-210">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="a237e-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="a237e-211">Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="a237e-212">configurationWebUrl</span></span>|<span data-ttu-id="a237e-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-213">Boolean</span></span>|<span data-ttu-id="a237e-214">URL para logon do assistente de instalação Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="a237e-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="a237e-215">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-215">registrationDisabled</span></span>|<span data-ttu-id="a237e-216">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-216">Boolean</span></span>|<span data-ttu-id="a237e-217">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="a237e-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="a237e-218">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-218">fileVaultDisabled</span></span>|<span data-ttu-id="a237e-219">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-219">Boolean</span></span>|<span data-ttu-id="a237e-220">Indica se o cofre de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="a237e-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="a237e-221">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="a237e-222">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-222">Boolean</span></span>|<span data-ttu-id="a237e-223">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="a237e-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="a237e-224">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-224">passCodeDisabled</span></span>|<span data-ttu-id="a237e-225">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-225">Boolean</span></span>|<span data-ttu-id="a237e-226">Indica se o painel de configuração senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="a237e-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="a237e-227">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-227">zoomDisabled</span></span>|<span data-ttu-id="a237e-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-228">Boolean</span></span>|<span data-ttu-id="a237e-229">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="a237e-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="a237e-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="a237e-231">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-231">Boolean</span></span>|<span data-ttu-id="a237e-232">Indica se a tela documentos e área de trabalho do iCloud está desabilitada</span><span class="sxs-lookup"><span data-stu-id="a237e-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="a237e-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="a237e-234">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-234">Boolean</span></span>|<span data-ttu-id="a237e-235">Indica se a tela documentos e área de trabalho do iCloud está desabilitada</span><span class="sxs-lookup"><span data-stu-id="a237e-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="a237e-236">accessibilityScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="a237e-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="a237e-237">Booleano</span><span class="sxs-lookup"><span data-stu-id="a237e-237">Boolean</span></span>|<span data-ttu-id="a237e-238">Indica se a tela acessibilidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="a237e-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="a237e-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="a237e-239">Response</span></span>
<span data-ttu-id="a237e-240">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a237e-240">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a237e-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a237e-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="a237e-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a237e-242">Request</span></span>
<span data-ttu-id="a237e-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a237e-243">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1300

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="a237e-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="a237e-244">Response</span></span>
<span data-ttu-id="a237e-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a237e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1349

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true,
  "accessibilityScreenDisabled": true
}
```




