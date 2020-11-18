---
title: Criar depIOSEnrollmentProfile
description: Criar um novo objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f86a8924ffb254437838152e76499912a158086e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201979"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="8eb4d-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8eb4d-103">Create depIOSEnrollmentProfile</span></span>

<span data-ttu-id="8eb4d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eb4d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8eb4d-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8eb4d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8eb4d-107">Criar um novo objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8eb4d-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8eb4d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8eb4d-108">Prerequisites</span></span>
<span data-ttu-id="8eb4d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8eb4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eb4d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8eb4d-111">Permission type</span></span>|<span data-ttu-id="8eb4d-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8eb4d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8eb4d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb4d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8eb4d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8eb4d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-116">Not supported.</span></span>|
|<span data-ttu-id="8eb4d-117">Application</span><span class="sxs-lookup"><span data-stu-id="8eb4d-117">Application</span></span>|<span data-ttu-id="8eb4d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8eb4d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8eb4d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8eb4d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8eb4d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8eb4d-120">Request headers</span></span>
|<span data-ttu-id="8eb4d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8eb4d-121">Header</span></span>|<span data-ttu-id="8eb4d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8eb4d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8eb4d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8eb4d-123">Authorization</span></span>|<span data-ttu-id="8eb4d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8eb4d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8eb4d-125">Accept</span></span>|<span data-ttu-id="8eb4d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8eb4d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8eb4d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8eb4d-127">Request body</span></span>
<span data-ttu-id="8eb4d-128">No corpo da solicitação, forneça uma representação JSON do objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="8eb4d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="8eb4d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8eb4d-130">Property</span></span>|<span data-ttu-id="8eb4d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8eb4d-131">Type</span></span>|<span data-ttu-id="8eb4d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8eb4d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8eb4d-133">id</span><span class="sxs-lookup"><span data-stu-id="8eb4d-133">id</span></span>|<span data-ttu-id="8eb4d-134">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-134">String</span></span>|<span data-ttu-id="8eb4d-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8eb4d-136">displayName</span></span>|<span data-ttu-id="8eb4d-137">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-137">String</span></span>|<span data-ttu-id="8eb4d-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-139">description</span><span class="sxs-lookup"><span data-stu-id="8eb4d-139">description</span></span>|<span data-ttu-id="8eb4d-140">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-140">String</span></span>|<span data-ttu-id="8eb4d-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8eb4d-142">requiresUserAuthentication</span></span>|<span data-ttu-id="8eb4d-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-143">Boolean</span></span>|<span data-ttu-id="8eb4d-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="8eb4d-145">configurationEndpointUrl</span></span>|<span data-ttu-id="8eb4d-146">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-146">String</span></span>|<span data-ttu-id="8eb4d-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8eb4d-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-149">Boolean</span></span>|<span data-ttu-id="8eb4d-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="8eb4d-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="8eb4d-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="8eb4d-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-153">Boolean</span></span>|<span data-ttu-id="8eb4d-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="8eb4d-155">isDefault</span></span>|<span data-ttu-id="8eb4d-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-156">Boolean</span></span>|<span data-ttu-id="8eb4d-157">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-158">supervisedModeEnabled</span></span>|<span data-ttu-id="8eb4d-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-159">Boolean</span></span>|<span data-ttu-id="8eb4d-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="8eb4d-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="8eb4d-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="8eb4d-163">supportDepartment</span></span>|<span data-ttu-id="8eb4d-164">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-164">String</span></span>|<span data-ttu-id="8eb4d-165">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-166">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="8eb4d-166">isMandatory</span></span>|<span data-ttu-id="8eb4d-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-167">Boolean</span></span>|<span data-ttu-id="8eb4d-168">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-169">locationDisabled</span></span>|<span data-ttu-id="8eb4d-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-170">Boolean</span></span>|<span data-ttu-id="8eb4d-171">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8eb4d-172">supportPhoneNumber</span></span>|<span data-ttu-id="8eb4d-173">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-173">String</span></span>|<span data-ttu-id="8eb4d-174">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-175">profileRemovalDisabled</span></span>|<span data-ttu-id="8eb4d-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-176">Boolean</span></span>|<span data-ttu-id="8eb4d-177">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8eb4d-178">restoreBlocked</span></span>|<span data-ttu-id="8eb4d-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-179">Boolean</span></span>|<span data-ttu-id="8eb4d-180">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-181">appleIdDisabled</span></span>|<span data-ttu-id="8eb4d-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-182">Boolean</span></span>|<span data-ttu-id="8eb4d-183">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="8eb4d-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-185">Boolean</span></span>|<span data-ttu-id="8eb4d-186">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-187">touchIdDisabled</span></span>|<span data-ttu-id="8eb4d-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-188">Boolean</span></span>|<span data-ttu-id="8eb4d-189">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-190">applePayDisabled</span></span>|<span data-ttu-id="8eb4d-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-191">Boolean</span></span>|<span data-ttu-id="8eb4d-192">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-193">siriDisabled</span></span>|<span data-ttu-id="8eb4d-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-194">Boolean</span></span>|<span data-ttu-id="8eb4d-195">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-196">diagnosticsDisabled</span></span>|<span data-ttu-id="8eb4d-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-197">Boolean</span></span>|<span data-ttu-id="8eb4d-198">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="8eb4d-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-200">Boolean</span></span>|<span data-ttu-id="8eb4d-201">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-202">privacyPaneDisabled</span></span>|<span data-ttu-id="8eb4d-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-203">Boolean</span></span>|<span data-ttu-id="8eb4d-204">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="8eb4d-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-206">Boolean</span></span>|<span data-ttu-id="8eb4d-207">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="8eb4d-208">deviceNameTemplate</span></span>|<span data-ttu-id="8eb4d-209">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-209">String</span></span>|<span data-ttu-id="8eb4d-210">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="8eb4d-211">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="8eb4d-212">configurationWebUrl</span></span>|<span data-ttu-id="8eb4d-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-213">Boolean</span></span>|<span data-ttu-id="8eb4d-214">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8eb4d-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8eb4d-215">iTunesPairingMode</span></span>|[<span data-ttu-id="8eb4d-216">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8eb4d-216">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="8eb4d-217">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="8eb4d-218">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="8eb4d-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="8eb4d-219">managementCertificates</span></span>|<span data-ttu-id="8eb4d-220">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="8eb4d-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="8eb4d-221">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="8eb4d-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="8eb4d-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="8eb4d-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-223">Boolean</span></span>|<span data-ttu-id="8eb4d-224">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="8eb4d-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="8eb4d-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="8eb4d-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-226">Boolean</span></span>|<span data-ttu-id="8eb4d-227">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="8eb4d-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="8eb4d-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="8eb4d-229">Int32</span><span class="sxs-lookup"><span data-stu-id="8eb4d-229">Int32</span></span>|<span data-ttu-id="8eb4d-230">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="8eb4d-231">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="8eb4d-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="8eb4d-232">enableSharedIPad</span></span>|<span data-ttu-id="8eb4d-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-233">Boolean</span></span>|<span data-ttu-id="8eb4d-234">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="8eb4d-235">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="8eb4d-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="8eb4d-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="8eb4d-237">String</span><span class="sxs-lookup"><span data-stu-id="8eb4d-237">String</span></span>|<span data-ttu-id="8eb4d-238">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="8eb4d-239">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="8eb4d-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="8eb4d-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="8eb4d-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-241">Boolean</span></span>|<span data-ttu-id="8eb4d-242">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="8eb4d-243">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-243">Default is false.</span></span> <span data-ttu-id="8eb4d-244">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="8eb4d-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="8eb4d-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-246">Boolean</span></span>|<span data-ttu-id="8eb4d-247">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="8eb4d-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-249">Boolean</span></span>|<span data-ttu-id="8eb4d-250">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="8eb4d-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-252">Boolean</span></span>|<span data-ttu-id="8eb4d-253">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="8eb4d-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-255">Boolean</span></span>|<span data-ttu-id="8eb4d-256">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="8eb4d-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-258">Boolean</span></span>|<span data-ttu-id="8eb4d-259">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="8eb4d-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-261">Boolean</span></span>|<span data-ttu-id="8eb4d-262">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="8eb4d-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-264">Boolean</span></span>|<span data-ttu-id="8eb4d-265">Indica se a tela do apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="8eb4d-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-267">Boolean</span></span>|<span data-ttu-id="8eb4d-268">Indica se a tela de idioma expresso está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="8eb4d-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-270">Boolean</span></span>|<span data-ttu-id="8eb4d-271">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="8eb4d-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-273">Boolean</span></span>|<span data-ttu-id="8eb4d-274">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="8eb4d-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="8eb4d-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-276">Boolean</span></span>|<span data-ttu-id="8eb4d-277">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-278">passCodeDisabled</span></span>|<span data-ttu-id="8eb4d-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-279">Boolean</span></span>|<span data-ttu-id="8eb4d-280">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8eb4d-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="8eb4d-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-281">zoomDisabled</span></span>|<span data-ttu-id="8eb4d-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-282">Boolean</span></span>|<span data-ttu-id="8eb4d-283">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8eb4d-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="8eb4d-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="8eb4d-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-285">Boolean</span></span>|<span data-ttu-id="8eb4d-286">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="8eb4d-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8eb4d-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="8eb4d-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="8eb4d-288">Boolean</span></span>|<span data-ttu-id="8eb4d-289">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8eb4d-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="8eb4d-290">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eb4d-290">Response</span></span>
<span data-ttu-id="8eb4d-291">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-291">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eb4d-292">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8eb4d-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="8eb4d-293">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8eb4d-293">Request</span></span>
<span data-ttu-id="8eb4d-294">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-294">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8eb4d-295">Resposta</span><span class="sxs-lookup"><span data-stu-id="8eb4d-295">Response</span></span>
<span data-ttu-id="8eb4d-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8eb4d-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




