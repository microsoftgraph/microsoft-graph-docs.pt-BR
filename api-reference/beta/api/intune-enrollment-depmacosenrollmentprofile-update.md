---
title: Atualizar depMacOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depMacOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 20a10d8357f4d59281c041ea101813a0bd380682
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37185368"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="62bba-103">Atualizar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="62bba-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="62bba-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62bba-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62bba-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62bba-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62bba-106">Atualiza as propriedades de um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="62bba-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62bba-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="62bba-107">Prerequisites</span></span>
<span data-ttu-id="62bba-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="62bba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62bba-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="62bba-110">Permission type</span></span>|<span data-ttu-id="62bba-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="62bba-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62bba-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="62bba-112">Delegated (work or school account)</span></span>|<span data-ttu-id="62bba-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62bba-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="62bba-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="62bba-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62bba-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="62bba-115">Not supported.</span></span>|
|<span data-ttu-id="62bba-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="62bba-116">Application</span></span>|<span data-ttu-id="62bba-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62bba-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62bba-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="62bba-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="62bba-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="62bba-119">Request headers</span></span>
|<span data-ttu-id="62bba-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="62bba-120">Header</span></span>|<span data-ttu-id="62bba-121">Valor</span><span class="sxs-lookup"><span data-stu-id="62bba-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62bba-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="62bba-122">Authorization</span></span>|<span data-ttu-id="62bba-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="62bba-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62bba-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="62bba-124">Accept</span></span>|<span data-ttu-id="62bba-125">application/json</span><span class="sxs-lookup"><span data-stu-id="62bba-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62bba-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="62bba-126">Request body</span></span>
<span data-ttu-id="62bba-127">No corpo da solicitação, forneça uma representação JSON do objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="62bba-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="62bba-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="62bba-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="62bba-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62bba-129">Property</span></span>|<span data-ttu-id="62bba-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="62bba-130">Type</span></span>|<span data-ttu-id="62bba-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="62bba-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62bba-132">id</span><span class="sxs-lookup"><span data-stu-id="62bba-132">id</span></span>|<span data-ttu-id="62bba-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62bba-133">String</span></span>|<span data-ttu-id="62bba-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-135">displayName</span><span class="sxs-lookup"><span data-stu-id="62bba-135">displayName</span></span>|<span data-ttu-id="62bba-136">String</span><span class="sxs-lookup"><span data-stu-id="62bba-136">String</span></span>|<span data-ttu-id="62bba-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-138">descrição</span><span class="sxs-lookup"><span data-stu-id="62bba-138">description</span></span>|<span data-ttu-id="62bba-139">String</span><span class="sxs-lookup"><span data-stu-id="62bba-139">String</span></span>|<span data-ttu-id="62bba-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="62bba-141">requiresUserAuthentication</span></span>|<span data-ttu-id="62bba-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-142">Boolean</span></span>|<span data-ttu-id="62bba-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="62bba-144">configurationEndpointUrl</span></span>|<span data-ttu-id="62bba-145">String</span><span class="sxs-lookup"><span data-stu-id="62bba-145">String</span></span>|<span data-ttu-id="62bba-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="62bba-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="62bba-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-148">Boolean</span></span>|<span data-ttu-id="62bba-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="62bba-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="62bba-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="62bba-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="62bba-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-152">Boolean</span></span>|<span data-ttu-id="62bba-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="62bba-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="62bba-154">isDefault</span></span>|<span data-ttu-id="62bba-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-155">Boolean</span></span>|<span data-ttu-id="62bba-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="62bba-157">supervisedModeEnabled</span></span>|<span data-ttu-id="62bba-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-158">Boolean</span></span>|<span data-ttu-id="62bba-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="62bba-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="62bba-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="62bba-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="62bba-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="62bba-162">supportDepartment</span></span>|<span data-ttu-id="62bba-163">String</span><span class="sxs-lookup"><span data-stu-id="62bba-163">String</span></span>|<span data-ttu-id="62bba-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-165">passCodeDisabled</span></span>|<span data-ttu-id="62bba-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-166">Boolean</span></span>|<span data-ttu-id="62bba-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="62bba-168">isMandatory</span></span>|<span data-ttu-id="62bba-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-169">Boolean</span></span>|<span data-ttu-id="62bba-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-171">locationDisabled</span></span>|<span data-ttu-id="62bba-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-172">Boolean</span></span>|<span data-ttu-id="62bba-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="62bba-174">supportPhoneNumber</span></span>|<span data-ttu-id="62bba-175">String</span><span class="sxs-lookup"><span data-stu-id="62bba-175">String</span></span>|<span data-ttu-id="62bba-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-177">profileRemovalDisabled</span></span>|<span data-ttu-id="62bba-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-178">Boolean</span></span>|<span data-ttu-id="62bba-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="62bba-180">restoreBlocked</span></span>|<span data-ttu-id="62bba-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-181">Boolean</span></span>|<span data-ttu-id="62bba-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-183">appleIdDisabled</span></span>|<span data-ttu-id="62bba-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-184">Boolean</span></span>|<span data-ttu-id="62bba-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="62bba-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-187">Boolean</span></span>|<span data-ttu-id="62bba-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-189">touchIdDisabled</span></span>|<span data-ttu-id="62bba-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-190">Boolean</span></span>|<span data-ttu-id="62bba-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-192">applePayDisabled</span></span>|<span data-ttu-id="62bba-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-193">Boolean</span></span>|<span data-ttu-id="62bba-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-195">zoomDisabled</span></span>|<span data-ttu-id="62bba-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-196">Boolean</span></span>|<span data-ttu-id="62bba-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-198">siriDisabled</span></span>|<span data-ttu-id="62bba-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-199">Boolean</span></span>|<span data-ttu-id="62bba-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-201">diagnosticsDisabled</span></span>|<span data-ttu-id="62bba-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-202">Boolean</span></span>|<span data-ttu-id="62bba-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="62bba-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-205">Boolean</span></span>|<span data-ttu-id="62bba-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-207">privacyPaneDisabled</span></span>|<span data-ttu-id="62bba-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-208">Boolean</span></span>|<span data-ttu-id="62bba-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-210">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="62bba-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-211">Boolean</span></span>|<span data-ttu-id="62bba-212">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-213">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="62bba-213">deviceNameTemplate</span></span>|<span data-ttu-id="62bba-214">String</span><span class="sxs-lookup"><span data-stu-id="62bba-214">String</span></span>|<span data-ttu-id="62bba-215">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="62bba-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="62bba-216">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="62bba-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="62bba-217">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-217">registrationDisabled</span></span>|<span data-ttu-id="62bba-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-218">Boolean</span></span>|<span data-ttu-id="62bba-219">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="62bba-219">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="62bba-220">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-220">fileVaultDisabled</span></span>|<span data-ttu-id="62bba-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-221">Boolean</span></span>|<span data-ttu-id="62bba-222">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="62bba-222">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="62bba-223">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-223">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="62bba-224">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-224">Boolean</span></span>|<span data-ttu-id="62bba-225">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="62bba-225">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="62bba-226">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-226">iCloudStorageDisabled</span></span>|<span data-ttu-id="62bba-227">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-227">Boolean</span></span>|<span data-ttu-id="62bba-228">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="62bba-228">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="62bba-229">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="62bba-229">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="62bba-230">Booliano</span><span class="sxs-lookup"><span data-stu-id="62bba-230">Boolean</span></span>|<span data-ttu-id="62bba-231">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="62bba-231">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="62bba-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="62bba-232">Response</span></span>
<span data-ttu-id="62bba-233">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="62bba-233">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62bba-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="62bba-234">Example</span></span>

### <a name="request"></a><span data-ttu-id="62bba-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="62bba-235">Request</span></span>
<span data-ttu-id="62bba-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="62bba-236">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1228

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="62bba-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="62bba-237">Response</span></span>
<span data-ttu-id="62bba-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="62bba-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1277

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




