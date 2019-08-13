---
title: Criar depIOSEnrollmentProfile
description: Criar um novo objeto depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aa03e61f1b2ad66aa55ea9dce7aa2ed6c58b5c41
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36309720"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="99d70-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="99d70-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="99d70-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="99d70-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99d70-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99d70-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99d70-106">Criar um novo objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="99d70-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99d70-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="99d70-107">Prerequisites</span></span>
<span data-ttu-id="99d70-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="99d70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99d70-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="99d70-110">Permission type</span></span>|<span data-ttu-id="99d70-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="99d70-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99d70-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="99d70-112">Delegated (work or school account)</span></span>|<span data-ttu-id="99d70-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d70-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="99d70-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="99d70-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99d70-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="99d70-115">Not supported.</span></span>|
|<span data-ttu-id="99d70-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="99d70-116">Application</span></span>|<span data-ttu-id="99d70-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99d70-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99d70-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="99d70-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="99d70-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="99d70-119">Request headers</span></span>
|<span data-ttu-id="99d70-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="99d70-120">Header</span></span>|<span data-ttu-id="99d70-121">Valor</span><span class="sxs-lookup"><span data-stu-id="99d70-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99d70-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="99d70-122">Authorization</span></span>|<span data-ttu-id="99d70-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="99d70-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99d70-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="99d70-124">Accept</span></span>|<span data-ttu-id="99d70-125">application/json</span><span class="sxs-lookup"><span data-stu-id="99d70-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99d70-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="99d70-126">Request body</span></span>
<span data-ttu-id="99d70-127">No corpo da solicitação, forneça uma representação JSON do objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="99d70-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="99d70-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="99d70-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="99d70-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99d70-129">Property</span></span>|<span data-ttu-id="99d70-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="99d70-130">Type</span></span>|<span data-ttu-id="99d70-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="99d70-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99d70-132">id</span><span class="sxs-lookup"><span data-stu-id="99d70-132">id</span></span>|<span data-ttu-id="99d70-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="99d70-133">String</span></span>|<span data-ttu-id="99d70-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-135">displayName</span><span class="sxs-lookup"><span data-stu-id="99d70-135">displayName</span></span>|<span data-ttu-id="99d70-136">String</span><span class="sxs-lookup"><span data-stu-id="99d70-136">String</span></span>|<span data-ttu-id="99d70-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-138">descrição</span><span class="sxs-lookup"><span data-stu-id="99d70-138">description</span></span>|<span data-ttu-id="99d70-139">String</span><span class="sxs-lookup"><span data-stu-id="99d70-139">String</span></span>|<span data-ttu-id="99d70-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="99d70-141">requiresUserAuthentication</span></span>|<span data-ttu-id="99d70-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-142">Boolean</span></span>|<span data-ttu-id="99d70-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="99d70-144">configurationEndpointUrl</span></span>|<span data-ttu-id="99d70-145">String</span><span class="sxs-lookup"><span data-stu-id="99d70-145">String</span></span>|<span data-ttu-id="99d70-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="99d70-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="99d70-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-148">Boolean</span></span>|<span data-ttu-id="99d70-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="99d70-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="99d70-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="99d70-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="99d70-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-152">Boolean</span></span>|<span data-ttu-id="99d70-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="99d70-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="99d70-154">isDefault</span></span>|<span data-ttu-id="99d70-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-155">Boolean</span></span>|<span data-ttu-id="99d70-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="99d70-157">supervisedModeEnabled</span></span>|<span data-ttu-id="99d70-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-158">Boolean</span></span>|<span data-ttu-id="99d70-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="99d70-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="99d70-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="99d70-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="99d70-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="99d70-162">supportDepartment</span></span>|<span data-ttu-id="99d70-163">String</span><span class="sxs-lookup"><span data-stu-id="99d70-163">String</span></span>|<span data-ttu-id="99d70-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-165">passCodeDisabled</span></span>|<span data-ttu-id="99d70-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-166">Boolean</span></span>|<span data-ttu-id="99d70-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="99d70-168">isMandatory</span></span>|<span data-ttu-id="99d70-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-169">Boolean</span></span>|<span data-ttu-id="99d70-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-171">locationDisabled</span></span>|<span data-ttu-id="99d70-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-172">Boolean</span></span>|<span data-ttu-id="99d70-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="99d70-174">supportPhoneNumber</span></span>|<span data-ttu-id="99d70-175">String</span><span class="sxs-lookup"><span data-stu-id="99d70-175">String</span></span>|<span data-ttu-id="99d70-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-177">profileRemovalDisabled</span></span>|<span data-ttu-id="99d70-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-178">Boolean</span></span>|<span data-ttu-id="99d70-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="99d70-180">restoreBlocked</span></span>|<span data-ttu-id="99d70-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-181">Boolean</span></span>|<span data-ttu-id="99d70-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-183">appleIdDisabled</span></span>|<span data-ttu-id="99d70-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-184">Boolean</span></span>|<span data-ttu-id="99d70-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="99d70-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-187">Boolean</span></span>|<span data-ttu-id="99d70-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-189">touchIdDisabled</span></span>|<span data-ttu-id="99d70-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-190">Boolean</span></span>|<span data-ttu-id="99d70-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-192">applePayDisabled</span></span>|<span data-ttu-id="99d70-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-193">Boolean</span></span>|<span data-ttu-id="99d70-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-195">zoomDisabled</span></span>|<span data-ttu-id="99d70-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-196">Boolean</span></span>|<span data-ttu-id="99d70-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-198">siriDisabled</span></span>|<span data-ttu-id="99d70-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-199">Boolean</span></span>|<span data-ttu-id="99d70-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-201">diagnosticsDisabled</span></span>|<span data-ttu-id="99d70-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-202">Boolean</span></span>|<span data-ttu-id="99d70-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="99d70-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-205">Boolean</span></span>|<span data-ttu-id="99d70-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-207">privacyPaneDisabled</span></span>|<span data-ttu-id="99d70-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-208">Boolean</span></span>|<span data-ttu-id="99d70-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="99d70-210">deviceNameTemplate</span></span>|<span data-ttu-id="99d70-211">String</span><span class="sxs-lookup"><span data-stu-id="99d70-211">String</span></span>|<span data-ttu-id="99d70-212">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="99d70-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="99d70-213">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="99d70-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="99d70-214">iTunesPairingMode</span></span>|[<span data-ttu-id="99d70-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="99d70-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="99d70-216">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="99d70-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="99d70-217">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="99d70-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="99d70-218">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="99d70-218">managementCertificates</span></span>|<span data-ttu-id="99d70-219">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="99d70-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="99d70-220">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="99d70-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="99d70-221">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="99d70-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-222">Boolean</span></span>|<span data-ttu-id="99d70-223">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="99d70-224">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="99d70-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="99d70-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-225">Boolean</span></span>|<span data-ttu-id="99d70-226">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="99d70-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="99d70-227">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="99d70-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="99d70-228">Int32</span><span class="sxs-lookup"><span data-stu-id="99d70-228">Int32</span></span>|<span data-ttu-id="99d70-229">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="99d70-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="99d70-230">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="99d70-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="99d70-231">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="99d70-231">enableSharedIPad</span></span>|<span data-ttu-id="99d70-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-232">Boolean</span></span>|<span data-ttu-id="99d70-233">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="99d70-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="99d70-234">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="99d70-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="99d70-235">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="99d70-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="99d70-236">String</span><span class="sxs-lookup"><span data-stu-id="99d70-236">String</span></span>|<span data-ttu-id="99d70-237">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="99d70-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="99d70-238">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="99d70-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="99d70-239">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="99d70-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="99d70-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-240">Boolean</span></span>|<span data-ttu-id="99d70-241">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="99d70-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="99d70-242">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="99d70-242">Default is false.</span></span> <span data-ttu-id="99d70-243">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="99d70-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="99d70-244">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="99d70-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-245">Boolean</span></span>|<span data-ttu-id="99d70-246">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="99d70-247">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="99d70-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-248">Boolean</span></span>|<span data-ttu-id="99d70-249">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="99d70-250">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="99d70-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-251">Boolean</span></span>|<span data-ttu-id="99d70-252">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="99d70-253">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="99d70-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-254">Boolean</span></span>|<span data-ttu-id="99d70-255">Indica se a configuração de tempo limite da tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="99d70-256">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="99d70-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-257">Boolean</span></span>|<span data-ttu-id="99d70-258">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="99d70-259">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="99d70-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-260">Boolean</span></span>|<span data-ttu-id="99d70-261">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="99d70-262">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="99d70-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="99d70-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="99d70-263">Boolean</span></span>|<span data-ttu-id="99d70-264">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="99d70-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="99d70-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="99d70-265">Response</span></span>
<span data-ttu-id="99d70-266">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="99d70-266">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99d70-267">Exemplo</span><span class="sxs-lookup"><span data-stu-id="99d70-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="99d70-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="99d70-268">Request</span></span>
<span data-ttu-id="99d70-269">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="99d70-269">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1791

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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="99d70-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="99d70-270">Response</span></span>
<span data-ttu-id="99d70-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="99d70-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1840

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
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "displayToneSetupDisabled": true,
  "privacyPaneDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
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
  "screenTimeScreenDisabled": true,
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true
}
```






