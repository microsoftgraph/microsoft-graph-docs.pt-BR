---
title: Criar depMacOSEnrollmentProfile
description: Criar um novo objeto depMacOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0cff1ebdf53e2b32bcebaee146e413c32316023c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467162"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="61c99-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="61c99-103">Create depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="61c99-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="61c99-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="61c99-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="61c99-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="61c99-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="61c99-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="61c99-107">Criar um novo objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="61c99-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="61c99-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="61c99-108">Prerequisites</span></span>
<span data-ttu-id="61c99-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="61c99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="61c99-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="61c99-111">Permission type</span></span>|<span data-ttu-id="61c99-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="61c99-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="61c99-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="61c99-113">Delegated (work or school account)</span></span>|<span data-ttu-id="61c99-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61c99-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="61c99-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="61c99-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="61c99-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="61c99-116">Not supported.</span></span>|
|<span data-ttu-id="61c99-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="61c99-117">Application</span></span>|<span data-ttu-id="61c99-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="61c99-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="61c99-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="61c99-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="61c99-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="61c99-120">Request headers</span></span>
|<span data-ttu-id="61c99-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="61c99-121">Header</span></span>|<span data-ttu-id="61c99-122">Valor</span><span class="sxs-lookup"><span data-stu-id="61c99-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="61c99-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="61c99-123">Authorization</span></span>|<span data-ttu-id="61c99-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="61c99-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="61c99-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="61c99-125">Accept</span></span>|<span data-ttu-id="61c99-126">application/json</span><span class="sxs-lookup"><span data-stu-id="61c99-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="61c99-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="61c99-127">Request body</span></span>
<span data-ttu-id="61c99-128">No corpo da solicitação, forneça uma representação JSON do objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="61c99-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="61c99-129">A tabela a seguir mostra as propriedades que são necessárias ao criar depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="61c99-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="61c99-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="61c99-130">Property</span></span>|<span data-ttu-id="61c99-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="61c99-131">Type</span></span>|<span data-ttu-id="61c99-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="61c99-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="61c99-133">id</span><span class="sxs-lookup"><span data-stu-id="61c99-133">id</span></span>|<span data-ttu-id="61c99-134">String</span><span class="sxs-lookup"><span data-stu-id="61c99-134">String</span></span>|<span data-ttu-id="61c99-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-136">displayName</span><span class="sxs-lookup"><span data-stu-id="61c99-136">displayName</span></span>|<span data-ttu-id="61c99-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="61c99-137">String</span></span>|<span data-ttu-id="61c99-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-139">description</span><span class="sxs-lookup"><span data-stu-id="61c99-139">description</span></span>|<span data-ttu-id="61c99-140">String</span><span class="sxs-lookup"><span data-stu-id="61c99-140">String</span></span>|<span data-ttu-id="61c99-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="61c99-142">requiresUserAuthentication</span></span>|<span data-ttu-id="61c99-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-143">Boolean</span></span>|<span data-ttu-id="61c99-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="61c99-145">configurationEndpointUrl</span></span>|<span data-ttu-id="61c99-146">String</span><span class="sxs-lookup"><span data-stu-id="61c99-146">String</span></span>|<span data-ttu-id="61c99-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="61c99-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="61c99-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-149">Boolean</span></span>|<span data-ttu-id="61c99-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="61c99-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="61c99-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="61c99-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="61c99-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-153">Boolean</span></span>|<span data-ttu-id="61c99-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="61c99-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="61c99-155">isDefault</span></span>|<span data-ttu-id="61c99-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="61c99-156">Boolean</span></span>|<span data-ttu-id="61c99-157">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="61c99-158">supervisedModeEnabled</span></span>|<span data-ttu-id="61c99-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-159">Boolean</span></span>|<span data-ttu-id="61c99-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="61c99-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="61c99-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="61c99-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="61c99-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="61c99-163">supportDepartment</span></span>|<span data-ttu-id="61c99-164">String</span><span class="sxs-lookup"><span data-stu-id="61c99-164">String</span></span>|<span data-ttu-id="61c99-165">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-166">passCodeDisabled</span></span>|<span data-ttu-id="61c99-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-167">Boolean</span></span>|<span data-ttu-id="61c99-168">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-169">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="61c99-169">isMandatory</span></span>|<span data-ttu-id="61c99-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-170">Boolean</span></span>|<span data-ttu-id="61c99-171">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-172">locationDisabled</span></span>|<span data-ttu-id="61c99-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-173">Boolean</span></span>|<span data-ttu-id="61c99-174">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="61c99-175">supportPhoneNumber</span></span>|<span data-ttu-id="61c99-176">String</span><span class="sxs-lookup"><span data-stu-id="61c99-176">String</span></span>|<span data-ttu-id="61c99-177">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-178">profileRemovalDisabled</span></span>|<span data-ttu-id="61c99-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-179">Boolean</span></span>|<span data-ttu-id="61c99-180">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="61c99-181">restoreBlocked</span></span>|<span data-ttu-id="61c99-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-182">Boolean</span></span>|<span data-ttu-id="61c99-183">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-184">appleIdDisabled</span></span>|<span data-ttu-id="61c99-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-185">Boolean</span></span>|<span data-ttu-id="61c99-186">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="61c99-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-188">Boolean</span></span>|<span data-ttu-id="61c99-189">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-190">touchIdDisabled</span></span>|<span data-ttu-id="61c99-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-191">Boolean</span></span>|<span data-ttu-id="61c99-192">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-193">applePayDisabled</span></span>|<span data-ttu-id="61c99-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-194">Boolean</span></span>|<span data-ttu-id="61c99-195">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-196">zoomDisabled</span></span>|<span data-ttu-id="61c99-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-197">Boolean</span></span>|<span data-ttu-id="61c99-198">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-199">siriDisabled</span></span>|<span data-ttu-id="61c99-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-200">Boolean</span></span>|<span data-ttu-id="61c99-201">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-202">diagnosticsDisabled</span></span>|<span data-ttu-id="61c99-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-203">Boolean</span></span>|<span data-ttu-id="61c99-204">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="61c99-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-206">Boolean</span></span>|<span data-ttu-id="61c99-207">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-208">privacyPaneDisabled</span></span>|<span data-ttu-id="61c99-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-209">Boolean</span></span>|<span data-ttu-id="61c99-210">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-211">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="61c99-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-212">Boolean</span></span>|<span data-ttu-id="61c99-213">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-214">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="61c99-214">deviceNameTemplate</span></span>|<span data-ttu-id="61c99-215">String</span><span class="sxs-lookup"><span data-stu-id="61c99-215">String</span></span>|<span data-ttu-id="61c99-216">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="61c99-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="61c99-217">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-218">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="61c99-218">configurationWebUrl</span></span>|<span data-ttu-id="61c99-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-219">Boolean</span></span>|<span data-ttu-id="61c99-220">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="61c99-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="61c99-221">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-221">registrationDisabled</span></span>|<span data-ttu-id="61c99-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-222">Boolean</span></span>|<span data-ttu-id="61c99-223">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="61c99-223">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="61c99-224">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-224">fileVaultDisabled</span></span>|<span data-ttu-id="61c99-225">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-225">Boolean</span></span>|<span data-ttu-id="61c99-226">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="61c99-226">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="61c99-227">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-227">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="61c99-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-228">Boolean</span></span>|<span data-ttu-id="61c99-229">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="61c99-229">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="61c99-230">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-230">iCloudStorageDisabled</span></span>|<span data-ttu-id="61c99-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-231">Boolean</span></span>|<span data-ttu-id="61c99-232">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="61c99-232">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="61c99-233">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="61c99-233">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="61c99-234">Boolean</span><span class="sxs-lookup"><span data-stu-id="61c99-234">Boolean</span></span>|<span data-ttu-id="61c99-235">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="61c99-235">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="61c99-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="61c99-236">Response</span></span>
<span data-ttu-id="61c99-237">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="61c99-237">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="61c99-238">Exemplo</span><span class="sxs-lookup"><span data-stu-id="61c99-238">Example</span></span>

### <a name="request"></a><span data-ttu-id="61c99-239">Solicitação</span><span class="sxs-lookup"><span data-stu-id="61c99-239">Request</span></span>
<span data-ttu-id="61c99-240">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="61c99-240">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1260

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
  "configurationWebUrl": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="61c99-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="61c99-241">Response</span></span>
<span data-ttu-id="61c99-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="61c99-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1309

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
  "configurationWebUrl": true,
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```





