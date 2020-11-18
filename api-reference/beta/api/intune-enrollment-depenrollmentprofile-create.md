---
title: Criar depEnrollmentProfile
description: Criar um novo objeto depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 076bb1e878b26d733ab3309e9bb4c1f1bf46678d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49202224"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="e2e8f-103">Criar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e2e8f-103">Create depEnrollmentProfile</span></span>

<span data-ttu-id="e2e8f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2e8f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e2e8f-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e2e8f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e2e8f-107">Criar um novo objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e2e8f-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2e8f-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e2e8f-108">Prerequisites</span></span>
<span data-ttu-id="e2e8f-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e2e8f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2e8f-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e2e8f-111">Permission type</span></span>|<span data-ttu-id="e2e8f-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2e8f-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e2e8f-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2e8f-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e2e8f-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2e8f-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-116">Not supported.</span></span>|
|<span data-ttu-id="e2e8f-117">Application</span><span class="sxs-lookup"><span data-stu-id="e2e8f-117">Application</span></span>|<span data-ttu-id="e2e8f-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2e8f-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2e8f-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e2e8f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e2e8f-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e2e8f-120">Request headers</span></span>
|<span data-ttu-id="e2e8f-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e2e8f-121">Header</span></span>|<span data-ttu-id="e2e8f-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e2e8f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2e8f-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e2e8f-123">Authorization</span></span>|<span data-ttu-id="e2e8f-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2e8f-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e2e8f-125">Accept</span></span>|<span data-ttu-id="e2e8f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e2e8f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2e8f-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e2e8f-127">Request body</span></span>
<span data-ttu-id="e2e8f-128">No corpo da solicitação, forneça uma representação JSON do objeto depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="e2e8f-129">A tabela a seguir mostra as propriedades que são necessárias ao criar depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="e2e8f-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e2e8f-130">Property</span></span>|<span data-ttu-id="e2e8f-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e2e8f-131">Type</span></span>|<span data-ttu-id="e2e8f-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e2e8f-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2e8f-133">id</span><span class="sxs-lookup"><span data-stu-id="e2e8f-133">id</span></span>|<span data-ttu-id="e2e8f-134">String</span><span class="sxs-lookup"><span data-stu-id="e2e8f-134">String</span></span>|<span data-ttu-id="e2e8f-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e2e8f-136">displayName</span></span>|<span data-ttu-id="e2e8f-137">String</span><span class="sxs-lookup"><span data-stu-id="e2e8f-137">String</span></span>|<span data-ttu-id="e2e8f-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-139">description</span><span class="sxs-lookup"><span data-stu-id="e2e8f-139">description</span></span>|<span data-ttu-id="e2e8f-140">String</span><span class="sxs-lookup"><span data-stu-id="e2e8f-140">String</span></span>|<span data-ttu-id="e2e8f-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e2e8f-142">requiresUserAuthentication</span></span>|<span data-ttu-id="e2e8f-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-143">Boolean</span></span>|<span data-ttu-id="e2e8f-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e2e8f-145">configurationEndpointUrl</span></span>|<span data-ttu-id="e2e8f-146">String</span><span class="sxs-lookup"><span data-stu-id="e2e8f-146">String</span></span>|<span data-ttu-id="e2e8f-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="e2e8f-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e2e8f-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-149">Boolean</span></span>|<span data-ttu-id="e2e8f-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="e2e8f-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="e2e8f-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="e2e8f-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-153">Boolean</span></span>|<span data-ttu-id="e2e8f-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e2e8f-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="e2e8f-155">isDefault</span></span>|<span data-ttu-id="e2e8f-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-156">Boolean</span></span>|<span data-ttu-id="e2e8f-157">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="e2e8f-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="e2e8f-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-158">supervisedModeEnabled</span></span>|<span data-ttu-id="e2e8f-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-159">Boolean</span></span>|<span data-ttu-id="e2e8f-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="e2e8f-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="e2e8f-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="e2e8f-162">supportDepartment</span></span>|<span data-ttu-id="e2e8f-163">String</span><span class="sxs-lookup"><span data-stu-id="e2e8f-163">String</span></span>|<span data-ttu-id="e2e8f-164">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="e2e8f-164">Support department information</span></span>|
|<span data-ttu-id="e2e8f-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-165">passCodeDisabled</span></span>|<span data-ttu-id="e2e8f-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-166">Boolean</span></span>|<span data-ttu-id="e2e8f-167">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="e2e8f-168">isMandatory</span></span>|<span data-ttu-id="e2e8f-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-169">Boolean</span></span>|<span data-ttu-id="e2e8f-170">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="e2e8f-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="e2e8f-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-171">locationDisabled</span></span>|<span data-ttu-id="e2e8f-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-172">Boolean</span></span>|<span data-ttu-id="e2e8f-173">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e2e8f-174">supportPhoneNumber</span></span>|<span data-ttu-id="e2e8f-175">String</span><span class="sxs-lookup"><span data-stu-id="e2e8f-175">String</span></span>|<span data-ttu-id="e2e8f-176">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="e2e8f-176">Support phone number</span></span>|
|<span data-ttu-id="e2e8f-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="e2e8f-177">iTunesPairingMode</span></span>|[<span data-ttu-id="e2e8f-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="e2e8f-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="e2e8f-179">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="e2e8f-180">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="e2e8f-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-181">profileRemovalDisabled</span></span>|<span data-ttu-id="e2e8f-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-182">Boolean</span></span>|<span data-ttu-id="e2e8f-183">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="e2e8f-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="e2e8f-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="e2e8f-184">managementCertificates</span></span>|<span data-ttu-id="e2e8f-185">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="e2e8f-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="e2e8f-186">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="e2e8f-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="e2e8f-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e2e8f-187">restoreBlocked</span></span>|<span data-ttu-id="e2e8f-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-188">Boolean</span></span>|<span data-ttu-id="e2e8f-189">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="e2e8f-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="e2e8f-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-191">Boolean</span></span>|<span data-ttu-id="e2e8f-192">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="e2e8f-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="e2e8f-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-193">appleIdDisabled</span></span>|<span data-ttu-id="e2e8f-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-194">Boolean</span></span>|<span data-ttu-id="e2e8f-195">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="e2e8f-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-197">Boolean</span></span>|<span data-ttu-id="e2e8f-198">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-199">touchIdDisabled</span></span>|<span data-ttu-id="e2e8f-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-200">Boolean</span></span>|<span data-ttu-id="e2e8f-201">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-202">applePayDisabled</span></span>|<span data-ttu-id="e2e8f-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-203">Boolean</span></span>|<span data-ttu-id="e2e8f-204">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-205">zoomDisabled</span></span>|<span data-ttu-id="e2e8f-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-206">Boolean</span></span>|<span data-ttu-id="e2e8f-207">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-208">siriDisabled</span></span>|<span data-ttu-id="e2e8f-209">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-209">Boolean</span></span>|<span data-ttu-id="e2e8f-210">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-211">diagnosticsDisabled</span></span>|<span data-ttu-id="e2e8f-212">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-212">Boolean</span></span>|<span data-ttu-id="e2e8f-213">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="e2e8f-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="e2e8f-215">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-215">Boolean</span></span>|<span data-ttu-id="e2e8f-216">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="e2e8f-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="e2e8f-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="e2e8f-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-218">Boolean</span></span>|<span data-ttu-id="e2e8f-219">Indica se o compartimento de arquivos do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e2e8f-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="e2e8f-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="e2e8f-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="e2e8f-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-221">Boolean</span></span>|<span data-ttu-id="e2e8f-222">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="e2e8f-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="e2e8f-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="e2e8f-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="e2e8f-224">Int32</span><span class="sxs-lookup"><span data-stu-id="e2e8f-224">Int32</span></span>|<span data-ttu-id="e2e8f-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="e2e8f-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="e2e8f-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="e2e8f-227">enableSharedIPad</span></span>|<span data-ttu-id="e2e8f-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="e2e8f-228">Boolean</span></span>|<span data-ttu-id="e2e8f-229">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="e2e8f-230">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="e2e8f-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2e8f-231">Response</span></span>
<span data-ttu-id="e2e8f-232">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2e8f-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e2e8f-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="e2e8f-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e2e8f-234">Request</span></span>
<span data-ttu-id="e2e8f-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-235">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="e2e8f-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="e2e8f-236">Response</span></span>
<span data-ttu-id="e2e8f-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e2e8f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




