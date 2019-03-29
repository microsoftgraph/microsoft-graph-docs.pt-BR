---
title: Criar depMacOSEnrollmentProfile
description: Criar um novo objeto depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b1d78668b77035e9a8fd9461214f8b47affe22ad
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30967045"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="651dc-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="651dc-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="651dc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="651dc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="651dc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="651dc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="651dc-106">Criar um novo objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="651dc-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="651dc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="651dc-107">Prerequisites</span></span>
<span data-ttu-id="651dc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="651dc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="651dc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="651dc-110">Permission type</span></span>|<span data-ttu-id="651dc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="651dc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="651dc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="651dc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="651dc-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="651dc-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="651dc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="651dc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="651dc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="651dc-115">Not supported.</span></span>|
|<span data-ttu-id="651dc-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="651dc-116">Application</span></span>|<span data-ttu-id="651dc-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="651dc-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="651dc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="651dc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="651dc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="651dc-119">Request headers</span></span>
|<span data-ttu-id="651dc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="651dc-120">Header</span></span>|<span data-ttu-id="651dc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="651dc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="651dc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="651dc-122">Authorization</span></span>|<span data-ttu-id="651dc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="651dc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="651dc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="651dc-124">Accept</span></span>|<span data-ttu-id="651dc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="651dc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="651dc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="651dc-126">Request body</span></span>
<span data-ttu-id="651dc-127">No corpo da solicitação, forneça uma representação JSON do objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="651dc-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="651dc-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="651dc-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="651dc-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="651dc-129">Property</span></span>|<span data-ttu-id="651dc-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="651dc-130">Type</span></span>|<span data-ttu-id="651dc-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="651dc-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="651dc-132">id</span><span class="sxs-lookup"><span data-stu-id="651dc-132">id</span></span>|<span data-ttu-id="651dc-133">String</span><span class="sxs-lookup"><span data-stu-id="651dc-133">String</span></span>|<span data-ttu-id="651dc-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-135">displayName</span><span class="sxs-lookup"><span data-stu-id="651dc-135">displayName</span></span>|<span data-ttu-id="651dc-136">String</span><span class="sxs-lookup"><span data-stu-id="651dc-136">String</span></span>|<span data-ttu-id="651dc-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-138">descrição</span><span class="sxs-lookup"><span data-stu-id="651dc-138">description</span></span>|<span data-ttu-id="651dc-139">String</span><span class="sxs-lookup"><span data-stu-id="651dc-139">String</span></span>|<span data-ttu-id="651dc-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="651dc-141">requiresUserAuthentication</span></span>|<span data-ttu-id="651dc-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-142">Boolean</span></span>|<span data-ttu-id="651dc-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="651dc-144">configurationEndpointUrl</span></span>|<span data-ttu-id="651dc-145">String</span><span class="sxs-lookup"><span data-stu-id="651dc-145">String</span></span>|<span data-ttu-id="651dc-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="651dc-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="651dc-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-148">Boolean</span></span>|<span data-ttu-id="651dc-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="651dc-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="651dc-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="651dc-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="651dc-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-152">Boolean</span></span>|<span data-ttu-id="651dc-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="651dc-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="651dc-154">isDefault</span></span>|<span data-ttu-id="651dc-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="651dc-155">Boolean</span></span>|<span data-ttu-id="651dc-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="651dc-157">supervisedModeEnabled</span></span>|<span data-ttu-id="651dc-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-158">Boolean</span></span>|<span data-ttu-id="651dc-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="651dc-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="651dc-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="651dc-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="651dc-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="651dc-162">supportDepartment</span></span>|<span data-ttu-id="651dc-163">String</span><span class="sxs-lookup"><span data-stu-id="651dc-163">String</span></span>|<span data-ttu-id="651dc-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-165">passCodeDisabled</span></span>|<span data-ttu-id="651dc-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-166">Boolean</span></span>|<span data-ttu-id="651dc-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="651dc-168">isMandatory</span></span>|<span data-ttu-id="651dc-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-169">Boolean</span></span>|<span data-ttu-id="651dc-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-171">locationDisabled</span></span>|<span data-ttu-id="651dc-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-172">Boolean</span></span>|<span data-ttu-id="651dc-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="651dc-174">supportPhoneNumber</span></span>|<span data-ttu-id="651dc-175">String</span><span class="sxs-lookup"><span data-stu-id="651dc-175">String</span></span>|<span data-ttu-id="651dc-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-177">profileRemovalDisabled</span></span>|<span data-ttu-id="651dc-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-178">Boolean</span></span>|<span data-ttu-id="651dc-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="651dc-180">restoreBlocked</span></span>|<span data-ttu-id="651dc-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-181">Boolean</span></span>|<span data-ttu-id="651dc-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-183">appleIdDisabled</span></span>|<span data-ttu-id="651dc-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-184">Boolean</span></span>|<span data-ttu-id="651dc-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="651dc-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-187">Boolean</span></span>|<span data-ttu-id="651dc-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-189">touchIdDisabled</span></span>|<span data-ttu-id="651dc-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-190">Boolean</span></span>|<span data-ttu-id="651dc-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-192">applePayDisabled</span></span>|<span data-ttu-id="651dc-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-193">Boolean</span></span>|<span data-ttu-id="651dc-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-195">zoomDisabled</span></span>|<span data-ttu-id="651dc-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-196">Boolean</span></span>|<span data-ttu-id="651dc-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-198">siriDisabled</span></span>|<span data-ttu-id="651dc-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-199">Boolean</span></span>|<span data-ttu-id="651dc-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-201">diagnosticsDisabled</span></span>|<span data-ttu-id="651dc-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-202">Boolean</span></span>|<span data-ttu-id="651dc-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="651dc-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-205">Boolean</span></span>|<span data-ttu-id="651dc-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-207">privacyPaneDisabled</span></span>|<span data-ttu-id="651dc-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-208">Boolean</span></span>|<span data-ttu-id="651dc-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="651dc-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="651dc-210">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-210">registrationDisabled</span></span>|<span data-ttu-id="651dc-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-211">Boolean</span></span>|<span data-ttu-id="651dc-212">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="651dc-212">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="651dc-213">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-213">fileVaultDisabled</span></span>|<span data-ttu-id="651dc-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-214">Boolean</span></span>|<span data-ttu-id="651dc-215">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="651dc-215">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="651dc-216">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-216">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="651dc-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-217">Boolean</span></span>|<span data-ttu-id="651dc-218">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="651dc-218">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="651dc-219">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-219">iCloudStorageDisabled</span></span>|<span data-ttu-id="651dc-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-220">Boolean</span></span>|<span data-ttu-id="651dc-221">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="651dc-221">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="651dc-222">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="651dc-222">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="651dc-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="651dc-223">Boolean</span></span>|<span data-ttu-id="651dc-224">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="651dc-224">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="651dc-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="651dc-225">Response</span></span>
<span data-ttu-id="651dc-226">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="651dc-226">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="651dc-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="651dc-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="651dc-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="651dc-228">Request</span></span>
<span data-ttu-id="651dc-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="651dc-229">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1136

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="651dc-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="651dc-230">Response</span></span>
<span data-ttu-id="651dc-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="651dc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1185

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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




