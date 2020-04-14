---
title: Atualizar depEnrollmentProfile
description: Atualiza as propriedades de um objeto depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ca8d1387d2b96368a4891825d5ddaf3e03d012fd
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413858"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="40851-103">Atualizar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="40851-103">Update depEnrollmentProfile</span></span>

<span data-ttu-id="40851-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40851-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40851-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="40851-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40851-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="40851-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40851-107">Atualiza as propriedades de um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="40851-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40851-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="40851-108">Prerequisites</span></span>
<span data-ttu-id="40851-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="40851-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40851-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="40851-111">Permission type</span></span>|<span data-ttu-id="40851-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="40851-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40851-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="40851-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40851-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40851-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="40851-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="40851-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40851-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="40851-116">Not supported.</span></span>|
|<span data-ttu-id="40851-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="40851-117">Application</span></span>|<span data-ttu-id="40851-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40851-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40851-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="40851-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="40851-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="40851-120">Request headers</span></span>
|<span data-ttu-id="40851-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="40851-121">Header</span></span>|<span data-ttu-id="40851-122">Valor</span><span class="sxs-lookup"><span data-stu-id="40851-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40851-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="40851-123">Authorization</span></span>|<span data-ttu-id="40851-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="40851-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40851-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="40851-125">Accept</span></span>|<span data-ttu-id="40851-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40851-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40851-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="40851-127">Request body</span></span>
<span data-ttu-id="40851-128">No corpo da solicitação, forneça uma representação JSON do objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="40851-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="40851-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="40851-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="40851-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="40851-130">Property</span></span>|<span data-ttu-id="40851-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="40851-131">Type</span></span>|<span data-ttu-id="40851-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="40851-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40851-133">id</span><span class="sxs-lookup"><span data-stu-id="40851-133">id</span></span>|<span data-ttu-id="40851-134">String</span><span class="sxs-lookup"><span data-stu-id="40851-134">String</span></span>|<span data-ttu-id="40851-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-136">displayName</span><span class="sxs-lookup"><span data-stu-id="40851-136">displayName</span></span>|<span data-ttu-id="40851-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="40851-137">String</span></span>|<span data-ttu-id="40851-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-139">description</span><span class="sxs-lookup"><span data-stu-id="40851-139">description</span></span>|<span data-ttu-id="40851-140">String</span><span class="sxs-lookup"><span data-stu-id="40851-140">String</span></span>|<span data-ttu-id="40851-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="40851-142">requiresUserAuthentication</span></span>|<span data-ttu-id="40851-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-143">Boolean</span></span>|<span data-ttu-id="40851-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="40851-145">configurationEndpointUrl</span></span>|<span data-ttu-id="40851-146">String</span><span class="sxs-lookup"><span data-stu-id="40851-146">String</span></span>|<span data-ttu-id="40851-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="40851-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="40851-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-149">Boolean</span></span>|<span data-ttu-id="40851-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="40851-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="40851-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="40851-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="40851-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-153">Boolean</span></span>|<span data-ttu-id="40851-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="40851-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="40851-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="40851-155">isDefault</span></span>|<span data-ttu-id="40851-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="40851-156">Boolean</span></span>|<span data-ttu-id="40851-157">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="40851-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="40851-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="40851-158">supervisedModeEnabled</span></span>|<span data-ttu-id="40851-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-159">Boolean</span></span>|<span data-ttu-id="40851-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="40851-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="40851-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="40851-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="40851-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="40851-162">supportDepartment</span></span>|<span data-ttu-id="40851-163">String</span><span class="sxs-lookup"><span data-stu-id="40851-163">String</span></span>|<span data-ttu-id="40851-164">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="40851-164">Support department information</span></span>|
|<span data-ttu-id="40851-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-165">passCodeDisabled</span></span>|<span data-ttu-id="40851-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-166">Boolean</span></span>|<span data-ttu-id="40851-167">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="40851-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="40851-168">isMandatory</span></span>|<span data-ttu-id="40851-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-169">Boolean</span></span>|<span data-ttu-id="40851-170">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="40851-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="40851-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-171">locationDisabled</span></span>|<span data-ttu-id="40851-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-172">Boolean</span></span>|<span data-ttu-id="40851-173">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="40851-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="40851-174">supportPhoneNumber</span></span>|<span data-ttu-id="40851-175">String</span><span class="sxs-lookup"><span data-stu-id="40851-175">String</span></span>|<span data-ttu-id="40851-176">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="40851-176">Support phone number</span></span>|
|<span data-ttu-id="40851-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="40851-177">iTunesPairingMode</span></span>|[<span data-ttu-id="40851-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="40851-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="40851-179">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="40851-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="40851-180">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="40851-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="40851-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-181">profileRemovalDisabled</span></span>|<span data-ttu-id="40851-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-182">Boolean</span></span>|<span data-ttu-id="40851-183">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="40851-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="40851-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="40851-184">managementCertificates</span></span>|<span data-ttu-id="40851-185">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="40851-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="40851-186">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="40851-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="40851-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="40851-187">restoreBlocked</span></span>|<span data-ttu-id="40851-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-188">Boolean</span></span>|<span data-ttu-id="40851-189">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="40851-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="40851-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="40851-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-191">Boolean</span></span>|<span data-ttu-id="40851-192">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="40851-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="40851-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-193">appleIdDisabled</span></span>|<span data-ttu-id="40851-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-194">Boolean</span></span>|<span data-ttu-id="40851-195">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="40851-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="40851-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-197">Boolean</span></span>|<span data-ttu-id="40851-198">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="40851-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-199">touchIdDisabled</span></span>|<span data-ttu-id="40851-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-200">Boolean</span></span>|<span data-ttu-id="40851-201">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="40851-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-202">applePayDisabled</span></span>|<span data-ttu-id="40851-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-203">Boolean</span></span>|<span data-ttu-id="40851-204">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="40851-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-205">zoomDisabled</span></span>|<span data-ttu-id="40851-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-206">Boolean</span></span>|<span data-ttu-id="40851-207">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="40851-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-208">siriDisabled</span></span>|<span data-ttu-id="40851-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-209">Boolean</span></span>|<span data-ttu-id="40851-210">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="40851-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-211">diagnosticsDisabled</span></span>|<span data-ttu-id="40851-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-212">Boolean</span></span>|<span data-ttu-id="40851-213">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="40851-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="40851-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-215">Boolean</span></span>|<span data-ttu-id="40851-216">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="40851-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="40851-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="40851-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-218">Boolean</span></span>|<span data-ttu-id="40851-219">Indica se o compartimento de arquivos do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="40851-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="40851-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="40851-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="40851-221">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-221">Boolean</span></span>|<span data-ttu-id="40851-222">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="40851-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="40851-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="40851-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="40851-224">Int32</span><span class="sxs-lookup"><span data-stu-id="40851-224">Int32</span></span>|<span data-ttu-id="40851-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="40851-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="40851-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="40851-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="40851-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="40851-227">enableSharedIPad</span></span>|<span data-ttu-id="40851-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="40851-228">Boolean</span></span>|<span data-ttu-id="40851-229">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="40851-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="40851-230">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="40851-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="40851-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="40851-231">Response</span></span>
<span data-ttu-id="40851-232">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="40851-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40851-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="40851-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="40851-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="40851-234">Request</span></span>
<span data-ttu-id="40851-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="40851-235">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
Content-type: application/json
Content-length: 1354

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
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

### <a name="response"></a><span data-ttu-id="40851-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="40851-236">Response</span></span>
<span data-ttu-id="40851-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="40851-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1403

{
  "@odata.type": "#microsoft.graph.depEnrollmentProfile",
  "id": "3d4534f7-34f7-3d45-f734-453df734453d",
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



