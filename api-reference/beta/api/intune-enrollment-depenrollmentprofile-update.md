---
title: Atualizar depEnrollmentProfile
description: Atualiza as propriedades de um objeto depEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e033d5f4601020e677e31a40b1d46c1e7652283
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30171446"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="43f31-103">Atualizar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="43f31-103">Update depEnrollmentProfile</span></span>

> <span data-ttu-id="43f31-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="43f31-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43f31-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="43f31-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43f31-106">Atualiza as propriedades de um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="43f31-106">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43f31-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="43f31-107">Prerequisites</span></span>
<span data-ttu-id="43f31-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="43f31-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="43f31-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="43f31-110">Permission type</span></span>|<span data-ttu-id="43f31-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="43f31-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43f31-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="43f31-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43f31-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43f31-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43f31-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="43f31-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43f31-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43f31-115">Not supported.</span></span>|
|<span data-ttu-id="43f31-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="43f31-116">Application</span></span>|<span data-ttu-id="43f31-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="43f31-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43f31-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="43f31-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="43f31-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="43f31-119">Request headers</span></span>
|<span data-ttu-id="43f31-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="43f31-120">Header</span></span>|<span data-ttu-id="43f31-121">Valor</span><span class="sxs-lookup"><span data-stu-id="43f31-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43f31-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="43f31-122">Authorization</span></span>|<span data-ttu-id="43f31-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="43f31-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43f31-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="43f31-124">Accept</span></span>|<span data-ttu-id="43f31-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43f31-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43f31-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="43f31-126">Request body</span></span>
<span data-ttu-id="43f31-127">No corpo da solicitação, forneça uma representação JSON do objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="43f31-127">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="43f31-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="43f31-128">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="43f31-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="43f31-129">Property</span></span>|<span data-ttu-id="43f31-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="43f31-130">Type</span></span>|<span data-ttu-id="43f31-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="43f31-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43f31-132">id</span><span class="sxs-lookup"><span data-stu-id="43f31-132">id</span></span>|<span data-ttu-id="43f31-133">String</span><span class="sxs-lookup"><span data-stu-id="43f31-133">String</span></span>|<span data-ttu-id="43f31-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-135">displayName</span><span class="sxs-lookup"><span data-stu-id="43f31-135">displayName</span></span>|<span data-ttu-id="43f31-136">String</span><span class="sxs-lookup"><span data-stu-id="43f31-136">String</span></span>|<span data-ttu-id="43f31-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-138">description</span><span class="sxs-lookup"><span data-stu-id="43f31-138">description</span></span>|<span data-ttu-id="43f31-139">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="43f31-139">String</span></span>|<span data-ttu-id="43f31-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="43f31-141">requiresUserAuthentication</span></span>|<span data-ttu-id="43f31-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-142">Boolean</span></span>|<span data-ttu-id="43f31-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="43f31-144">configurationEndpointUrl</span></span>|<span data-ttu-id="43f31-145">String</span><span class="sxs-lookup"><span data-stu-id="43f31-145">String</span></span>|<span data-ttu-id="43f31-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="43f31-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="43f31-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-148">Boolean</span></span>|<span data-ttu-id="43f31-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="43f31-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="43f31-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="43f31-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="43f31-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-152">Boolean</span></span>|<span data-ttu-id="43f31-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="43f31-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="43f31-154">isDefault</span></span>|<span data-ttu-id="43f31-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-155">Boolean</span></span>|<span data-ttu-id="43f31-156">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="43f31-156">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="43f31-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="43f31-157">supervisedModeEnabled</span></span>|<span data-ttu-id="43f31-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-158">Boolean</span></span>|<span data-ttu-id="43f31-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="43f31-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="43f31-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="43f31-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="43f31-161">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="43f31-161">supportDepartment</span></span>|<span data-ttu-id="43f31-162">String</span><span class="sxs-lookup"><span data-stu-id="43f31-162">String</span></span>|<span data-ttu-id="43f31-163">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="43f31-163">Support department information</span></span>|
|<span data-ttu-id="43f31-164">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-164">passCodeDisabled</span></span>|<span data-ttu-id="43f31-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-165">Boolean</span></span>|<span data-ttu-id="43f31-166">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-166">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-167">isMandatory</span><span class="sxs-lookup"><span data-stu-id="43f31-167">isMandatory</span></span>|<span data-ttu-id="43f31-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-168">Boolean</span></span>|<span data-ttu-id="43f31-169">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="43f31-169">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="43f31-170">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-170">locationDisabled</span></span>|<span data-ttu-id="43f31-171">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-171">Boolean</span></span>|<span data-ttu-id="43f31-172">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-172">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-173">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="43f31-173">supportPhoneNumber</span></span>|<span data-ttu-id="43f31-174">String</span><span class="sxs-lookup"><span data-stu-id="43f31-174">String</span></span>|<span data-ttu-id="43f31-175">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="43f31-175">Support phone number</span></span>|
|<span data-ttu-id="43f31-176">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="43f31-176">iTunesPairingMode</span></span>|[<span data-ttu-id="43f31-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="43f31-177">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="43f31-178">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="43f31-178">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="43f31-179">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="43f31-179">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="43f31-180">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-180">profileRemovalDisabled</span></span>|<span data-ttu-id="43f31-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-181">Boolean</span></span>|<span data-ttu-id="43f31-182">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="43f31-182">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="43f31-183">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="43f31-183">managementCertificates</span></span>|<span data-ttu-id="43f31-184">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="43f31-184">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="43f31-185">Certificados de gerenciamento para o Apple conFigurator</span><span class="sxs-lookup"><span data-stu-id="43f31-185">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="43f31-186">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="43f31-186">restoreBlocked</span></span>|<span data-ttu-id="43f31-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-187">Boolean</span></span>|<span data-ttu-id="43f31-188">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="43f31-188">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="43f31-189">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-189">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="43f31-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-190">Boolean</span></span>|<span data-ttu-id="43f31-191">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="43f31-191">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="43f31-192">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-192">appleIdDisabled</span></span>|<span data-ttu-id="43f31-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-193">Boolean</span></span>|<span data-ttu-id="43f31-194">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-194">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-195">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-195">termsAndConditionsDisabled</span></span>|<span data-ttu-id="43f31-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-196">Boolean</span></span>|<span data-ttu-id="43f31-197">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-197">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-198">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-198">touchIdDisabled</span></span>|<span data-ttu-id="43f31-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-199">Boolean</span></span>|<span data-ttu-id="43f31-200">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-200">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-201">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-201">applePayDisabled</span></span>|<span data-ttu-id="43f31-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-202">Boolean</span></span>|<span data-ttu-id="43f31-203">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-203">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-204">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-204">zoomDisabled</span></span>|<span data-ttu-id="43f31-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-205">Boolean</span></span>|<span data-ttu-id="43f31-206">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-206">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-207">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-207">siriDisabled</span></span>|<span data-ttu-id="43f31-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-208">Boolean</span></span>|<span data-ttu-id="43f31-209">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-209">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-210">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-210">diagnosticsDisabled</span></span>|<span data-ttu-id="43f31-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-211">Boolean</span></span>|<span data-ttu-id="43f31-212">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-212">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="43f31-213">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-213">macOSRegistrationDisabled</span></span>|<span data-ttu-id="43f31-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-214">Boolean</span></span>|<span data-ttu-id="43f31-215">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-215">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="43f31-216">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="43f31-216">macOSFileVaultDisabled</span></span>|<span data-ttu-id="43f31-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-217">Boolean</span></span>|<span data-ttu-id="43f31-218">Indica se o compartimento de arquivos do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="43f31-218">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="43f31-219">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="43f31-219">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="43f31-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-220">Boolean</span></span>|<span data-ttu-id="43f31-221">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="43f31-221">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="43f31-222">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="43f31-222">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="43f31-223">Int32</span><span class="sxs-lookup"><span data-stu-id="43f31-223">Int32</span></span>|<span data-ttu-id="43f31-224">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="43f31-224">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="43f31-225">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="43f31-225">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="43f31-226">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="43f31-226">enableSharedIPad</span></span>|<span data-ttu-id="43f31-227">Boolean</span><span class="sxs-lookup"><span data-stu-id="43f31-227">Boolean</span></span>|<span data-ttu-id="43f31-228">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="43f31-228">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="43f31-229">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="43f31-229">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="43f31-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f31-230">Response</span></span>
<span data-ttu-id="43f31-231">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="43f31-231">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43f31-232">Exemplo</span><span class="sxs-lookup"><span data-stu-id="43f31-232">Example</span></span>

### <a name="request"></a><span data-ttu-id="43f31-233">Solicitação</span><span class="sxs-lookup"><span data-stu-id="43f31-233">Request</span></span>
<span data-ttu-id="43f31-234">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="43f31-234">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="43f31-235">Resposta</span><span class="sxs-lookup"><span data-stu-id="43f31-235">Response</span></span>
<span data-ttu-id="43f31-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="43f31-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




