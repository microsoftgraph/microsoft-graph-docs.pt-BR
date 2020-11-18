---
title: Atualizar depEnrollmentProfile
description: Atualiza as propriedades de um objeto depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6183fed00b52144e5d24ed9ecfba064bdbbca3d2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201993"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="8a600-103">Atualizar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="8a600-103">Update depEnrollmentProfile</span></span>

<span data-ttu-id="8a600-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a600-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8a600-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8a600-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8a600-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8a600-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a600-107">Atualiza as propriedades de um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8a600-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8a600-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="8a600-108">Prerequisites</span></span>
<span data-ttu-id="8a600-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8a600-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8a600-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="8a600-111">Permission type</span></span>|<span data-ttu-id="8a600-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="8a600-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8a600-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="8a600-113">Delegated (work or school account)</span></span>|<span data-ttu-id="8a600-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a600-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8a600-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="8a600-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8a600-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="8a600-116">Not supported.</span></span>|
|<span data-ttu-id="8a600-117">Application</span><span class="sxs-lookup"><span data-stu-id="8a600-117">Application</span></span>|<span data-ttu-id="8a600-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8a600-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8a600-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="8a600-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8a600-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="8a600-120">Request headers</span></span>
|<span data-ttu-id="8a600-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="8a600-121">Header</span></span>|<span data-ttu-id="8a600-122">Valor</span><span class="sxs-lookup"><span data-stu-id="8a600-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8a600-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="8a600-123">Authorization</span></span>|<span data-ttu-id="8a600-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="8a600-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8a600-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="8a600-125">Accept</span></span>|<span data-ttu-id="8a600-126">application/json</span><span class="sxs-lookup"><span data-stu-id="8a600-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8a600-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="8a600-127">Request body</span></span>
<span data-ttu-id="8a600-128">No corpo da solicitação, forneça uma representação JSON do objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="8a600-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8a600-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="8a600-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="8a600-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a600-130">Property</span></span>|<span data-ttu-id="8a600-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a600-131">Type</span></span>|<span data-ttu-id="8a600-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a600-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a600-133">id</span><span class="sxs-lookup"><span data-stu-id="8a600-133">id</span></span>|<span data-ttu-id="8a600-134">String</span><span class="sxs-lookup"><span data-stu-id="8a600-134">String</span></span>|<span data-ttu-id="8a600-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8a600-136">displayName</span></span>|<span data-ttu-id="8a600-137">String</span><span class="sxs-lookup"><span data-stu-id="8a600-137">String</span></span>|<span data-ttu-id="8a600-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-139">description</span><span class="sxs-lookup"><span data-stu-id="8a600-139">description</span></span>|<span data-ttu-id="8a600-140">String</span><span class="sxs-lookup"><span data-stu-id="8a600-140">String</span></span>|<span data-ttu-id="8a600-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="8a600-142">requiresUserAuthentication</span></span>|<span data-ttu-id="8a600-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-143">Boolean</span></span>|<span data-ttu-id="8a600-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="8a600-145">configurationEndpointUrl</span></span>|<span data-ttu-id="8a600-146">String</span><span class="sxs-lookup"><span data-stu-id="8a600-146">String</span></span>|<span data-ttu-id="8a600-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="8a600-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="8a600-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-149">Boolean</span></span>|<span data-ttu-id="8a600-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="8a600-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="8a600-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="8a600-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="8a600-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-153">Boolean</span></span>|<span data-ttu-id="8a600-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="8a600-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="8a600-155">isDefault</span></span>|<span data-ttu-id="8a600-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-156">Boolean</span></span>|<span data-ttu-id="8a600-157">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="8a600-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="8a600-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="8a600-158">supervisedModeEnabled</span></span>|<span data-ttu-id="8a600-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-159">Boolean</span></span>|<span data-ttu-id="8a600-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="8a600-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="8a600-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="8a600-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="8a600-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="8a600-162">supportDepartment</span></span>|<span data-ttu-id="8a600-163">String</span><span class="sxs-lookup"><span data-stu-id="8a600-163">String</span></span>|<span data-ttu-id="8a600-164">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="8a600-164">Support department information</span></span>|
|<span data-ttu-id="8a600-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-165">passCodeDisabled</span></span>|<span data-ttu-id="8a600-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-166">Boolean</span></span>|<span data-ttu-id="8a600-167">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="8a600-168">isMandatory</span></span>|<span data-ttu-id="8a600-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-169">Boolean</span></span>|<span data-ttu-id="8a600-170">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="8a600-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="8a600-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-171">locationDisabled</span></span>|<span data-ttu-id="8a600-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-172">Boolean</span></span>|<span data-ttu-id="8a600-173">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="8a600-174">supportPhoneNumber</span></span>|<span data-ttu-id="8a600-175">String</span><span class="sxs-lookup"><span data-stu-id="8a600-175">String</span></span>|<span data-ttu-id="8a600-176">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="8a600-176">Support phone number</span></span>|
|<span data-ttu-id="8a600-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8a600-177">iTunesPairingMode</span></span>|[<span data-ttu-id="8a600-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="8a600-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="8a600-179">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="8a600-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="8a600-180">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="8a600-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="8a600-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-181">profileRemovalDisabled</span></span>|<span data-ttu-id="8a600-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-182">Boolean</span></span>|<span data-ttu-id="8a600-183">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8a600-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="8a600-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="8a600-184">managementCertificates</span></span>|<span data-ttu-id="8a600-185">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="8a600-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="8a600-186">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="8a600-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="8a600-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="8a600-187">restoreBlocked</span></span>|<span data-ttu-id="8a600-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-188">Boolean</span></span>|<span data-ttu-id="8a600-189">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="8a600-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="8a600-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="8a600-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-191">Boolean</span></span>|<span data-ttu-id="8a600-192">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="8a600-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="8a600-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-193">appleIdDisabled</span></span>|<span data-ttu-id="8a600-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-194">Boolean</span></span>|<span data-ttu-id="8a600-195">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="8a600-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-197">Boolean</span></span>|<span data-ttu-id="8a600-198">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-199">touchIdDisabled</span></span>|<span data-ttu-id="8a600-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-200">Boolean</span></span>|<span data-ttu-id="8a600-201">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-202">applePayDisabled</span></span>|<span data-ttu-id="8a600-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-203">Boolean</span></span>|<span data-ttu-id="8a600-204">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-205">zoomDisabled</span></span>|<span data-ttu-id="8a600-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-206">Boolean</span></span>|<span data-ttu-id="8a600-207">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-208">siriDisabled</span></span>|<span data-ttu-id="8a600-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-209">Boolean</span></span>|<span data-ttu-id="8a600-210">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-211">diagnosticsDisabled</span></span>|<span data-ttu-id="8a600-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-212">Boolean</span></span>|<span data-ttu-id="8a600-213">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="8a600-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="8a600-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-215">Boolean</span></span>|<span data-ttu-id="8a600-216">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="8a600-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="8a600-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="8a600-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-218">Boolean</span></span>|<span data-ttu-id="8a600-219">Indica se o compartimento de arquivos do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="8a600-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="8a600-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="8a600-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="8a600-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-221">Boolean</span></span>|<span data-ttu-id="8a600-222">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="8a600-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="8a600-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="8a600-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="8a600-224">Int32</span><span class="sxs-lookup"><span data-stu-id="8a600-224">Int32</span></span>|<span data-ttu-id="8a600-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8a600-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="8a600-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8a600-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="8a600-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="8a600-227">enableSharedIPad</span></span>|<span data-ttu-id="8a600-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="8a600-228">Boolean</span></span>|<span data-ttu-id="8a600-229">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="8a600-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="8a600-230">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="8a600-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="8a600-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a600-231">Response</span></span>
<span data-ttu-id="8a600-232">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="8a600-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8a600-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="8a600-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="8a600-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="8a600-234">Request</span></span>
<span data-ttu-id="8a600-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="8a600-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8a600-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="8a600-236">Response</span></span>
<span data-ttu-id="8a600-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="8a600-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




