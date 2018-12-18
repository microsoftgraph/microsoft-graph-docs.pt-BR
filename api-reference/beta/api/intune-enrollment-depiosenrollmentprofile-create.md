---
title: Criar depIOSEnrollmentProfile
description: Crie um novo objeto de depIOSEnrollmentProfile.
author: tfitzmac
ms.openlocfilehash: f06457571a2630c32842a202d45107f768d345f2
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308571"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="f8b40-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f8b40-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="f8b40-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f8b40-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f8b40-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f8b40-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8b40-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f8b40-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f8b40-107">Crie um novo objeto de [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f8b40-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f8b40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f8b40-108">Prerequisites</span></span>
<span data-ttu-id="f8b40-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f8b40-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f8b40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f8b40-111">Permission type</span></span>|<span data-ttu-id="f8b40-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f8b40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8b40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f8b40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8b40-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8b40-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f8b40-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f8b40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8b40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8b40-116">Not supported.</span></span>|
|<span data-ttu-id="f8b40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f8b40-117">Application</span></span>|<span data-ttu-id="f8b40-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f8b40-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8b40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f8b40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="f8b40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f8b40-120">Request headers</span></span>
|<span data-ttu-id="f8b40-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f8b40-121">Header</span></span>|<span data-ttu-id="f8b40-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f8b40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8b40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f8b40-123">Authorization</span></span>|<span data-ttu-id="f8b40-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f8b40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8b40-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8b40-125">Accept</span></span>|<span data-ttu-id="f8b40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8b40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8b40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f8b40-127">Request body</span></span>
<span data-ttu-id="f8b40-128">No corpo da solicitação, fornece uma representação JSON para o objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="f8b40-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="f8b40-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="f8b40-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="f8b40-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f8b40-130">Property</span></span>|<span data-ttu-id="f8b40-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f8b40-131">Type</span></span>|<span data-ttu-id="f8b40-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f8b40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8b40-133">id</span><span class="sxs-lookup"><span data-stu-id="f8b40-133">id</span></span>|<span data-ttu-id="f8b40-134">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-134">String</span></span>|<span data-ttu-id="f8b40-135">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f8b40-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f8b40-136">displayName</span></span>|<span data-ttu-id="f8b40-137">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-137">String</span></span>|<span data-ttu-id="f8b40-138">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f8b40-139">description</span><span class="sxs-lookup"><span data-stu-id="f8b40-139">description</span></span>|<span data-ttu-id="f8b40-140">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-140">String</span></span>|<span data-ttu-id="f8b40-141">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f8b40-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f8b40-142">requiresUserAuthentication</span></span>|<span data-ttu-id="f8b40-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-143">Boolean</span></span>|<span data-ttu-id="f8b40-144">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f8b40-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f8b40-145">configurationEndpointUrl</span></span>|<span data-ttu-id="f8b40-146">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-146">String</span></span>|<span data-ttu-id="f8b40-147">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f8b40-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f8b40-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f8b40-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-149">Boolean</span></span>|<span data-ttu-id="f8b40-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="f8b40-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f8b40-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f8b40-152">isDefault</span><span class="sxs-lookup"><span data-stu-id="f8b40-152">isDefault</span></span>|<span data-ttu-id="f8b40-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-153">Boolean</span></span>|<span data-ttu-id="f8b40-154">Indica se esse é o perfil padrão Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-154">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-155">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-155">supervisedModeEnabled</span></span>|<span data-ttu-id="f8b40-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-156">Boolean</span></span>|<span data-ttu-id="f8b40-157">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="f8b40-157">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f8b40-158">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f8b40-158">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="f8b40-159">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-159">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-160">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f8b40-160">supportDepartment</span></span>|<span data-ttu-id="f8b40-161">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-161">String</span></span>|<span data-ttu-id="f8b40-162">Informações de departamento de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-162">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-163">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-163">passCodeDisabled</span></span>|<span data-ttu-id="f8b40-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-164">Boolean</span></span>|<span data-ttu-id="f8b40-165">Indica se a senha instalação painel está desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-165">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="f8b40-166">isMandatory</span></span>|<span data-ttu-id="f8b40-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-167">Boolean</span></span>|<span data-ttu-id="f8b40-168">Indica se o perfil é obrigatória herdar de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-169">locationDisabled</span></span>|<span data-ttu-id="f8b40-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-170">Boolean</span></span>|<span data-ttu-id="f8b40-171">Indica se o local do painel de configuração do serviço é desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f8b40-172">supportPhoneNumber</span></span>|<span data-ttu-id="f8b40-173">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-173">String</span></span>|<span data-ttu-id="f8b40-174">Número de telefone de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-175">profileRemovalDisabled</span></span>|<span data-ttu-id="f8b40-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-176">Boolean</span></span>|<span data-ttu-id="f8b40-177">Indica se a opção de remoção de perfil será desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f8b40-178">restoreBlocked</span></span>|<span data-ttu-id="f8b40-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-179">Boolean</span></span>|<span data-ttu-id="f8b40-180">Indica se o painel de configuração de restauração será bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-181">appleIdDisabled</span></span>|<span data-ttu-id="f8b40-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-182">Boolean</span></span>|<span data-ttu-id="f8b40-183">Indica se o Apple painel de configuração de id estará desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f8b40-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-185">Boolean</span></span>|<span data-ttu-id="f8b40-186">Indica se o painel de configuração de 'Termos e condições' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-187">touchIdDisabled</span></span>|<span data-ttu-id="f8b40-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-188">Boolean</span></span>|<span data-ttu-id="f8b40-189">Indica se o painel de configuração de id de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-190">applePayDisabled</span></span>|<span data-ttu-id="f8b40-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-191">Boolean</span></span>|<span data-ttu-id="f8b40-192">Indica se o painel de configuração de pagamento do Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-193">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-193">zoomDisabled</span></span>|<span data-ttu-id="f8b40-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-194">Boolean</span></span>|<span data-ttu-id="f8b40-195">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-195">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-196">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-196">siriDisabled</span></span>|<span data-ttu-id="f8b40-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-197">Boolean</span></span>|<span data-ttu-id="f8b40-198">Indica se o painel de configuração de siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-198">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-199">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-199">diagnosticsDisabled</span></span>|<span data-ttu-id="f8b40-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-200">Boolean</span></span>|<span data-ttu-id="f8b40-201">Indica se o diagnóstico do painel de instalação está desabilitada Inherited em [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-201">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f8b40-202">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="f8b40-202">iTunesPairingMode</span></span>|[<span data-ttu-id="f8b40-203">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="f8b40-203">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="f8b40-204">Indica a modo de emparelhamento de iTunes.</span><span class="sxs-lookup"><span data-stu-id="f8b40-204">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="f8b40-205">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="f8b40-205">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="f8b40-206">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="f8b40-206">managementCertificates</span></span>|<span data-ttu-id="f8b40-207">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="f8b40-207">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="f8b40-208">Certificados de gerenciamento para configurador da Apple</span><span class="sxs-lookup"><span data-stu-id="f8b40-208">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="f8b40-209">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="f8b40-209">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="f8b40-210">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-210">Boolean</span></span>|<span data-ttu-id="f8b40-211">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f8b40-211">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="f8b40-212">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="f8b40-212">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="f8b40-213">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-213">Boolean</span></span>|<span data-ttu-id="f8b40-214">Indica se o dispositivo será necessário aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="f8b40-214">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="f8b40-215">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="f8b40-215">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="f8b40-216">Int32</span><span class="sxs-lookup"><span data-stu-id="f8b40-216">Int32</span></span>|<span data-ttu-id="f8b40-217">Especifica o número máximo de usuários que podem utilizar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="f8b40-217">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="f8b40-218">Só é aplicável no modo compartilhado iPad.</span><span class="sxs-lookup"><span data-stu-id="f8b40-218">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="f8b40-219">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="f8b40-219">enableSharedIPad</span></span>|<span data-ttu-id="f8b40-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-220">Boolean</span></span>|<span data-ttu-id="f8b40-221">Isso indica se o dispositivo é registrado em um modo que permite que vários cenários de usuário.</span><span class="sxs-lookup"><span data-stu-id="f8b40-221">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="f8b40-222">Só é aplicável no compartilhados iPads.</span><span class="sxs-lookup"><span data-stu-id="f8b40-222">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="f8b40-223">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="f8b40-223">companyPortalVppTokenId</span></span>|<span data-ttu-id="f8b40-224">String</span><span class="sxs-lookup"><span data-stu-id="f8b40-224">String</span></span>|<span data-ttu-id="f8b40-225">Se definido, que indica qual token Vpp deve ser usado para implantar o Portal da empresa c / licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="f8b40-225">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="f8b40-226">'enableAuthenticationViaCompanyPortal' deve ser definida para que essa propriedade ser definida.</span><span class="sxs-lookup"><span data-stu-id="f8b40-226">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="f8b40-227">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="f8b40-227">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="f8b40-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="f8b40-228">Boolean</span></span>|<span data-ttu-id="f8b40-229">Informa o dispositivo para habilitar o modo de aplicativo único e aplicar o app-lock durante o registro.</span><span class="sxs-lookup"><span data-stu-id="f8b40-229">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="f8b40-230">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="f8b40-230">Default is false.</span></span> <span data-ttu-id="f8b40-231">'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidas para que essa propriedade ser definida.</span><span class="sxs-lookup"><span data-stu-id="f8b40-231">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|



## <a name="response"></a><span data-ttu-id="f8b40-232">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8b40-232">Response</span></span>
<span data-ttu-id="f8b40-233">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f8b40-233">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8b40-234">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f8b40-234">Example</span></span>
### <a name="request"></a><span data-ttu-id="f8b40-235">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f8b40-235">Request</span></span>
<span data-ttu-id="f8b40-236">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f8b40-236">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1329

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
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
  "enableSingleAppEnrollmentMode": true
}
```

### <a name="response"></a><span data-ttu-id="f8b40-237">Resposta</span><span class="sxs-lookup"><span data-stu-id="f8b40-237">Response</span></span>
<span data-ttu-id="f8b40-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f8b40-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1378

{
  "@odata.type": "#microsoft.graph.depIOSEnrollmentProfile",
  "id": "1ec10a60-0a60-1ec1-600a-c11e600ac11e",
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
  "enableSingleAppEnrollmentMode": true
}
```





