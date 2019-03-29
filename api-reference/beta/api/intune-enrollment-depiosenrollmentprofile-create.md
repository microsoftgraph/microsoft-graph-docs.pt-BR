---
title: Criar depIOSEnrollmentProfile
description: Criar um novo objeto depIOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 446fccbcba1563f17e9de349386544e907b34140
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30963720"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="8b4ed-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8b4ed-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="8b4ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b4ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b4ed-106">Criar um novo objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8b4ed-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b4ed-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8b4ed-107">Prerequisites</span></span>
<span data-ttu-id="8b4ed-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8b4ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b4ed-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8b4ed-110">Permission type</span></span>|<span data-ttu-id="8b4ed-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b4ed-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b4ed-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b4ed-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8b4ed-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b4ed-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-115">Not supported.</span></span>|
|<span data-ttu-id="8b4ed-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="8b4ed-116">Application</span></span>|<span data-ttu-id="8b4ed-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b4ed-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8b4ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="8b4ed-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8b4ed-119">Request headers</span></span>
|<span data-ttu-id="8b4ed-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8b4ed-120">Header</span></span>|<span data-ttu-id="8b4ed-121">Valor</span><span class="sxs-lookup"><span data-stu-id="8b4ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b4ed-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="8b4ed-122">Authorization</span></span>|<span data-ttu-id="8b4ed-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b4ed-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8b4ed-124">Accept</span></span>|<span data-ttu-id="8b4ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b4ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b4ed-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8b4ed-126">Request body</span></span>
<span data-ttu-id="8b4ed-127">No corpo da solicitação, forneça uma representação JSON do objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="8b4ed-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="8b4ed-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8b4ed-129">Property</span></span>|<span data-ttu-id="8b4ed-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="8b4ed-130">Type</span></span>|<span data-ttu-id="8b4ed-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="8b4ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b4ed-132">id</span><span class="sxs-lookup"><span data-stu-id="8b4ed-132">id</span></span>|<span data-ttu-id="8b4ed-133">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-133">String</span></span>|<span data-ttu-id="8b4ed-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-135">displayName</span><span class="sxs-lookup"><span data-stu-id="8b4ed-135">displayName</span></span>|<span data-ttu-id="8b4ed-136">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-136">String</span></span>|<span data-ttu-id="8b4ed-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-138">descrição</span><span class="sxs-lookup"><span data-stu-id="8b4ed-138">description</span></span>|<span data-ttu-id="8b4ed-139">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-139">String</span></span>|<span data-ttu-id="8b4ed-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8b4ed-141">requiresUserAuthentication</span></span>|<span data-ttu-id="8b4ed-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-142">Boolean</span></span>|<span data-ttu-id="8b4ed-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="8b4ed-144">configurationEndpointUrl</span></span>|<span data-ttu-id="8b4ed-145">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-145">String</span></span>|<span data-ttu-id="8b4ed-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8b4ed-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-148">Boolean</span></span>|<span data-ttu-id="8b4ed-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="8b4ed-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="8b4ed-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="8b4ed-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-152">Boolean</span></span>|<span data-ttu-id="8b4ed-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="8b4ed-154">isDefault</span></span>|<span data-ttu-id="8b4ed-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="8b4ed-155">Boolean</span></span>|<span data-ttu-id="8b4ed-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-157">supervisedModeEnabled</span></span>|<span data-ttu-id="8b4ed-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-158">Boolean</span></span>|<span data-ttu-id="8b4ed-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="8b4ed-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="8b4ed-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="8b4ed-162">supportDepartment</span></span>|<span data-ttu-id="8b4ed-163">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-163">String</span></span>|<span data-ttu-id="8b4ed-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-165">passCodeDisabled</span></span>|<span data-ttu-id="8b4ed-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-166">Boolean</span></span>|<span data-ttu-id="8b4ed-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="8b4ed-168">isMandatory</span></span>|<span data-ttu-id="8b4ed-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-169">Boolean</span></span>|<span data-ttu-id="8b4ed-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-171">locationDisabled</span></span>|<span data-ttu-id="8b4ed-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-172">Boolean</span></span>|<span data-ttu-id="8b4ed-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8b4ed-174">supportPhoneNumber</span></span>|<span data-ttu-id="8b4ed-175">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-175">String</span></span>|<span data-ttu-id="8b4ed-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-177">profileRemovalDisabled</span></span>|<span data-ttu-id="8b4ed-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-178">Boolean</span></span>|<span data-ttu-id="8b4ed-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8b4ed-180">restoreBlocked</span></span>|<span data-ttu-id="8b4ed-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-181">Boolean</span></span>|<span data-ttu-id="8b4ed-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-183">appleIdDisabled</span></span>|<span data-ttu-id="8b4ed-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-184">Boolean</span></span>|<span data-ttu-id="8b4ed-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="8b4ed-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-187">Boolean</span></span>|<span data-ttu-id="8b4ed-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-189">touchIdDisabled</span></span>|<span data-ttu-id="8b4ed-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-190">Boolean</span></span>|<span data-ttu-id="8b4ed-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-192">applePayDisabled</span></span>|<span data-ttu-id="8b4ed-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-193">Boolean</span></span>|<span data-ttu-id="8b4ed-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-195">zoomDisabled</span></span>|<span data-ttu-id="8b4ed-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-196">Boolean</span></span>|<span data-ttu-id="8b4ed-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-198">siriDisabled</span></span>|<span data-ttu-id="8b4ed-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-199">Boolean</span></span>|<span data-ttu-id="8b4ed-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-201">diagnosticsDisabled</span></span>|<span data-ttu-id="8b4ed-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-202">Boolean</span></span>|<span data-ttu-id="8b4ed-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="8b4ed-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-205">Boolean</span></span>|<span data-ttu-id="8b4ed-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-207">privacyPaneDisabled</span></span>|<span data-ttu-id="8b4ed-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-208">Boolean</span></span>|<span data-ttu-id="8b4ed-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="8b4ed-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8b4ed-210">iTunesPairingMode</span></span>|[<span data-ttu-id="8b4ed-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8b4ed-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="8b4ed-212">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="8b4ed-213">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="8b4ed-214">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="8b4ed-214">managementCertificates</span></span>|<span data-ttu-id="8b4ed-215">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="8b4ed-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="8b4ed-216">Certificados de gerenciamento para o Apple conFigurator</span><span class="sxs-lookup"><span data-stu-id="8b4ed-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="8b4ed-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="8b4ed-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-218">Boolean</span></span>|<span data-ttu-id="8b4ed-219">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="8b4ed-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="8b4ed-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="8b4ed-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-221">Boolean</span></span>|<span data-ttu-id="8b4ed-222">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="8b4ed-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="8b4ed-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="8b4ed-224">Int32</span><span class="sxs-lookup"><span data-stu-id="8b4ed-224">Int32</span></span>|<span data-ttu-id="8b4ed-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="8b4ed-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="8b4ed-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="8b4ed-227">enableSharedIPad</span></span>|<span data-ttu-id="8b4ed-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-228">Boolean</span></span>|<span data-ttu-id="8b4ed-229">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="8b4ed-230">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="8b4ed-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="8b4ed-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="8b4ed-232">String</span><span class="sxs-lookup"><span data-stu-id="8b4ed-232">String</span></span>|<span data-ttu-id="8b4ed-233">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="8b4ed-234">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="8b4ed-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="8b4ed-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="8b4ed-236">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-236">Boolean</span></span>|<span data-ttu-id="8b4ed-237">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="8b4ed-238">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-238">Default is false.</span></span> <span data-ttu-id="8b4ed-239">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="8b4ed-240">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="8b4ed-241">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-241">Boolean</span></span>|<span data-ttu-id="8b4ed-242">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="8b4ed-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="8b4ed-244">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-244">Boolean</span></span>|<span data-ttu-id="8b4ed-245">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="8b4ed-246">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="8b4ed-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-247">Boolean</span></span>|<span data-ttu-id="8b4ed-248">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="8b4ed-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="8b4ed-250">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-250">Boolean</span></span>|<span data-ttu-id="8b4ed-251">Indica se a configuração de tempo limite da tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="8b4ed-252">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="8b4ed-253">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-253">Boolean</span></span>|<span data-ttu-id="8b4ed-254">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="8b4ed-255">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="8b4ed-256">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-256">Boolean</span></span>|<span data-ttu-id="8b4ed-257">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="8b4ed-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="8b4ed-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="8b4ed-259">Boolean</span><span class="sxs-lookup"><span data-stu-id="8b4ed-259">Boolean</span></span>|<span data-ttu-id="8b4ed-260">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8b4ed-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="8b4ed-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b4ed-261">Response</span></span>
<span data-ttu-id="8b4ed-262">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-262">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b4ed-263">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8b4ed-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b4ed-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8b4ed-264">Request</span></span>
<span data-ttu-id="8b4ed-265">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-265">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1736

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

### <a name="response"></a><span data-ttu-id="8b4ed-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="8b4ed-266">Response</span></span>
<span data-ttu-id="8b4ed-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8b4ed-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1785

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




