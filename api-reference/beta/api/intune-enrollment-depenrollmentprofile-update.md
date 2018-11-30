---
title: Atualizar depEnrollmentProfile
description: Atualize as propriedades de um objeto depEnrollmentProfile.
ms.openlocfilehash: 1026abe11bec1a766b7fda2907612d77af077bd9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27038554"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="0ca94-103">Atualizar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="0ca94-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="0ca94-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0ca94-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0ca94-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0ca94-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0ca94-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0ca94-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0ca94-107">Atualize as propriedades de um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0ca94-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0ca94-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="0ca94-108">Prerequisites</span></span>
<span data-ttu-id="0ca94-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0ca94-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ca94-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0ca94-111">Permission type</span></span>|<span data-ttu-id="0ca94-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="0ca94-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0ca94-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0ca94-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0ca94-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ca94-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0ca94-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0ca94-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0ca94-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ca94-116">Not supported.</span></span>|
|<span data-ttu-id="0ca94-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0ca94-117">Application</span></span>|<span data-ttu-id="0ca94-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0ca94-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0ca94-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0ca94-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0ca94-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0ca94-120">Request headers</span></span>
|<span data-ttu-id="0ca94-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0ca94-121">Header</span></span>|<span data-ttu-id="0ca94-122">Valor</span><span class="sxs-lookup"><span data-stu-id="0ca94-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0ca94-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="0ca94-123">Authorization</span></span>|<span data-ttu-id="0ca94-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0ca94-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0ca94-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0ca94-125">Accept</span></span>|<span data-ttu-id="0ca94-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0ca94-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ca94-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0ca94-127">Request body</span></span>
<span data-ttu-id="0ca94-128">No corpo da solicitação, fornece uma representação JSON para o objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="0ca94-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="0ca94-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="0ca94-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="0ca94-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0ca94-130">Property</span></span>|<span data-ttu-id="0ca94-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="0ca94-131">Type</span></span>|<span data-ttu-id="0ca94-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="0ca94-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0ca94-133">id</span><span class="sxs-lookup"><span data-stu-id="0ca94-133">id</span></span>|<span data-ttu-id="0ca94-134">String</span><span class="sxs-lookup"><span data-stu-id="0ca94-134">String</span></span>|<span data-ttu-id="0ca94-135">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0ca94-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0ca94-136">displayName</span></span>|<span data-ttu-id="0ca94-137">String</span><span class="sxs-lookup"><span data-stu-id="0ca94-137">String</span></span>|<span data-ttu-id="0ca94-138">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0ca94-139">description</span><span class="sxs-lookup"><span data-stu-id="0ca94-139">description</span></span>|<span data-ttu-id="0ca94-140">String</span><span class="sxs-lookup"><span data-stu-id="0ca94-140">String</span></span>|<span data-ttu-id="0ca94-141">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0ca94-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="0ca94-142">requiresUserAuthentication</span></span>|<span data-ttu-id="0ca94-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-143">Boolean</span></span>|<span data-ttu-id="0ca94-144">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0ca94-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="0ca94-145">configurationEndpointUrl</span></span>|<span data-ttu-id="0ca94-146">String</span><span class="sxs-lookup"><span data-stu-id="0ca94-146">String</span></span>|<span data-ttu-id="0ca94-147">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0ca94-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="0ca94-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="0ca94-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-149">Boolean</span></span>|<span data-ttu-id="0ca94-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="0ca94-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="0ca94-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="0ca94-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="0ca94-152">isDefault</span></span>|<span data-ttu-id="0ca94-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-153">Boolean</span></span>|<span data-ttu-id="0ca94-154">Indica se esse é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="0ca94-154">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="0ca94-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-155">supervisedModeEnabled</span></span>|<span data-ttu-id="0ca94-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-156">Boolean</span></span>|<span data-ttu-id="0ca94-157">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="0ca94-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="0ca94-158">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="0ca94-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="0ca94-159">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="0ca94-159">supportDepartment</span></span>|<span data-ttu-id="0ca94-160">String</span><span class="sxs-lookup"><span data-stu-id="0ca94-160">String</span></span>|<span data-ttu-id="0ca94-161">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="0ca94-161">Support department information</span></span>|
|<span data-ttu-id="0ca94-162">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-162">passCodeDisabled</span></span>|<span data-ttu-id="0ca94-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-163">Boolean</span></span>|<span data-ttu-id="0ca94-164">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-164">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-165">isMandatory</span><span class="sxs-lookup"><span data-stu-id="0ca94-165">isMandatory</span></span>|<span data-ttu-id="0ca94-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-166">Boolean</span></span>|<span data-ttu-id="0ca94-167">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="0ca94-167">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="0ca94-168">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-168">locationDisabled</span></span>|<span data-ttu-id="0ca94-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-169">Boolean</span></span>|<span data-ttu-id="0ca94-170">Indica se o painel de configuração do serviço local está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-170">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-171">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="0ca94-171">supportPhoneNumber</span></span>|<span data-ttu-id="0ca94-172">String</span><span class="sxs-lookup"><span data-stu-id="0ca94-172">String</span></span>|<span data-ttu-id="0ca94-173">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="0ca94-173">Support phone number</span></span>|
|<span data-ttu-id="0ca94-174">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="0ca94-174">iTunesPairingMode</span></span>|[<span data-ttu-id="0ca94-175">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="0ca94-175">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="0ca94-176">Indica a modo de emparelhamento de iTunes.</span><span class="sxs-lookup"><span data-stu-id="0ca94-176">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="0ca94-177">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="0ca94-177">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="0ca94-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-178">profileRemovalDisabled</span></span>|<span data-ttu-id="0ca94-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-179">Boolean</span></span>|<span data-ttu-id="0ca94-180">Indica se a opção de remoção do perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="0ca94-180">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="0ca94-181">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="0ca94-181">managementCertificates</span></span>|<span data-ttu-id="0ca94-182">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="0ca94-182">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="0ca94-183">Certificados de gerenciamento para configurador da Apple</span><span class="sxs-lookup"><span data-stu-id="0ca94-183">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="0ca94-184">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="0ca94-184">restoreBlocked</span></span>|<span data-ttu-id="0ca94-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-185">Boolean</span></span>|<span data-ttu-id="0ca94-186">Indica se o painel de configuração de restauração será bloqueado</span><span class="sxs-lookup"><span data-stu-id="0ca94-186">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="0ca94-187">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-187">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="0ca94-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-188">Boolean</span></span>|<span data-ttu-id="0ca94-189">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="0ca94-189">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="0ca94-190">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-190">appleIdDisabled</span></span>|<span data-ttu-id="0ca94-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-191">Boolean</span></span>|<span data-ttu-id="0ca94-192">Indica se o painel de configuração de id do Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-192">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-193">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-193">termsAndConditionsDisabled</span></span>|<span data-ttu-id="0ca94-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-194">Boolean</span></span>|<span data-ttu-id="0ca94-195">Indica se o painel de configuração de 'Termos e condições' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-195">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-196">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-196">touchIdDisabled</span></span>|<span data-ttu-id="0ca94-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-197">Boolean</span></span>|<span data-ttu-id="0ca94-198">Indica se o painel de configuração de id de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-198">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-199">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-199">applePayDisabled</span></span>|<span data-ttu-id="0ca94-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-200">Boolean</span></span>|<span data-ttu-id="0ca94-201">Indica se o painel de configuração de pagamento do Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-201">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-202">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-202">zoomDisabled</span></span>|<span data-ttu-id="0ca94-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-203">Boolean</span></span>|<span data-ttu-id="0ca94-204">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-204">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-205">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-205">siriDisabled</span></span>|<span data-ttu-id="0ca94-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-206">Boolean</span></span>|<span data-ttu-id="0ca94-207">Indica se o painel de configuração de siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-207">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-208">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-208">diagnosticsDisabled</span></span>|<span data-ttu-id="0ca94-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-209">Boolean</span></span>|<span data-ttu-id="0ca94-210">Indica se o painel de configuração de diagnósticos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-210">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="0ca94-211">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-211">macOSRegistrationDisabled</span></span>|<span data-ttu-id="0ca94-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-212">Boolean</span></span>|<span data-ttu-id="0ca94-213">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-213">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="0ca94-214">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="0ca94-214">macOSFileVaultDisabled</span></span>|<span data-ttu-id="0ca94-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-215">Boolean</span></span>|<span data-ttu-id="0ca94-216">Indica se o armazenamento de arquivo do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="0ca94-216">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="0ca94-217">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="0ca94-217">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="0ca94-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-218">Boolean</span></span>|<span data-ttu-id="0ca94-219">Indica se o dispositivo será necessário aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="0ca94-219">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="0ca94-220">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="0ca94-220">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="0ca94-221">Int32</span><span class="sxs-lookup"><span data-stu-id="0ca94-221">Int32</span></span>|<span data-ttu-id="0ca94-222">Especifica o número máximo de usuários que podem utilizar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="0ca94-222">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="0ca94-223">Só é aplicável no modo compartilhado iPad.</span><span class="sxs-lookup"><span data-stu-id="0ca94-223">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="0ca94-224">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="0ca94-224">enableSharedIPad</span></span>|<span data-ttu-id="0ca94-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="0ca94-225">Boolean</span></span>|<span data-ttu-id="0ca94-226">Isso indica se o dispositivo é registrado em um modo que permite que vários cenários de usuário.</span><span class="sxs-lookup"><span data-stu-id="0ca94-226">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="0ca94-227">Só é aplicável no compartilhados iPads.</span><span class="sxs-lookup"><span data-stu-id="0ca94-227">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="0ca94-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ca94-228">Response</span></span>
<span data-ttu-id="0ca94-229">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0ca94-229">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ca94-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="0ca94-230">Example</span></span>
### <a name="request"></a><span data-ttu-id="0ca94-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0ca94-231">Request</span></span>
<span data-ttu-id="0ca94-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="0ca94-232">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1231

{
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
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```

### <a name="response"></a><span data-ttu-id="0ca94-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="0ca94-233">Response</span></span>
<span data-ttu-id="0ca94-p108">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0ca94-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1339

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
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
  "iTunesPairingMode": "allow",
  "profileRemovalDisabled": true,
  "managementCertificates": [
    {
      "@odata.type": "microsoft.graph.managementCertificateWithThumbprint",
      "thumbprint": "Thumbprint value",
      "certificate": "Certificate value"
    }
  ],
  "restoreBlocked": true,
  "restoreFromAndroidDisabled": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
  "zoomDisabled": true,
  "siriDisabled": true,
  "diagnosticsDisabled": true,
  "macOSRegistrationDisabled": true,
  "macOSFileVaultDisabled": true,
  "awaitDeviceConfiguredConfirmation": true,
  "sharedIPadMaximumUserCount": 10,
  "enableSharedIPad": true
}
```





