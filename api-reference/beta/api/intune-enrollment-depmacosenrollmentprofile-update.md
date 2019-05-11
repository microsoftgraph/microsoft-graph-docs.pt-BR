---
title: Atualizar depMacOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depMacOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 238676c0c1ea2019c6f505b55fb5db398d248d2b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908767"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="ac43b-103">Atualizar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ac43b-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="ac43b-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ac43b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ac43b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ac43b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac43b-106">Atualiza as propriedades de um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ac43b-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ac43b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ac43b-107">Prerequisites</span></span>
<span data-ttu-id="ac43b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ac43b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ac43b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ac43b-110">Permission type</span></span>|<span data-ttu-id="ac43b-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ac43b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ac43b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ac43b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ac43b-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ac43b-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ac43b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ac43b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac43b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac43b-115">Not supported.</span></span>|
|<span data-ttu-id="ac43b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ac43b-116">Application</span></span>|<span data-ttu-id="ac43b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ac43b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ac43b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ac43b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="ac43b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ac43b-119">Request headers</span></span>
|<span data-ttu-id="ac43b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ac43b-120">Header</span></span>|<span data-ttu-id="ac43b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="ac43b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ac43b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="ac43b-122">Authorization</span></span>|<span data-ttu-id="ac43b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ac43b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ac43b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ac43b-124">Accept</span></span>|<span data-ttu-id="ac43b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ac43b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac43b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ac43b-126">Request body</span></span>
<span data-ttu-id="ac43b-127">No corpo da solicitação, forneça uma representação JSON do objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ac43b-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="ac43b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="ac43b-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="ac43b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac43b-129">Property</span></span>|<span data-ttu-id="ac43b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac43b-130">Type</span></span>|<span data-ttu-id="ac43b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac43b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac43b-132">id</span><span class="sxs-lookup"><span data-stu-id="ac43b-132">id</span></span>|<span data-ttu-id="ac43b-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac43b-133">String</span></span>|<span data-ttu-id="ac43b-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-135">displayName</span><span class="sxs-lookup"><span data-stu-id="ac43b-135">displayName</span></span>|<span data-ttu-id="ac43b-136">String</span><span class="sxs-lookup"><span data-stu-id="ac43b-136">String</span></span>|<span data-ttu-id="ac43b-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-138">description</span><span class="sxs-lookup"><span data-stu-id="ac43b-138">description</span></span>|<span data-ttu-id="ac43b-139">String</span><span class="sxs-lookup"><span data-stu-id="ac43b-139">String</span></span>|<span data-ttu-id="ac43b-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ac43b-141">requiresUserAuthentication</span></span>|<span data-ttu-id="ac43b-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-142">Boolean</span></span>|<span data-ttu-id="ac43b-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ac43b-144">configurationEndpointUrl</span></span>|<span data-ttu-id="ac43b-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac43b-145">String</span></span>|<span data-ttu-id="ac43b-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="ac43b-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ac43b-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-148">Boolean</span></span>|<span data-ttu-id="ac43b-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="ac43b-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ac43b-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ac43b-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ac43b-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-152">Boolean</span></span>|<span data-ttu-id="ac43b-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ac43b-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="ac43b-154">isDefault</span></span>|<span data-ttu-id="ac43b-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-155">Boolean</span></span>|<span data-ttu-id="ac43b-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-157">supervisedModeEnabled</span></span>|<span data-ttu-id="ac43b-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-158">Boolean</span></span>|<span data-ttu-id="ac43b-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="ac43b-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ac43b-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ac43b-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="ac43b-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ac43b-162">supportDepartment</span></span>|<span data-ttu-id="ac43b-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac43b-163">String</span></span>|<span data-ttu-id="ac43b-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-165">passCodeDisabled</span></span>|<span data-ttu-id="ac43b-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-166">Boolean</span></span>|<span data-ttu-id="ac43b-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="ac43b-168">isMandatory</span></span>|<span data-ttu-id="ac43b-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-169">Boolean</span></span>|<span data-ttu-id="ac43b-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-171">locationDisabled</span></span>|<span data-ttu-id="ac43b-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-172">Boolean</span></span>|<span data-ttu-id="ac43b-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ac43b-174">supportPhoneNumber</span></span>|<span data-ttu-id="ac43b-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac43b-175">String</span></span>|<span data-ttu-id="ac43b-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-177">profileRemovalDisabled</span></span>|<span data-ttu-id="ac43b-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-178">Boolean</span></span>|<span data-ttu-id="ac43b-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ac43b-180">restoreBlocked</span></span>|<span data-ttu-id="ac43b-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-181">Boolean</span></span>|<span data-ttu-id="ac43b-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-183">appleIdDisabled</span></span>|<span data-ttu-id="ac43b-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-184">Boolean</span></span>|<span data-ttu-id="ac43b-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ac43b-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-187">Boolean</span></span>|<span data-ttu-id="ac43b-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-189">touchIdDisabled</span></span>|<span data-ttu-id="ac43b-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-190">Boolean</span></span>|<span data-ttu-id="ac43b-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-192">applePayDisabled</span></span>|<span data-ttu-id="ac43b-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-193">Boolean</span></span>|<span data-ttu-id="ac43b-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-195">zoomDisabled</span></span>|<span data-ttu-id="ac43b-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-196">Boolean</span></span>|<span data-ttu-id="ac43b-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-198">siriDisabled</span></span>|<span data-ttu-id="ac43b-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-199">Boolean</span></span>|<span data-ttu-id="ac43b-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-201">diagnosticsDisabled</span></span>|<span data-ttu-id="ac43b-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-202">Boolean</span></span>|<span data-ttu-id="ac43b-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="ac43b-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-205">Boolean</span></span>|<span data-ttu-id="ac43b-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-207">privacyPaneDisabled</span></span>|<span data-ttu-id="ac43b-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-208">Boolean</span></span>|<span data-ttu-id="ac43b-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="ac43b-210">deviceNameTemplate</span></span>|<span data-ttu-id="ac43b-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ac43b-211">String</span></span>|<span data-ttu-id="ac43b-212">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="ac43b-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="ac43b-213">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ac43b-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="ac43b-214">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-214">registrationDisabled</span></span>|<span data-ttu-id="ac43b-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-215">Boolean</span></span>|<span data-ttu-id="ac43b-216">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ac43b-216">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="ac43b-217">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-217">fileVaultDisabled</span></span>|<span data-ttu-id="ac43b-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-218">Boolean</span></span>|<span data-ttu-id="ac43b-219">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ac43b-219">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="ac43b-220">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-220">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="ac43b-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-221">Boolean</span></span>|<span data-ttu-id="ac43b-222">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ac43b-222">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="ac43b-223">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-223">iCloudStorageDisabled</span></span>|<span data-ttu-id="ac43b-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-224">Boolean</span></span>|<span data-ttu-id="ac43b-225">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ac43b-225">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="ac43b-226">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ac43b-226">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="ac43b-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="ac43b-227">Boolean</span></span>|<span data-ttu-id="ac43b-228">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ac43b-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="ac43b-229">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac43b-229">Response</span></span>
<span data-ttu-id="ac43b-230">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ac43b-230">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ac43b-231">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ac43b-231">Example</span></span>

### <a name="request"></a><span data-ttu-id="ac43b-232">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ac43b-232">Request</span></span>
<span data-ttu-id="ac43b-233">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ac43b-233">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1191

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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="ac43b-234">Resposta</span><span class="sxs-lookup"><span data-stu-id="ac43b-234">Response</span></span>
<span data-ttu-id="ac43b-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ac43b-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1240

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
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




