---
title: Atualizar depIOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12998cd361e51b4c4c9c6ecb0ddad946b6605295
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908774"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="94c5c-103">Atualizar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="94c5c-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="94c5c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="94c5c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94c5c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="94c5c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94c5c-106">Atualiza as propriedades de um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="94c5c-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="94c5c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="94c5c-107">Prerequisites</span></span>
<span data-ttu-id="94c5c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="94c5c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="94c5c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="94c5c-110">Permission type</span></span>|<span data-ttu-id="94c5c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="94c5c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="94c5c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="94c5c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="94c5c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="94c5c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="94c5c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="94c5c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="94c5c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94c5c-115">Not supported.</span></span>|
|<span data-ttu-id="94c5c-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="94c5c-116">Application</span></span>|<span data-ttu-id="94c5c-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="94c5c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="94c5c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="94c5c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="94c5c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="94c5c-119">Request headers</span></span>
|<span data-ttu-id="94c5c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="94c5c-120">Header</span></span>|<span data-ttu-id="94c5c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="94c5c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="94c5c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="94c5c-122">Authorization</span></span>|<span data-ttu-id="94c5c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="94c5c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="94c5c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="94c5c-124">Accept</span></span>|<span data-ttu-id="94c5c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="94c5c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="94c5c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="94c5c-126">Request body</span></span>
<span data-ttu-id="94c5c-127">No corpo da solicitação, forneça uma representação JSON do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="94c5c-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="94c5c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="94c5c-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="94c5c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="94c5c-129">Property</span></span>|<span data-ttu-id="94c5c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="94c5c-130">Type</span></span>|<span data-ttu-id="94c5c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="94c5c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94c5c-132">id</span><span class="sxs-lookup"><span data-stu-id="94c5c-132">id</span></span>|<span data-ttu-id="94c5c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c5c-133">String</span></span>|<span data-ttu-id="94c5c-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="94c5c-135">displayName</span></span>|<span data-ttu-id="94c5c-136">String</span><span class="sxs-lookup"><span data-stu-id="94c5c-136">String</span></span>|<span data-ttu-id="94c5c-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-138">description</span><span class="sxs-lookup"><span data-stu-id="94c5c-138">description</span></span>|<span data-ttu-id="94c5c-139">String</span><span class="sxs-lookup"><span data-stu-id="94c5c-139">String</span></span>|<span data-ttu-id="94c5c-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="94c5c-141">requiresUserAuthentication</span></span>|<span data-ttu-id="94c5c-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-142">Boolean</span></span>|<span data-ttu-id="94c5c-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="94c5c-144">configurationEndpointUrl</span></span>|<span data-ttu-id="94c5c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c5c-145">String</span></span>|<span data-ttu-id="94c5c-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="94c5c-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="94c5c-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-148">Boolean</span></span>|<span data-ttu-id="94c5c-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="94c5c-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="94c5c-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="94c5c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="94c5c-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-152">Boolean</span></span>|<span data-ttu-id="94c5c-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="94c5c-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="94c5c-154">isDefault</span></span>|<span data-ttu-id="94c5c-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-155">Boolean</span></span>|<span data-ttu-id="94c5c-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-157">supervisedModeEnabled</span></span>|<span data-ttu-id="94c5c-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-158">Boolean</span></span>|<span data-ttu-id="94c5c-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="94c5c-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="94c5c-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="94c5c-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="94c5c-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="94c5c-162">supportDepartment</span></span>|<span data-ttu-id="94c5c-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c5c-163">String</span></span>|<span data-ttu-id="94c5c-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-165">passCodeDisabled</span></span>|<span data-ttu-id="94c5c-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-166">Boolean</span></span>|<span data-ttu-id="94c5c-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="94c5c-168">isMandatory</span></span>|<span data-ttu-id="94c5c-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-169">Boolean</span></span>|<span data-ttu-id="94c5c-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-171">locationDisabled</span></span>|<span data-ttu-id="94c5c-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-172">Boolean</span></span>|<span data-ttu-id="94c5c-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="94c5c-174">supportPhoneNumber</span></span>|<span data-ttu-id="94c5c-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c5c-175">String</span></span>|<span data-ttu-id="94c5c-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-177">profileRemovalDisabled</span></span>|<span data-ttu-id="94c5c-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-178">Boolean</span></span>|<span data-ttu-id="94c5c-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="94c5c-180">restoreBlocked</span></span>|<span data-ttu-id="94c5c-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-181">Boolean</span></span>|<span data-ttu-id="94c5c-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-183">appleIdDisabled</span></span>|<span data-ttu-id="94c5c-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-184">Boolean</span></span>|<span data-ttu-id="94c5c-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="94c5c-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-187">Boolean</span></span>|<span data-ttu-id="94c5c-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-189">touchIdDisabled</span></span>|<span data-ttu-id="94c5c-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-190">Boolean</span></span>|<span data-ttu-id="94c5c-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-192">applePayDisabled</span></span>|<span data-ttu-id="94c5c-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-193">Boolean</span></span>|<span data-ttu-id="94c5c-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-195">zoomDisabled</span></span>|<span data-ttu-id="94c5c-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-196">Boolean</span></span>|<span data-ttu-id="94c5c-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-198">siriDisabled</span></span>|<span data-ttu-id="94c5c-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-199">Boolean</span></span>|<span data-ttu-id="94c5c-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-201">diagnosticsDisabled</span></span>|<span data-ttu-id="94c5c-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-202">Boolean</span></span>|<span data-ttu-id="94c5c-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="94c5c-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-205">Boolean</span></span>|<span data-ttu-id="94c5c-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-207">privacyPaneDisabled</span></span>|<span data-ttu-id="94c5c-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-208">Boolean</span></span>|<span data-ttu-id="94c5c-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-210">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="94c5c-210">deviceNameTemplate</span></span>|<span data-ttu-id="94c5c-211">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c5c-211">String</span></span>|<span data-ttu-id="94c5c-212">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="94c5c-212">Sets a literal or name pattern.</span></span> <span data-ttu-id="94c5c-213">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-213">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="94c5c-214">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="94c5c-214">iTunesPairingMode</span></span>|[<span data-ttu-id="94c5c-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="94c5c-215">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="94c5c-216">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="94c5c-216">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="94c5c-217">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="94c5c-217">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="94c5c-218">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="94c5c-218">managementCertificates</span></span>|<span data-ttu-id="94c5c-219">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="94c5c-219">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="94c5c-220">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="94c5c-220">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="94c5c-221">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-221">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="94c5c-222">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-222">Boolean</span></span>|<span data-ttu-id="94c5c-223">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-223">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="94c5c-224">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="94c5c-224">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="94c5c-225">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-225">Boolean</span></span>|<span data-ttu-id="94c5c-226">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="94c5c-226">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="94c5c-227">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="94c5c-227">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="94c5c-228">Int32</span><span class="sxs-lookup"><span data-stu-id="94c5c-228">Int32</span></span>|<span data-ttu-id="94c5c-229">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94c5c-229">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="94c5c-230">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94c5c-230">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="94c5c-231">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="94c5c-231">enableSharedIPad</span></span>|<span data-ttu-id="94c5c-232">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-232">Boolean</span></span>|<span data-ttu-id="94c5c-233">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="94c5c-233">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="94c5c-234">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="94c5c-234">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="94c5c-235">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="94c5c-235">companyPortalVppTokenId</span></span>|<span data-ttu-id="94c5c-236">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="94c5c-236">String</span></span>|<span data-ttu-id="94c5c-237">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="94c5c-237">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="94c5c-238">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="94c5c-238">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="94c5c-239">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="94c5c-239">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="94c5c-240">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-240">Boolean</span></span>|<span data-ttu-id="94c5c-241">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="94c5c-241">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="94c5c-242">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="94c5c-242">Default is false.</span></span> <span data-ttu-id="94c5c-243">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="94c5c-243">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="94c5c-244">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-244">homeButtonScreenDisabled</span></span>|<span data-ttu-id="94c5c-245">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-245">Boolean</span></span>|<span data-ttu-id="94c5c-246">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-246">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="94c5c-247">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-247">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="94c5c-248">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-248">Boolean</span></span>|<span data-ttu-id="94c5c-249">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-249">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="94c5c-250">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-250">onBoardingScreenDisabled</span></span>|<span data-ttu-id="94c5c-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-251">Boolean</span></span>|<span data-ttu-id="94c5c-252">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-252">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="94c5c-253">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-253">screenTimeScreenDisabled</span></span>|<span data-ttu-id="94c5c-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-254">Boolean</span></span>|<span data-ttu-id="94c5c-255">Indica se a configuração de tempo limite da tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-255">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="94c5c-256">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-256">simSetupScreenDisabled</span></span>|<span data-ttu-id="94c5c-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-257">Boolean</span></span>|<span data-ttu-id="94c5c-258">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-258">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="94c5c-259">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-259">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="94c5c-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-260">Boolean</span></span>|<span data-ttu-id="94c5c-261">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-261">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="94c5c-262">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="94c5c-262">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="94c5c-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="94c5c-263">Boolean</span></span>|<span data-ttu-id="94c5c-264">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="94c5c-264">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="94c5c-265">Resposta</span><span class="sxs-lookup"><span data-stu-id="94c5c-265">Response</span></span>
<span data-ttu-id="94c5c-266">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="94c5c-266">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="94c5c-267">Exemplo</span><span class="sxs-lookup"><span data-stu-id="94c5c-267">Example</span></span>

### <a name="request"></a><span data-ttu-id="94c5c-268">Solicitação</span><span class="sxs-lookup"><span data-stu-id="94c5c-268">Request</span></span>
<span data-ttu-id="94c5c-269">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="94c5c-269">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 1791

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
  "deviceNameTemplate": "Device Name Template value",
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

### <a name="response"></a><span data-ttu-id="94c5c-270">Resposta</span><span class="sxs-lookup"><span data-stu-id="94c5c-270">Response</span></span>
<span data-ttu-id="94c5c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="94c5c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1840

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
  "deviceNameTemplate": "Device Name Template value",
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




