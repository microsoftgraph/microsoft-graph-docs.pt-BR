---
title: Atualizar depEnrollmentProfile
description: Atualize as propriedades de um objeto depEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5e85e539200fbb6ddb661d5fb28ce0da8353dbec
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145989"
---
# <a name="update-depenrollmentprofile"></a><span data-ttu-id="5b642-103">Atualizar depEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5b642-103">Update depEnrollmentProfile</span></span>

<span data-ttu-id="5b642-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5b642-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5b642-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="5b642-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5b642-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5b642-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b642-107">Atualize as propriedades de [um objeto depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-107">Update the properties of a [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b642-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5b642-108">Prerequisites</span></span>
<span data-ttu-id="5b642-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5b642-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5b642-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5b642-111">Permission type</span></span>|<span data-ttu-id="5b642-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5b642-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b642-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5b642-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5b642-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b642-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5b642-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5b642-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b642-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5b642-116">Not supported.</span></span>|
|<span data-ttu-id="5b642-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5b642-117">Application</span></span>|<span data-ttu-id="5b642-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b642-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b642-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5b642-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="5b642-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5b642-120">Request headers</span></span>
|<span data-ttu-id="5b642-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5b642-121">Header</span></span>|<span data-ttu-id="5b642-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5b642-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b642-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5b642-123">Authorization</span></span>|<span data-ttu-id="5b642-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5b642-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b642-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5b642-125">Accept</span></span>|<span data-ttu-id="5b642-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5b642-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b642-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5b642-127">Request body</span></span>
<span data-ttu-id="5b642-128">No corpo da solicitação, fornece uma representação JSON para o [objeto depEnrollmentProfile.](../resources/intune-enrollment-depenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-128">In the request body, supply a JSON representation for the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object.</span></span>

<span data-ttu-id="5b642-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="5b642-129">The following table shows the properties that are required when you create the [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md).</span></span>

|<span data-ttu-id="5b642-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5b642-130">Property</span></span>|<span data-ttu-id="5b642-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5b642-131">Type</span></span>|<span data-ttu-id="5b642-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5b642-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b642-133">id</span><span class="sxs-lookup"><span data-stu-id="5b642-133">id</span></span>|<span data-ttu-id="5b642-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b642-134">String</span></span>|<span data-ttu-id="5b642-135">O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5b642-136">displayName</span></span>|<span data-ttu-id="5b642-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b642-137">String</span></span>|<span data-ttu-id="5b642-138">Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-139">descrição</span><span class="sxs-lookup"><span data-stu-id="5b642-139">description</span></span>|<span data-ttu-id="5b642-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b642-140">String</span></span>|<span data-ttu-id="5b642-141">Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="5b642-142">requiresUserAuthentication</span></span>|<span data-ttu-id="5b642-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-143">Boolean</span></span>|<span data-ttu-id="5b642-144">Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="5b642-145">configurationEndpointUrl</span></span>|<span data-ttu-id="5b642-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b642-146">String</span></span>|<span data-ttu-id="5b642-147">URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="5b642-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="5b642-149">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-149">Boolean</span></span>|<span data-ttu-id="5b642-150">Indica a autenticação com o Assistente de Instalação da Apple em vez do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="5b642-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="5b642-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="5b642-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="5b642-153">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-153">Boolean</span></span>|<span data-ttu-id="5b642-154">Indica que o Portal da Empresa é necessário em dispositivos inscritos pelo assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="5b642-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="5b642-155">isDefault</span></span>|<span data-ttu-id="5b642-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="5b642-156">Boolean</span></span>|<span data-ttu-id="5b642-157">Indica se esse é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="5b642-157">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="5b642-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="5b642-158">supervisedModeEnabled</span></span>|<span data-ttu-id="5b642-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-159">Boolean</span></span>|<span data-ttu-id="5b642-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="5b642-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="5b642-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5b642-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="5b642-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="5b642-162">supportDepartment</span></span>|<span data-ttu-id="5b642-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b642-163">String</span></span>|<span data-ttu-id="5b642-164">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="5b642-164">Support department information</span></span>|
|<span data-ttu-id="5b642-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-165">passCodeDisabled</span></span>|<span data-ttu-id="5b642-166">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-166">Boolean</span></span>|<span data-ttu-id="5b642-167">Indica se o painel de configuração senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-167">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="5b642-168">isMandatory</span></span>|<span data-ttu-id="5b642-169">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-169">Boolean</span></span>|<span data-ttu-id="5b642-170">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="5b642-170">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="5b642-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-171">locationDisabled</span></span>|<span data-ttu-id="5b642-172">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-172">Boolean</span></span>|<span data-ttu-id="5b642-173">Indica se o painel de configuração do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-173">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="5b642-174">supportPhoneNumber</span></span>|<span data-ttu-id="5b642-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5b642-175">String</span></span>|<span data-ttu-id="5b642-176">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="5b642-176">Support phone number</span></span>|
|<span data-ttu-id="5b642-177">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="5b642-177">iTunesPairingMode</span></span>|[<span data-ttu-id="5b642-178">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="5b642-178">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="5b642-179">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="5b642-179">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="5b642-180">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="5b642-180">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="5b642-181">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-181">profileRemovalDisabled</span></span>|<span data-ttu-id="5b642-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-182">Boolean</span></span>|<span data-ttu-id="5b642-183">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="5b642-183">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="5b642-184">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="5b642-184">managementCertificates</span></span>|<span data-ttu-id="5b642-185">[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="5b642-185">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="5b642-186">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="5b642-186">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="5b642-187">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="5b642-187">restoreBlocked</span></span>|<span data-ttu-id="5b642-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-188">Boolean</span></span>|<span data-ttu-id="5b642-189">Indica se o painel restaurar instalação está bloqueado</span><span class="sxs-lookup"><span data-stu-id="5b642-189">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="5b642-190">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-190">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="5b642-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-191">Boolean</span></span>|<span data-ttu-id="5b642-192">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="5b642-192">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="5b642-193">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-193">appleIdDisabled</span></span>|<span data-ttu-id="5b642-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-194">Boolean</span></span>|<span data-ttu-id="5b642-195">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-195">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-196">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-196">termsAndConditionsDisabled</span></span>|<span data-ttu-id="5b642-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-197">Boolean</span></span>|<span data-ttu-id="5b642-198">Indica se o painel de configuração 'Termos e Condições' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-198">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-199">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-199">touchIdDisabled</span></span>|<span data-ttu-id="5b642-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-200">Boolean</span></span>|<span data-ttu-id="5b642-201">Indica se o painel de configuração de ID por toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-201">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-202">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-202">applePayDisabled</span></span>|<span data-ttu-id="5b642-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-203">Boolean</span></span>|<span data-ttu-id="5b642-204">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-204">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-205">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-205">zoomDisabled</span></span>|<span data-ttu-id="5b642-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-206">Boolean</span></span>|<span data-ttu-id="5b642-207">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-207">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-208">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-208">siriDisabled</span></span>|<span data-ttu-id="5b642-209">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-209">Boolean</span></span>|<span data-ttu-id="5b642-210">Indica se o painel de configuração de siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-210">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-211">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-211">diagnosticsDisabled</span></span>|<span data-ttu-id="5b642-212">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-212">Boolean</span></span>|<span data-ttu-id="5b642-213">Indica se o painel de configuração de diagnósticos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-213">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="5b642-214">macOSRegistrationDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-214">macOSRegistrationDisabled</span></span>|<span data-ttu-id="5b642-215">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-215">Boolean</span></span>|<span data-ttu-id="5b642-216">Indica se o registro do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-216">Indicates if Mac OS registration is disabled</span></span>|
|<span data-ttu-id="5b642-217">macOSFileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="5b642-217">macOSFileVaultDisabled</span></span>|<span data-ttu-id="5b642-218">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-218">Boolean</span></span>|<span data-ttu-id="5b642-219">Indica se o cofre de arquivos do Mac OS está desabilitado</span><span class="sxs-lookup"><span data-stu-id="5b642-219">Indicates if Mac OS file vault is disabled</span></span>|
|<span data-ttu-id="5b642-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="5b642-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="5b642-221">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-221">Boolean</span></span>|<span data-ttu-id="5b642-222">Indica se o dispositivo precisará aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="5b642-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="5b642-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="5b642-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="5b642-224">Int32</span><span class="sxs-lookup"><span data-stu-id="5b642-224">Int32</span></span>|<span data-ttu-id="5b642-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5b642-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="5b642-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="5b642-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="5b642-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="5b642-227">enableSharedIPad</span></span>|<span data-ttu-id="5b642-228">Booleano</span><span class="sxs-lookup"><span data-stu-id="5b642-228">Boolean</span></span>|<span data-ttu-id="5b642-229">Isso indica se o dispositivo deve ser inscrito em um modo que habilita cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="5b642-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="5b642-230">Aplicável somente em iPads compartilhados.</span><span class="sxs-lookup"><span data-stu-id="5b642-230">Only applicable in shared iPads.</span></span>|



## <a name="response"></a><span data-ttu-id="5b642-231">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b642-231">Response</span></span>
<span data-ttu-id="5b642-232">Se tiver êxito, este método retornará um código de resposta e um `200 OK` objeto [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5b642-232">If successful, this method returns a `200 OK` response code and an updated [depEnrollmentProfile](../resources/intune-enrollment-depenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b642-233">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5b642-233">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b642-234">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5b642-234">Request</span></span>
<span data-ttu-id="5b642-235">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5b642-235">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5b642-236">Resposta</span><span class="sxs-lookup"><span data-stu-id="5b642-236">Response</span></span>
<span data-ttu-id="5b642-p107">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5b642-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




