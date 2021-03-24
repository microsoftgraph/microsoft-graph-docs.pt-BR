---
title: Criar depEnrollmentProfile
description: Crie um novo objeto depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 72dd66b0cb453966f1c6701e1ae5b0316506f508
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51149916"
---
# <a name="create-depenrollmentprofile"></a><span data-ttu-id="ca12d-103">Criar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="ca12d-103">Create depEnrollmentProfile</span></span>

<span data-ttu-id="ca12d-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ca12d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ca12d-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ca12d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca12d-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ca12d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca12d-107">Crie um novo [objeto depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-107">Create a new [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca12d-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca12d-108">Prerequisites</span></span>
<span data-ttu-id="ca12d-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca12d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca12d-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca12d-111">Permission type</span></span>|<span data-ttu-id="ca12d-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="ca12d-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca12d-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca12d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca12d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca12d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ca12d-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca12d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca12d-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca12d-116">Not supported.</span></span>|
|<span data-ttu-id="ca12d-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca12d-117">Application</span></span>|<span data-ttu-id="ca12d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca12d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca12d-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca12d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="ca12d-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca12d-120">Request headers</span></span>
|<span data-ttu-id="ca12d-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca12d-121">Header</span></span>|<span data-ttu-id="ca12d-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca12d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca12d-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca12d-123">Authorization</span></span>|<span data-ttu-id="ca12d-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca12d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca12d-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca12d-125">Accept</span></span>|<span data-ttu-id="ca12d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca12d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca12d-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca12d-127">Request body</span></span>
<span data-ttu-id="ca12d-128">No corpo da solicitação, fornece uma representação JSON para o objeto depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="ca12d-128">In the request body, supply a JSON representation for the depEnrollmentProfile object.</span></span>

<span data-ttu-id="ca12d-129">A tabela a seguir mostra as propriedades que são necessárias ao criar o depEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="ca12d-129">The following table shows the properties that are required when you create the depEnrollmentProfile.</span></span>

|<span data-ttu-id="ca12d-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca12d-130">Property</span></span>|<span data-ttu-id="ca12d-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca12d-131">Type</span></span>|<span data-ttu-id="ca12d-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca12d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca12d-133">id</span><span class="sxs-lookup"><span data-stu-id="ca12d-133">id</span></span>|<span data-ttu-id="ca12d-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca12d-134">String</span></span>|<span data-ttu-id="ca12d-135">O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ca12d-136">displayName</span></span>|<span data-ttu-id="ca12d-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca12d-137">String</span></span>|<span data-ttu-id="ca12d-138">Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-139">descrição</span><span class="sxs-lookup"><span data-stu-id="ca12d-139">description</span></span>|<span data-ttu-id="ca12d-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca12d-140">String</span></span>|<span data-ttu-id="ca12d-141">Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ca12d-142">requiresUserAuthentication</span></span>|<span data-ttu-id="ca12d-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-143">Boolean</span></span>|<span data-ttu-id="ca12d-144">Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ca12d-145">configurationEndpointUrl</span></span>|<span data-ttu-id="ca12d-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca12d-146">String</span></span>|<span data-ttu-id="ca12d-147">URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="ca12d-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ca12d-149">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-149">Boolean</span></span>|<span data-ttu-id="ca12d-150">Indica a autenticação com o Assistente de Instalação da Apple em vez do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="ca12d-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ca12d-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ca12d-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ca12d-153">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-153">Boolean</span></span>|<span data-ttu-id="ca12d-154">Indica que o Portal da Empresa é necessário em dispositivos inscritos pelo assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ca12d-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="ca12d-155">isDefault</span></span>|<span data-ttu-id="ca12d-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca12d-156">Boolean</span></span>|<span data-ttu-id="ca12d-157">Indica se esse é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="ca12d-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ca12d-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-158">supervisedModeEnabled</span></span>|<span data-ttu-id="ca12d-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-159">Boolean</span></span>|<span data-ttu-id="ca12d-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="ca12d-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ca12d-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="ca12d-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ca12d-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ca12d-162">supportDepartment</span></span>|<span data-ttu-id="ca12d-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca12d-163">String</span></span>|<span data-ttu-id="ca12d-164">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="ca12d-164">Support department information</span></span>|
|<span data-ttu-id="ca12d-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-165">passCodeDisabled</span></span>|<span data-ttu-id="ca12d-166">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-166">Boolean</span></span>|<span data-ttu-id="ca12d-167">Indica se o painel de configuração senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="ca12d-168">isMandatory</span></span>|<span data-ttu-id="ca12d-169">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-169">Boolean</span></span>|<span data-ttu-id="ca12d-170">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="ca12d-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ca12d-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-171">locationDisabled</span></span>|<span data-ttu-id="ca12d-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-172">Boolean</span></span>|<span data-ttu-id="ca12d-173">Indica se o painel de configuração do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ca12d-174">supportPhoneNumber</span></span>|<span data-ttu-id="ca12d-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca12d-175">String</span></span>|<span data-ttu-id="ca12d-176">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="ca12d-176">Support phone number</span></span>|
|<span data-ttu-id="ca12d-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ca12d-177">iTunesPairingMode</span></span>|[<span data-ttu-id="ca12d-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="ca12d-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="ca12d-179">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="ca12d-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="ca12d-180">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="ca12d-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="ca12d-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-181">profileRemovalDisabled</span></span>|<span data-ttu-id="ca12d-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-182">Boolean</span></span>|<span data-ttu-id="ca12d-183">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ca12d-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ca12d-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="ca12d-184">managementCertificates</span></span>|<span data-ttu-id="ca12d-185">[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="ca12d-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="ca12d-186">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="ca12d-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="ca12d-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ca12d-187">restoreBlocked</span></span>|<span data-ttu-id="ca12d-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-188">Boolean</span></span>|<span data-ttu-id="ca12d-189">Indica se o painel restaurar instalação está bloqueado</span><span class="sxs-lookup"><span data-stu-id="ca12d-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ca12d-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="ca12d-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-191">Boolean</span></span>|<span data-ttu-id="ca12d-192">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ca12d-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="ca12d-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-193">appleIdDisabled</span></span>|<span data-ttu-id="ca12d-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-194">Boolean</span></span>|<span data-ttu-id="ca12d-195">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ca12d-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-197">Boolean</span></span>|<span data-ttu-id="ca12d-198">Indica se o painel de configuração 'Termos e Condições' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-199">touchIdDisabled</span></span>|<span data-ttu-id="ca12d-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-200">Boolean</span></span>|<span data-ttu-id="ca12d-201">Indica se o painel de configuração de ID por toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-202">applePayDisabled</span></span>|<span data-ttu-id="ca12d-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-203">Boolean</span></span>|<span data-ttu-id="ca12d-204">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-205">zoomDisabled</span></span>|<span data-ttu-id="ca12d-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-206">Boolean</span></span>|<span data-ttu-id="ca12d-207">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-208">siriDisabled</span></span>|<span data-ttu-id="ca12d-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-209">Boolean</span></span>|<span data-ttu-id="ca12d-210">Indica se o painel de configuração de siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-211">diagnosticsDisabled</span></span>|<span data-ttu-id="ca12d-212">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-212">Boolean</span></span>|<span data-ttu-id="ca12d-213">Indica se o painel de configuração de diagnósticos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="ca12d-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="ca12d-215">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-215">Boolean</span></span>|<span data-ttu-id="ca12d-216">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="ca12d-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="ca12d-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="ca12d-218">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-218">Boolean</span></span>|<span data-ttu-id="ca12d-219">Indica se o cofre de arquivos do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ca12d-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="ca12d-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="ca12d-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="ca12d-221">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-221">Boolean</span></span>|<span data-ttu-id="ca12d-222">Indica se o dispositivo precisará aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="ca12d-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="ca12d-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="ca12d-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="ca12d-224">Int32</span><span class="sxs-lookup"><span data-stu-id="ca12d-224">Int32</span></span>|<span data-ttu-id="ca12d-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="ca12d-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="ca12d-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="ca12d-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="ca12d-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="ca12d-227">enableSharedIPad</span></span>|<span data-ttu-id="ca12d-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="ca12d-228">Boolean</span></span>|<span data-ttu-id="ca12d-229">Isso indica se o dispositivo deve ser inscrito em um modo que habilita cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="ca12d-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="ca12d-230">Aplicável somente em iPads compartilhados.</span><span class="sxs-lookup"><span data-stu-id="ca12d-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="ca12d-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca12d-231">Response</span></span>
<span data-ttu-id="ca12d-232">Se tiver êxito, este método retornará um código de resposta e um `201 Created` [objeto depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca12d-232">If successful, this method returns a `201 Created` response code and a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca12d-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca12d-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca12d-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca12d-234">Request</span></span>
<span data-ttu-id="ca12d-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca12d-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca12d-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca12d-236">Response</span></span>
<span data-ttu-id="ca12d-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca12d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




