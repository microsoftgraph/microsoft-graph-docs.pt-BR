---
title: Criar depIOSEnrollmentProfile
description: Crie um novo objeto de depIOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a716e088dd9bcad19bc01a23f012f1a3cd5b3373
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398783"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="fdc04-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="fdc04-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="fdc04-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="fdc04-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fdc04-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="fdc04-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fdc04-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="fdc04-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fdc04-107">Crie um novo objeto de [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="fdc04-107">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fdc04-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="fdc04-108">Prerequisites</span></span>
<span data-ttu-id="fdc04-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="fdc04-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fdc04-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="fdc04-111">Permission type</span></span>|<span data-ttu-id="fdc04-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="fdc04-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fdc04-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="fdc04-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fdc04-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdc04-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="fdc04-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="fdc04-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fdc04-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdc04-116">Not supported.</span></span>|
|<span data-ttu-id="fdc04-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="fdc04-117">Application</span></span>|<span data-ttu-id="fdc04-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="fdc04-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fdc04-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="fdc04-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="fdc04-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="fdc04-120">Request headers</span></span>
|<span data-ttu-id="fdc04-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="fdc04-121">Header</span></span>|<span data-ttu-id="fdc04-122">Valor</span><span class="sxs-lookup"><span data-stu-id="fdc04-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fdc04-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="fdc04-123">Authorization</span></span>|<span data-ttu-id="fdc04-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="fdc04-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fdc04-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="fdc04-125">Accept</span></span>|<span data-ttu-id="fdc04-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fdc04-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdc04-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="fdc04-127">Request body</span></span>
<span data-ttu-id="fdc04-128">No corpo da solicitação, fornece uma representação JSON para o objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="fdc04-128">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="fdc04-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="fdc04-129">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="fdc04-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="fdc04-130">Property</span></span>|<span data-ttu-id="fdc04-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="fdc04-131">Type</span></span>|<span data-ttu-id="fdc04-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="fdc04-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fdc04-133">id</span><span class="sxs-lookup"><span data-stu-id="fdc04-133">id</span></span>|<span data-ttu-id="fdc04-134">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-134">String</span></span>|<span data-ttu-id="fdc04-135">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-136">displayName</span><span class="sxs-lookup"><span data-stu-id="fdc04-136">displayName</span></span>|<span data-ttu-id="fdc04-137">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-137">String</span></span>|<span data-ttu-id="fdc04-138">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-139">description</span><span class="sxs-lookup"><span data-stu-id="fdc04-139">description</span></span>|<span data-ttu-id="fdc04-140">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-140">String</span></span>|<span data-ttu-id="fdc04-141">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="fdc04-142">requiresUserAuthentication</span></span>|<span data-ttu-id="fdc04-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-143">Boolean</span></span>|<span data-ttu-id="fdc04-144">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="fdc04-145">configurationEndpointUrl</span></span>|<span data-ttu-id="fdc04-146">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-146">String</span></span>|<span data-ttu-id="fdc04-147">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="fdc04-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="fdc04-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-149">Boolean</span></span>|<span data-ttu-id="fdc04-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="fdc04-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="fdc04-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="fdc04-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="fdc04-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-153">Boolean</span></span>|<span data-ttu-id="fdc04-154">Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="fdc04-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="fdc04-155">isDefault</span></span>|<span data-ttu-id="fdc04-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-156">Boolean</span></span>|<span data-ttu-id="fdc04-157">Indica se esse é o perfil padrão Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-158">supervisedModeEnabled</span></span>|<span data-ttu-id="fdc04-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-159">Boolean</span></span>|<span data-ttu-id="fdc04-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="fdc04-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="fdc04-161">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="fdc04-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="fdc04-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="fdc04-163">supportDepartment</span></span>|<span data-ttu-id="fdc04-164">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-164">String</span></span>|<span data-ttu-id="fdc04-165">Informações de departamento de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-166">passCodeDisabled</span></span>|<span data-ttu-id="fdc04-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-167">Boolean</span></span>|<span data-ttu-id="fdc04-168">Indica se a senha instalação painel está desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="fdc04-169">isMandatory</span></span>|<span data-ttu-id="fdc04-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-170">Boolean</span></span>|<span data-ttu-id="fdc04-171">Indica se o perfil é obrigatória herdar de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-172">locationDisabled</span></span>|<span data-ttu-id="fdc04-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-173">Boolean</span></span>|<span data-ttu-id="fdc04-174">Indica se o local do painel de configuração do serviço é desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="fdc04-175">supportPhoneNumber</span></span>|<span data-ttu-id="fdc04-176">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-176">String</span></span>|<span data-ttu-id="fdc04-177">Número de telefone de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-178">profileRemovalDisabled</span></span>|<span data-ttu-id="fdc04-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-179">Boolean</span></span>|<span data-ttu-id="fdc04-180">Indica se a opção de remoção de perfil será desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="fdc04-181">restoreBlocked</span></span>|<span data-ttu-id="fdc04-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-182">Boolean</span></span>|<span data-ttu-id="fdc04-183">Indica se o painel de configuração de restauração será bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-184">appleIdDisabled</span></span>|<span data-ttu-id="fdc04-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-185">Boolean</span></span>|<span data-ttu-id="fdc04-186">Indica se o Apple painel de configuração de id estará desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="fdc04-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-188">Boolean</span></span>|<span data-ttu-id="fdc04-189">Indica se o painel de configuração de 'Termos e condições' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-190">touchIdDisabled</span></span>|<span data-ttu-id="fdc04-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-191">Boolean</span></span>|<span data-ttu-id="fdc04-192">Indica se o painel de configuração de id de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-193">applePayDisabled</span></span>|<span data-ttu-id="fdc04-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-194">Boolean</span></span>|<span data-ttu-id="fdc04-195">Indica se o painel de configuração de pagamento do Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-196">zoomDisabled</span></span>|<span data-ttu-id="fdc04-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-197">Boolean</span></span>|<span data-ttu-id="fdc04-198">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-199">siriDisabled</span></span>|<span data-ttu-id="fdc04-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-200">Boolean</span></span>|<span data-ttu-id="fdc04-201">Indica se o painel de configuração de siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-202">diagnosticsDisabled</span></span>|<span data-ttu-id="fdc04-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-203">Boolean</span></span>|<span data-ttu-id="fdc04-204">Indica se o diagnóstico do painel de instalação está desabilitada Inherited em [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="fdc04-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-206">Boolean</span></span>|<span data-ttu-id="fdc04-207">Indica se a tela de instalação do displaytone está desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-208">privacyPaneDisabled</span></span>|<span data-ttu-id="fdc04-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-209">Boolean</span></span>|<span data-ttu-id="fdc04-210">Indica se a tela de privacidade está desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="fdc04-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="fdc04-211">iTunesPairingMode</span></span>|[<span data-ttu-id="fdc04-212">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="fdc04-212">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="fdc04-213">Indica a modo de emparelhamento de iTunes.</span><span class="sxs-lookup"><span data-stu-id="fdc04-213">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="fdc04-214">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="fdc04-214">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="fdc04-215">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="fdc04-215">managementCertificates</span></span>|<span data-ttu-id="fdc04-216">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="fdc04-216">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="fdc04-217">Certificados de gerenciamento para configurador da Apple</span><span class="sxs-lookup"><span data-stu-id="fdc04-217">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="fdc04-218">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-218">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="fdc04-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-219">Boolean</span></span>|<span data-ttu-id="fdc04-220">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-220">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="fdc04-221">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="fdc04-221">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="fdc04-222">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-222">Boolean</span></span>|<span data-ttu-id="fdc04-223">Indica se o dispositivo será necessário aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="fdc04-223">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="fdc04-224">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="fdc04-224">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="fdc04-225">Int32</span><span class="sxs-lookup"><span data-stu-id="fdc04-225">Int32</span></span>|<span data-ttu-id="fdc04-226">Especifica o número máximo de usuários que podem utilizar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="fdc04-226">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="fdc04-227">Só é aplicável no modo compartilhado iPad.</span><span class="sxs-lookup"><span data-stu-id="fdc04-227">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="fdc04-228">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="fdc04-228">enableSharedIPad</span></span>|<span data-ttu-id="fdc04-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-229">Boolean</span></span>|<span data-ttu-id="fdc04-230">Isso indica se o dispositivo é registrado em um modo que permite que vários cenários de usuário.</span><span class="sxs-lookup"><span data-stu-id="fdc04-230">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="fdc04-231">Só é aplicável no compartilhados iPads.</span><span class="sxs-lookup"><span data-stu-id="fdc04-231">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="fdc04-232">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="fdc04-232">companyPortalVppTokenId</span></span>|<span data-ttu-id="fdc04-233">String</span><span class="sxs-lookup"><span data-stu-id="fdc04-233">String</span></span>|<span data-ttu-id="fdc04-234">Se definido, que indica qual token Vpp deve ser usado para implantar o Portal da empresa c / licenciamento do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="fdc04-234">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="fdc04-235">'enableAuthenticationViaCompanyPortal' deve ser definida para que essa propriedade ser definida.</span><span class="sxs-lookup"><span data-stu-id="fdc04-235">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="fdc04-236">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="fdc04-236">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="fdc04-237">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-237">Boolean</span></span>|<span data-ttu-id="fdc04-238">Informa o dispositivo para habilitar o modo de aplicativo único e aplicar o app-lock durante o registro.</span><span class="sxs-lookup"><span data-stu-id="fdc04-238">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="fdc04-239">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="fdc04-239">Default is false.</span></span> <span data-ttu-id="fdc04-240">'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidas para que essa propriedade ser definida.</span><span class="sxs-lookup"><span data-stu-id="fdc04-240">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="fdc04-241">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-241">homeButtonScreenDisabled</span></span>|<span data-ttu-id="fdc04-242">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-242">Boolean</span></span>|<span data-ttu-id="fdc04-243">Indica se a tela de sensibilidade do botão página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-243">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="fdc04-244">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-244">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="fdc04-245">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-245">Boolean</span></span>|<span data-ttu-id="fdc04-246">Indica se iMessage e FaceTime tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-246">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="fdc04-247">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-247">onBoardingScreenDisabled</span></span>|<span data-ttu-id="fdc04-248">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-248">Boolean</span></span>|<span data-ttu-id="fdc04-249">Indica se a tela de instalação de inclusão está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-249">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="fdc04-250">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-250">screenTimeScreenDisabled</span></span>|<span data-ttu-id="fdc04-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-251">Boolean</span></span>|<span data-ttu-id="fdc04-252">Indica se a configuração de tempo limite de tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-252">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="fdc04-253">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-253">simSetupScreenDisabled</span></span>|<span data-ttu-id="fdc04-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-254">Boolean</span></span>|<span data-ttu-id="fdc04-255">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-255">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="fdc04-256">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-256">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="fdc04-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-257">Boolean</span></span>|<span data-ttu-id="fdc04-258">Indica se a tela de atualização de software obrigatório está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-258">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="fdc04-259">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="fdc04-259">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="fdc04-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="fdc04-260">Boolean</span></span>|<span data-ttu-id="fdc04-261">Indica se a tela de migração de inspeção está desabilitada</span><span class="sxs-lookup"><span data-stu-id="fdc04-261">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="fdc04-262">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdc04-262">Response</span></span>
<span data-ttu-id="fdc04-263">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="fdc04-263">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdc04-264">Exemplo</span><span class="sxs-lookup"><span data-stu-id="fdc04-264">Example</span></span>

### <a name="request"></a><span data-ttu-id="fdc04-265">Solicitação</span><span class="sxs-lookup"><span data-stu-id="fdc04-265">Request</span></span>
<span data-ttu-id="fdc04-266">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="fdc04-266">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fdc04-267">Resposta</span><span class="sxs-lookup"><span data-stu-id="fdc04-267">Response</span></span>
<span data-ttu-id="fdc04-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="fdc04-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




