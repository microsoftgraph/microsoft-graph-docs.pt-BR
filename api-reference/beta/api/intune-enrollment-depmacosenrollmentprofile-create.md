---
title: Criar depMacOSEnrollmentProfile
description: Criar um novo objeto depMacOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cff4bea7e36c8e973e33af5aba9c8ce538afb4be
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201937"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="543cf-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="543cf-103">Create depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="543cf-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="543cf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="543cf-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="543cf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="543cf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="543cf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="543cf-107">Criar um novo objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="543cf-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="543cf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="543cf-108">Prerequisites</span></span>
<span data-ttu-id="543cf-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="543cf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="543cf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="543cf-111">Permission type</span></span>|<span data-ttu-id="543cf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="543cf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="543cf-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="543cf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="543cf-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543cf-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="543cf-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="543cf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="543cf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="543cf-116">Not supported.</span></span>|
|<span data-ttu-id="543cf-117">Application</span><span class="sxs-lookup"><span data-stu-id="543cf-117">Application</span></span>|<span data-ttu-id="543cf-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="543cf-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="543cf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="543cf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="543cf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="543cf-120">Request headers</span></span>
|<span data-ttu-id="543cf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="543cf-121">Header</span></span>|<span data-ttu-id="543cf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="543cf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="543cf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="543cf-123">Authorization</span></span>|<span data-ttu-id="543cf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="543cf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="543cf-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="543cf-125">Accept</span></span>|<span data-ttu-id="543cf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="543cf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="543cf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="543cf-127">Request body</span></span>
<span data-ttu-id="543cf-128">No corpo da solicitação, forneça uma representação JSON do objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="543cf-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="543cf-129">A tabela a seguir mostra as propriedades que são necessárias ao criar depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="543cf-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="543cf-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="543cf-130">Property</span></span>|<span data-ttu-id="543cf-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="543cf-131">Type</span></span>|<span data-ttu-id="543cf-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="543cf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="543cf-133">id</span><span class="sxs-lookup"><span data-stu-id="543cf-133">id</span></span>|<span data-ttu-id="543cf-134">String</span><span class="sxs-lookup"><span data-stu-id="543cf-134">String</span></span>|<span data-ttu-id="543cf-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-136">displayName</span><span class="sxs-lookup"><span data-stu-id="543cf-136">displayName</span></span>|<span data-ttu-id="543cf-137">String</span><span class="sxs-lookup"><span data-stu-id="543cf-137">String</span></span>|<span data-ttu-id="543cf-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-139">description</span><span class="sxs-lookup"><span data-stu-id="543cf-139">description</span></span>|<span data-ttu-id="543cf-140">String</span><span class="sxs-lookup"><span data-stu-id="543cf-140">String</span></span>|<span data-ttu-id="543cf-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="543cf-142">requiresUserAuthentication</span></span>|<span data-ttu-id="543cf-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-143">Boolean</span></span>|<span data-ttu-id="543cf-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="543cf-145">configurationEndpointUrl</span></span>|<span data-ttu-id="543cf-146">String</span><span class="sxs-lookup"><span data-stu-id="543cf-146">String</span></span>|<span data-ttu-id="543cf-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="543cf-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="543cf-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-149">Boolean</span></span>|<span data-ttu-id="543cf-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="543cf-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="543cf-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="543cf-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="543cf-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-153">Boolean</span></span>|<span data-ttu-id="543cf-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="543cf-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="543cf-155">isDefault</span></span>|<span data-ttu-id="543cf-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-156">Boolean</span></span>|<span data-ttu-id="543cf-157">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="543cf-158">supervisedModeEnabled</span></span>|<span data-ttu-id="543cf-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-159">Boolean</span></span>|<span data-ttu-id="543cf-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="543cf-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="543cf-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="543cf-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="543cf-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="543cf-163">supportDepartment</span></span>|<span data-ttu-id="543cf-164">String</span><span class="sxs-lookup"><span data-stu-id="543cf-164">String</span></span>|<span data-ttu-id="543cf-165">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-166">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="543cf-166">isMandatory</span></span>|<span data-ttu-id="543cf-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-167">Boolean</span></span>|<span data-ttu-id="543cf-168">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-169">locationDisabled</span></span>|<span data-ttu-id="543cf-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-170">Boolean</span></span>|<span data-ttu-id="543cf-171">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="543cf-172">supportPhoneNumber</span></span>|<span data-ttu-id="543cf-173">String</span><span class="sxs-lookup"><span data-stu-id="543cf-173">String</span></span>|<span data-ttu-id="543cf-174">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-175">profileRemovalDisabled</span></span>|<span data-ttu-id="543cf-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-176">Boolean</span></span>|<span data-ttu-id="543cf-177">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="543cf-178">restoreBlocked</span></span>|<span data-ttu-id="543cf-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-179">Boolean</span></span>|<span data-ttu-id="543cf-180">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-181">appleIdDisabled</span></span>|<span data-ttu-id="543cf-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-182">Boolean</span></span>|<span data-ttu-id="543cf-183">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="543cf-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-185">Boolean</span></span>|<span data-ttu-id="543cf-186">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-187">touchIdDisabled</span></span>|<span data-ttu-id="543cf-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-188">Boolean</span></span>|<span data-ttu-id="543cf-189">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-190">applePayDisabled</span></span>|<span data-ttu-id="543cf-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-191">Boolean</span></span>|<span data-ttu-id="543cf-192">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-193">siriDisabled</span></span>|<span data-ttu-id="543cf-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-194">Boolean</span></span>|<span data-ttu-id="543cf-195">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-196">diagnosticsDisabled</span></span>|<span data-ttu-id="543cf-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-197">Boolean</span></span>|<span data-ttu-id="543cf-198">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="543cf-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-200">Boolean</span></span>|<span data-ttu-id="543cf-201">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-202">privacyPaneDisabled</span></span>|<span data-ttu-id="543cf-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-203">Boolean</span></span>|<span data-ttu-id="543cf-204">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="543cf-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-206">Boolean</span></span>|<span data-ttu-id="543cf-207">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="543cf-208">deviceNameTemplate</span></span>|<span data-ttu-id="543cf-209">String</span><span class="sxs-lookup"><span data-stu-id="543cf-209">String</span></span>|<span data-ttu-id="543cf-210">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="543cf-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="543cf-211">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="543cf-212">configurationWebUrl</span></span>|<span data-ttu-id="543cf-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-213">Boolean</span></span>|<span data-ttu-id="543cf-214">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="543cf-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="543cf-215">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-215">registrationDisabled</span></span>|<span data-ttu-id="543cf-216">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-216">Boolean</span></span>|<span data-ttu-id="543cf-217">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="543cf-217">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="543cf-218">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-218">fileVaultDisabled</span></span>|<span data-ttu-id="543cf-219">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-219">Boolean</span></span>|<span data-ttu-id="543cf-220">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="543cf-220">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="543cf-221">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-221">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="543cf-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-222">Boolean</span></span>|<span data-ttu-id="543cf-223">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="543cf-223">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="543cf-224">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-224">passCodeDisabled</span></span>|<span data-ttu-id="543cf-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-225">Boolean</span></span>|<span data-ttu-id="543cf-226">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="543cf-226">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="543cf-227">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-227">zoomDisabled</span></span>|<span data-ttu-id="543cf-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-228">Boolean</span></span>|<span data-ttu-id="543cf-229">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="543cf-229">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="543cf-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="543cf-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-231">Boolean</span></span>|<span data-ttu-id="543cf-232">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="543cf-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="543cf-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="543cf-234">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-234">Boolean</span></span>|<span data-ttu-id="543cf-235">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="543cf-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="543cf-236">accessibilityScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="543cf-236">accessibilityScreenDisabled</span></span>|<span data-ttu-id="543cf-237">Booliano</span><span class="sxs-lookup"><span data-stu-id="543cf-237">Boolean</span></span>|<span data-ttu-id="543cf-238">Indica se a tela de acessibilidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="543cf-238">Indicates if Accessibility screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="543cf-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="543cf-239">Response</span></span>
<span data-ttu-id="543cf-240">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="543cf-240">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="543cf-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="543cf-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="543cf-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="543cf-242">Request</span></span>
<span data-ttu-id="543cf-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="543cf-243">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="543cf-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="543cf-244">Response</span></span>
<span data-ttu-id="543cf-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="543cf-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




