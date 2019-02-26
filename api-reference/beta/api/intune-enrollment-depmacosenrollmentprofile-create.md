---
title: Criar depMacOSEnrollmentProfile
description: Criar um novo objeto depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dbd5abc203f8391b038454c0995668487a9466e
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30164621"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="58a09-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="58a09-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="58a09-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="58a09-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58a09-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58a09-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a09-106">Criar um novo objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="58a09-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a09-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58a09-107">Prerequisites</span></span>
<span data-ttu-id="58a09-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="58a09-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58a09-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58a09-110">Permission type</span></span>|<span data-ttu-id="58a09-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58a09-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a09-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58a09-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58a09-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a09-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="58a09-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58a09-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a09-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a09-115">Not supported.</span></span>|
|<span data-ttu-id="58a09-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58a09-116">Application</span></span>|<span data-ttu-id="58a09-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a09-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a09-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58a09-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="58a09-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58a09-119">Request headers</span></span>
|<span data-ttu-id="58a09-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58a09-120">Header</span></span>|<span data-ttu-id="58a09-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58a09-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a09-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58a09-122">Authorization</span></span>|<span data-ttu-id="58a09-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58a09-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a09-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58a09-124">Accept</span></span>|<span data-ttu-id="58a09-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58a09-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a09-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58a09-126">Request body</span></span>
<span data-ttu-id="58a09-127">No corpo da solicitação, forneça uma representação JSON do objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="58a09-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="58a09-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="58a09-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="58a09-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58a09-129">Property</span></span>|<span data-ttu-id="58a09-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58a09-130">Type</span></span>|<span data-ttu-id="58a09-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58a09-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a09-132">id</span><span class="sxs-lookup"><span data-stu-id="58a09-132">id</span></span>|<span data-ttu-id="58a09-133">String</span><span class="sxs-lookup"><span data-stu-id="58a09-133">String</span></span>|<span data-ttu-id="58a09-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-135">displayName</span><span class="sxs-lookup"><span data-stu-id="58a09-135">displayName</span></span>|<span data-ttu-id="58a09-136">String</span><span class="sxs-lookup"><span data-stu-id="58a09-136">String</span></span>|<span data-ttu-id="58a09-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-138">description</span><span class="sxs-lookup"><span data-stu-id="58a09-138">description</span></span>|<span data-ttu-id="58a09-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="58a09-139">String</span></span>|<span data-ttu-id="58a09-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="58a09-141">requiresUserAuthentication</span></span>|<span data-ttu-id="58a09-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-142">Boolean</span></span>|<span data-ttu-id="58a09-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="58a09-144">configurationEndpointUrl</span></span>|<span data-ttu-id="58a09-145">String</span><span class="sxs-lookup"><span data-stu-id="58a09-145">String</span></span>|<span data-ttu-id="58a09-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="58a09-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="58a09-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-148">Boolean</span></span>|<span data-ttu-id="58a09-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="58a09-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="58a09-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="58a09-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="58a09-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-152">Boolean</span></span>|<span data-ttu-id="58a09-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="58a09-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="58a09-154">isDefault</span></span>|<span data-ttu-id="58a09-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-155">Boolean</span></span>|<span data-ttu-id="58a09-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="58a09-157">supervisedModeEnabled</span></span>|<span data-ttu-id="58a09-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-158">Boolean</span></span>|<span data-ttu-id="58a09-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="58a09-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="58a09-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="58a09-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="58a09-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="58a09-162">supportDepartment</span></span>|<span data-ttu-id="58a09-163">String</span><span class="sxs-lookup"><span data-stu-id="58a09-163">String</span></span>|<span data-ttu-id="58a09-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-165">passCodeDisabled</span></span>|<span data-ttu-id="58a09-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-166">Boolean</span></span>|<span data-ttu-id="58a09-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="58a09-168">isMandatory</span></span>|<span data-ttu-id="58a09-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-169">Boolean</span></span>|<span data-ttu-id="58a09-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-171">locationDisabled</span></span>|<span data-ttu-id="58a09-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-172">Boolean</span></span>|<span data-ttu-id="58a09-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="58a09-174">supportPhoneNumber</span></span>|<span data-ttu-id="58a09-175">String</span><span class="sxs-lookup"><span data-stu-id="58a09-175">String</span></span>|<span data-ttu-id="58a09-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-177">profileRemovalDisabled</span></span>|<span data-ttu-id="58a09-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-178">Boolean</span></span>|<span data-ttu-id="58a09-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="58a09-180">restoreBlocked</span></span>|<span data-ttu-id="58a09-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-181">Boolean</span></span>|<span data-ttu-id="58a09-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-183">appleIdDisabled</span></span>|<span data-ttu-id="58a09-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-184">Boolean</span></span>|<span data-ttu-id="58a09-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="58a09-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-187">Boolean</span></span>|<span data-ttu-id="58a09-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-189">touchIdDisabled</span></span>|<span data-ttu-id="58a09-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-190">Boolean</span></span>|<span data-ttu-id="58a09-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-192">applePayDisabled</span></span>|<span data-ttu-id="58a09-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-193">Boolean</span></span>|<span data-ttu-id="58a09-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-195">zoomDisabled</span></span>|<span data-ttu-id="58a09-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-196">Boolean</span></span>|<span data-ttu-id="58a09-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-198">siriDisabled</span></span>|<span data-ttu-id="58a09-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-199">Boolean</span></span>|<span data-ttu-id="58a09-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-201">diagnosticsDisabled</span></span>|<span data-ttu-id="58a09-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-202">Boolean</span></span>|<span data-ttu-id="58a09-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="58a09-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-205">Boolean</span></span>|<span data-ttu-id="58a09-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-207">privacyPaneDisabled</span></span>|<span data-ttu-id="58a09-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-208">Boolean</span></span>|<span data-ttu-id="58a09-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="58a09-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="58a09-210">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-210">registrationDisabled</span></span>|<span data-ttu-id="58a09-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-211">Boolean</span></span>|<span data-ttu-id="58a09-212">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="58a09-212">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="58a09-213">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-213">fileVaultDisabled</span></span>|<span data-ttu-id="58a09-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-214">Boolean</span></span>|<span data-ttu-id="58a09-215">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="58a09-215">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="58a09-216">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="58a09-216">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="58a09-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a09-217">Boolean</span></span>|<span data-ttu-id="58a09-218">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="58a09-218">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="58a09-219">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a09-219">Response</span></span>
<span data-ttu-id="58a09-220">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a09-220">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a09-221">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58a09-221">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a09-222">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58a09-222">Request</span></span>
<span data-ttu-id="58a09-223">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58a09-223">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1061

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
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="58a09-224">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a09-224">Response</span></span>
<span data-ttu-id="58a09-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58a09-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

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
  "iCloudDiagnosticsDisabled": true
}
```




