---
title: Criar depMacOSEnrollmentProfile
description: Criar um novo objeto depMacOSEnrollmentProfile.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37a4e58641415b6f6d8a759439d084d96ae9c665
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42813331"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="f0d26-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f0d26-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="f0d26-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f0d26-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0d26-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f0d26-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0d26-106">Criar um novo objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f0d26-106">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f0d26-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f0d26-107">Prerequisites</span></span>
<span data-ttu-id="f0d26-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f0d26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f0d26-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f0d26-110">Permission type</span></span>|<span data-ttu-id="f0d26-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f0d26-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f0d26-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f0d26-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f0d26-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0d26-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f0d26-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f0d26-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f0d26-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f0d26-115">Not supported.</span></span>|
|<span data-ttu-id="f0d26-116">Application</span><span class="sxs-lookup"><span data-stu-id="f0d26-116">Application</span></span>|<span data-ttu-id="f0d26-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f0d26-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f0d26-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f0d26-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f0d26-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f0d26-119">Request headers</span></span>
|<span data-ttu-id="f0d26-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f0d26-120">Header</span></span>|<span data-ttu-id="f0d26-121">Valor</span><span class="sxs-lookup"><span data-stu-id="f0d26-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f0d26-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="f0d26-122">Authorization</span></span>|<span data-ttu-id="f0d26-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f0d26-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f0d26-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f0d26-124">Accept</span></span>|<span data-ttu-id="f0d26-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f0d26-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f0d26-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f0d26-126">Request body</span></span>
<span data-ttu-id="f0d26-127">No corpo da solicitação, forneça uma representação JSON do objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="f0d26-127">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="f0d26-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="f0d26-128">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="f0d26-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f0d26-129">Property</span></span>|<span data-ttu-id="f0d26-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="f0d26-130">Type</span></span>|<span data-ttu-id="f0d26-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="f0d26-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0d26-132">id</span><span class="sxs-lookup"><span data-stu-id="f0d26-132">id</span></span>|<span data-ttu-id="f0d26-133">String</span><span class="sxs-lookup"><span data-stu-id="f0d26-133">String</span></span>|<span data-ttu-id="f0d26-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-135">displayName</span><span class="sxs-lookup"><span data-stu-id="f0d26-135">displayName</span></span>|<span data-ttu-id="f0d26-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f0d26-136">String</span></span>|<span data-ttu-id="f0d26-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-138">description</span><span class="sxs-lookup"><span data-stu-id="f0d26-138">description</span></span>|<span data-ttu-id="f0d26-139">String</span><span class="sxs-lookup"><span data-stu-id="f0d26-139">String</span></span>|<span data-ttu-id="f0d26-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f0d26-141">requiresUserAuthentication</span></span>|<span data-ttu-id="f0d26-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-142">Boolean</span></span>|<span data-ttu-id="f0d26-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f0d26-144">configurationEndpointUrl</span></span>|<span data-ttu-id="f0d26-145">String</span><span class="sxs-lookup"><span data-stu-id="f0d26-145">String</span></span>|<span data-ttu-id="f0d26-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="f0d26-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f0d26-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-148">Boolean</span></span>|<span data-ttu-id="f0d26-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="f0d26-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f0d26-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f0d26-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f0d26-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-152">Boolean</span></span>|<span data-ttu-id="f0d26-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f0d26-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="f0d26-154">isDefault</span></span>|<span data-ttu-id="f0d26-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="f0d26-155">Boolean</span></span>|<span data-ttu-id="f0d26-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-157">supervisedModeEnabled</span></span>|<span data-ttu-id="f0d26-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-158">Boolean</span></span>|<span data-ttu-id="f0d26-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="f0d26-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f0d26-160">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f0d26-160">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="f0d26-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f0d26-162">supportDepartment</span></span>|<span data-ttu-id="f0d26-163">String</span><span class="sxs-lookup"><span data-stu-id="f0d26-163">String</span></span>|<span data-ttu-id="f0d26-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-165">passCodeDisabled</span></span>|<span data-ttu-id="f0d26-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-166">Boolean</span></span>|<span data-ttu-id="f0d26-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="f0d26-168">isMandatory</span></span>|<span data-ttu-id="f0d26-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-169">Boolean</span></span>|<span data-ttu-id="f0d26-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-171">locationDisabled</span></span>|<span data-ttu-id="f0d26-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-172">Boolean</span></span>|<span data-ttu-id="f0d26-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f0d26-174">supportPhoneNumber</span></span>|<span data-ttu-id="f0d26-175">String</span><span class="sxs-lookup"><span data-stu-id="f0d26-175">String</span></span>|<span data-ttu-id="f0d26-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-177">profileRemovalDisabled</span></span>|<span data-ttu-id="f0d26-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-178">Boolean</span></span>|<span data-ttu-id="f0d26-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f0d26-180">restoreBlocked</span></span>|<span data-ttu-id="f0d26-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-181">Boolean</span></span>|<span data-ttu-id="f0d26-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-183">appleIdDisabled</span></span>|<span data-ttu-id="f0d26-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-184">Boolean</span></span>|<span data-ttu-id="f0d26-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f0d26-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-187">Boolean</span></span>|<span data-ttu-id="f0d26-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-189">touchIdDisabled</span></span>|<span data-ttu-id="f0d26-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-190">Boolean</span></span>|<span data-ttu-id="f0d26-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-192">applePayDisabled</span></span>|<span data-ttu-id="f0d26-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-193">Boolean</span></span>|<span data-ttu-id="f0d26-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-195">zoomDisabled</span></span>|<span data-ttu-id="f0d26-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-196">Boolean</span></span>|<span data-ttu-id="f0d26-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-198">siriDisabled</span></span>|<span data-ttu-id="f0d26-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-199">Boolean</span></span>|<span data-ttu-id="f0d26-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-201">diagnosticsDisabled</span></span>|<span data-ttu-id="f0d26-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-202">Boolean</span></span>|<span data-ttu-id="f0d26-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="f0d26-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-205">Boolean</span></span>|<span data-ttu-id="f0d26-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-207">privacyPaneDisabled</span></span>|<span data-ttu-id="f0d26-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-208">Boolean</span></span>|<span data-ttu-id="f0d26-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-210">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="f0d26-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-211">Boolean</span></span>|<span data-ttu-id="f0d26-212">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-213">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="f0d26-213">deviceNameTemplate</span></span>|<span data-ttu-id="f0d26-214">String</span><span class="sxs-lookup"><span data-stu-id="f0d26-214">String</span></span>|<span data-ttu-id="f0d26-215">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="f0d26-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="f0d26-216">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-217">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="f0d26-217">configurationWebUrl</span></span>|<span data-ttu-id="f0d26-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-218">Boolean</span></span>|<span data-ttu-id="f0d26-219">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f0d26-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f0d26-220">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-220">registrationDisabled</span></span>|<span data-ttu-id="f0d26-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-221">Boolean</span></span>|<span data-ttu-id="f0d26-222">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f0d26-222">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="f0d26-223">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-223">fileVaultDisabled</span></span>|<span data-ttu-id="f0d26-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-224">Boolean</span></span>|<span data-ttu-id="f0d26-225">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f0d26-225">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="f0d26-226">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-226">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="f0d26-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-227">Boolean</span></span>|<span data-ttu-id="f0d26-228">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f0d26-228">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="f0d26-229">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-229">iCloudStorageDisabled</span></span>|<span data-ttu-id="f0d26-230">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-230">Boolean</span></span>|<span data-ttu-id="f0d26-231">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f0d26-231">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="f0d26-232">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="f0d26-232">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="f0d26-233">Boolean</span><span class="sxs-lookup"><span data-stu-id="f0d26-233">Boolean</span></span>|<span data-ttu-id="f0d26-234">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f0d26-234">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="f0d26-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0d26-235">Response</span></span>
<span data-ttu-id="f0d26-236">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f0d26-236">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f0d26-237">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f0d26-237">Example</span></span>

### <a name="request"></a><span data-ttu-id="f0d26-238">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f0d26-238">Request</span></span>
<span data-ttu-id="f0d26-239">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f0d26-239">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f0d26-240">Resposta</span><span class="sxs-lookup"><span data-stu-id="f0d26-240">Response</span></span>
<span data-ttu-id="f0d26-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f0d26-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




