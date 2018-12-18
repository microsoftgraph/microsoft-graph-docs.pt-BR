---
title: Criar depMacOSEnrollmentProfile
description: Crie um novo objeto de depMacOSEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: 9b9d05045139dc83477760923fcc8924e1f83b1e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338511"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="20f0c-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="20f0c-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="20f0c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="20f0c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20f0c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="20f0c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="20f0c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="20f0c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="20f0c-107">Crie um novo objeto de [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="20f0c-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="20f0c-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="20f0c-108">Prerequisites</span></span>
<span data-ttu-id="20f0c-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="20f0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20f0c-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="20f0c-111">Permission type</span></span>|<span data-ttu-id="20f0c-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="20f0c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20f0c-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="20f0c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="20f0c-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20f0c-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="20f0c-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="20f0c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20f0c-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20f0c-116">Not supported.</span></span>|
|<span data-ttu-id="20f0c-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="20f0c-117">Application</span></span>|<span data-ttu-id="20f0c-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="20f0c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20f0c-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="20f0c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="20f0c-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="20f0c-120">Request headers</span></span>
|<span data-ttu-id="20f0c-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="20f0c-121">Header</span></span>|<span data-ttu-id="20f0c-122">Valor</span><span class="sxs-lookup"><span data-stu-id="20f0c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20f0c-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="20f0c-123">Authorization</span></span>|<span data-ttu-id="20f0c-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="20f0c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20f0c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="20f0c-125">Accept</span></span>|<span data-ttu-id="20f0c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="20f0c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20f0c-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="20f0c-127">Request body</span></span>
<span data-ttu-id="20f0c-128">No corpo da solicitação, fornece uma representação JSON para o objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="20f0c-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="20f0c-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="20f0c-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="20f0c-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20f0c-130">Property</span></span>|<span data-ttu-id="20f0c-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="20f0c-131">Type</span></span>|<span data-ttu-id="20f0c-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="20f0c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20f0c-133">id</span><span class="sxs-lookup"><span data-stu-id="20f0c-133">id</span></span>|<span data-ttu-id="20f0c-134">String</span><span class="sxs-lookup"><span data-stu-id="20f0c-134">String</span></span>|<span data-ttu-id="20f0c-135">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="20f0c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="20f0c-136">displayName</span></span>|<span data-ttu-id="20f0c-137">String</span><span class="sxs-lookup"><span data-stu-id="20f0c-137">String</span></span>|<span data-ttu-id="20f0c-138">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="20f0c-139">description</span><span class="sxs-lookup"><span data-stu-id="20f0c-139">description</span></span>|<span data-ttu-id="20f0c-140">String</span><span class="sxs-lookup"><span data-stu-id="20f0c-140">String</span></span>|<span data-ttu-id="20f0c-141">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="20f0c-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="20f0c-142">requiresUserAuthentication</span></span>|<span data-ttu-id="20f0c-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-143">Boolean</span></span>|<span data-ttu-id="20f0c-144">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="20f0c-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="20f0c-145">configurationEndpointUrl</span></span>|<span data-ttu-id="20f0c-146">String</span><span class="sxs-lookup"><span data-stu-id="20f0c-146">String</span></span>|<span data-ttu-id="20f0c-147">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="20f0c-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="20f0c-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="20f0c-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-149">Boolean</span></span>|<span data-ttu-id="20f0c-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="20f0c-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="20f0c-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="20f0c-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="20f0c-152">isDefault</span></span>|<span data-ttu-id="20f0c-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-153">Boolean</span></span>|<span data-ttu-id="20f0c-154">Indica se esse é o perfil padrão Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-155">supervisedModeEnabled</span></span>|<span data-ttu-id="20f0c-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-156">Boolean</span></span>|<span data-ttu-id="20f0c-157">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="20f0c-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="20f0c-158">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="20f0c-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="20f0c-159">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="20f0c-160">supportDepartment</span></span>|<span data-ttu-id="20f0c-161">String</span><span class="sxs-lookup"><span data-stu-id="20f0c-161">String</span></span>|<span data-ttu-id="20f0c-162">Informações de departamento de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-163">passCodeDisabled</span></span>|<span data-ttu-id="20f0c-164">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-164">Boolean</span></span>|<span data-ttu-id="20f0c-165">Indica se a senha instalação painel está desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="20f0c-166">isMandatory</span></span>|<span data-ttu-id="20f0c-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-167">Boolean</span></span>|<span data-ttu-id="20f0c-168">Indica se o perfil é obrigatória herdar de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-169">locationDisabled</span></span>|<span data-ttu-id="20f0c-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-170">Boolean</span></span>|<span data-ttu-id="20f0c-171">Indica se o local do painel de configuração do serviço é desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="20f0c-172">supportPhoneNumber</span></span>|<span data-ttu-id="20f0c-173">String</span><span class="sxs-lookup"><span data-stu-id="20f0c-173">String</span></span>|<span data-ttu-id="20f0c-174">Número de telefone de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-175">profileRemovalDisabled</span></span>|<span data-ttu-id="20f0c-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-176">Boolean</span></span>|<span data-ttu-id="20f0c-177">Indica se a opção de remoção de perfil será desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="20f0c-178">restoreBlocked</span></span>|<span data-ttu-id="20f0c-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-179">Boolean</span></span>|<span data-ttu-id="20f0c-180">Indica se o painel de configuração de restauração será bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-181">appleIdDisabled</span></span>|<span data-ttu-id="20f0c-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-182">Boolean</span></span>|<span data-ttu-id="20f0c-183">Indica se o Apple painel de configuração de id estará desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="20f0c-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-185">Boolean</span></span>|<span data-ttu-id="20f0c-186">Indica se o painel de configuração de 'Termos e condições' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-187">touchIdDisabled</span></span>|<span data-ttu-id="20f0c-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-188">Boolean</span></span>|<span data-ttu-id="20f0c-189">Indica se o painel de configuração de id de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-190">applePayDisabled</span></span>|<span data-ttu-id="20f0c-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-191">Boolean</span></span>|<span data-ttu-id="20f0c-192">Indica se o painel de configuração de pagamento do Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-193">zoomDisabled</span></span>|<span data-ttu-id="20f0c-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-194">Boolean</span></span>|<span data-ttu-id="20f0c-195">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-196">siriDisabled</span></span>|<span data-ttu-id="20f0c-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-197">Boolean</span></span>|<span data-ttu-id="20f0c-198">Indica se o painel de configuração de siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-199">diagnosticsDisabled</span></span>|<span data-ttu-id="20f0c-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-200">Boolean</span></span>|<span data-ttu-id="20f0c-201">Indica se o diagnóstico do painel de instalação está desabilitada Inherited em [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="20f0c-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="20f0c-202">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-202">registrationDisabled</span></span>|<span data-ttu-id="20f0c-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-203">Boolean</span></span>|<span data-ttu-id="20f0c-204">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="20f0c-204">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="20f0c-205">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-205">fileVaultDisabled</span></span>|<span data-ttu-id="20f0c-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-206">Boolean</span></span>|<span data-ttu-id="20f0c-207">Indica se o armazenamento de arquivo está desabilitado</span><span class="sxs-lookup"><span data-stu-id="20f0c-207">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="20f0c-208">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="20f0c-208">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="20f0c-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="20f0c-209">Boolean</span></span>|<span data-ttu-id="20f0c-210">Indica se a tela de análise de iCloud está desabilitada</span><span class="sxs-lookup"><span data-stu-id="20f0c-210">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="20f0c-211">Resposta</span><span class="sxs-lookup"><span data-stu-id="20f0c-211">Response</span></span>
<span data-ttu-id="20f0c-212">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="20f0c-212">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20f0c-213">Exemplo</span><span class="sxs-lookup"><span data-stu-id="20f0c-213">Example</span></span>
### <a name="request"></a><span data-ttu-id="20f0c-214">Solicitação</span><span class="sxs-lookup"><span data-stu-id="20f0c-214">Request</span></span>
<span data-ttu-id="20f0c-215">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="20f0c-215">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 928

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="20f0c-216">Resposta</span><span class="sxs-lookup"><span data-stu-id="20f0c-216">Response</span></span>
<span data-ttu-id="20f0c-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="20f0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 977

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
  "displayName": "Display Name value",
  "description": "Description value",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "https://example.com/configurationEndpointUrl/",
  "enableAuthenticationViaCompanyPortal": true,
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true
}
```





