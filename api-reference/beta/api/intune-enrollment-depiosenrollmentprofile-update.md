---
title: Atualizar depIOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 14526428268dda5ee4d273c0a03e01318410e13f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093872"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="55f40-103">Atualizar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="55f40-103">Update depIOSEnrollmentProfile</span></span>

<span data-ttu-id="55f40-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55f40-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55f40-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="55f40-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55f40-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="55f40-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55f40-107">Atualiza as propriedades de um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55f40-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55f40-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="55f40-108">Prerequisites</span></span>
<span data-ttu-id="55f40-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="55f40-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55f40-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="55f40-111">Permission type</span></span>|<span data-ttu-id="55f40-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="55f40-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55f40-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="55f40-113">Delegated (work or school account)</span></span>|<span data-ttu-id="55f40-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f40-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="55f40-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="55f40-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55f40-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="55f40-116">Not supported.</span></span>|
|<span data-ttu-id="55f40-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="55f40-117">Application</span></span>|<span data-ttu-id="55f40-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="55f40-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="55f40-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="55f40-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="55f40-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="55f40-120">Request headers</span></span>
|<span data-ttu-id="55f40-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="55f40-121">Header</span></span>|<span data-ttu-id="55f40-122">Valor</span><span class="sxs-lookup"><span data-stu-id="55f40-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55f40-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="55f40-123">Authorization</span></span>|<span data-ttu-id="55f40-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="55f40-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55f40-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="55f40-125">Accept</span></span>|<span data-ttu-id="55f40-126">application/json</span><span class="sxs-lookup"><span data-stu-id="55f40-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55f40-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="55f40-127">Request body</span></span>
<span data-ttu-id="55f40-128">No corpo da solicitação, forneça uma representação JSON do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="55f40-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="55f40-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="55f40-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="55f40-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55f40-130">Property</span></span>|<span data-ttu-id="55f40-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="55f40-131">Type</span></span>|<span data-ttu-id="55f40-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="55f40-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55f40-133">id</span><span class="sxs-lookup"><span data-stu-id="55f40-133">id</span></span>|<span data-ttu-id="55f40-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-134">String</span></span>|<span data-ttu-id="55f40-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-136">displayName</span><span class="sxs-lookup"><span data-stu-id="55f40-136">displayName</span></span>|<span data-ttu-id="55f40-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-137">String</span></span>|<span data-ttu-id="55f40-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-139">description</span><span class="sxs-lookup"><span data-stu-id="55f40-139">description</span></span>|<span data-ttu-id="55f40-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-140">String</span></span>|<span data-ttu-id="55f40-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="55f40-142">requiresUserAuthentication</span></span>|<span data-ttu-id="55f40-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-143">Boolean</span></span>|<span data-ttu-id="55f40-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="55f40-145">configurationEndpointUrl</span></span>|<span data-ttu-id="55f40-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-146">String</span></span>|<span data-ttu-id="55f40-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="55f40-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="55f40-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-149">Boolean</span></span>|<span data-ttu-id="55f40-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="55f40-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="55f40-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="55f40-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="55f40-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-153">Boolean</span></span>|<span data-ttu-id="55f40-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="55f40-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="55f40-155">isDefault</span></span>|<span data-ttu-id="55f40-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="55f40-156">Boolean</span></span>|<span data-ttu-id="55f40-157">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="55f40-158">supervisedModeEnabled</span></span>|<span data-ttu-id="55f40-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-159">Boolean</span></span>|<span data-ttu-id="55f40-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="55f40-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="55f40-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="55f40-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="55f40-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="55f40-163">supportDepartment</span></span>|<span data-ttu-id="55f40-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-164">String</span></span>|<span data-ttu-id="55f40-165">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-166">passCodeDisabled</span></span>|<span data-ttu-id="55f40-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-167">Boolean</span></span>|<span data-ttu-id="55f40-168">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-169">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="55f40-169">isMandatory</span></span>|<span data-ttu-id="55f40-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-170">Boolean</span></span>|<span data-ttu-id="55f40-171">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-172">locationDisabled</span></span>|<span data-ttu-id="55f40-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-173">Boolean</span></span>|<span data-ttu-id="55f40-174">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="55f40-175">supportPhoneNumber</span></span>|<span data-ttu-id="55f40-176">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-176">String</span></span>|<span data-ttu-id="55f40-177">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-178">profileRemovalDisabled</span></span>|<span data-ttu-id="55f40-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-179">Boolean</span></span>|<span data-ttu-id="55f40-180">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="55f40-181">restoreBlocked</span></span>|<span data-ttu-id="55f40-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-182">Boolean</span></span>|<span data-ttu-id="55f40-183">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-184">appleIdDisabled</span></span>|<span data-ttu-id="55f40-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-185">Boolean</span></span>|<span data-ttu-id="55f40-186">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="55f40-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-188">Boolean</span></span>|<span data-ttu-id="55f40-189">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-190">touchIdDisabled</span></span>|<span data-ttu-id="55f40-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-191">Boolean</span></span>|<span data-ttu-id="55f40-192">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-193">applePayDisabled</span></span>|<span data-ttu-id="55f40-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-194">Boolean</span></span>|<span data-ttu-id="55f40-195">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-196">zoomDisabled</span></span>|<span data-ttu-id="55f40-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-197">Boolean</span></span>|<span data-ttu-id="55f40-198">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-199">siriDisabled</span></span>|<span data-ttu-id="55f40-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-200">Boolean</span></span>|<span data-ttu-id="55f40-201">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-202">diagnosticsDisabled</span></span>|<span data-ttu-id="55f40-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-203">Boolean</span></span>|<span data-ttu-id="55f40-204">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="55f40-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-206">Boolean</span></span>|<span data-ttu-id="55f40-207">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-208">privacyPaneDisabled</span></span>|<span data-ttu-id="55f40-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-209">Boolean</span></span>|<span data-ttu-id="55f40-210">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-211">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-211">screenTimeScreenDisabled</span></span>|<span data-ttu-id="55f40-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-212">Boolean</span></span>|<span data-ttu-id="55f40-213">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-213">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-214">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="55f40-214">deviceNameTemplate</span></span>|<span data-ttu-id="55f40-215">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-215">String</span></span>|<span data-ttu-id="55f40-216">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="55f40-216">Sets a literal or name pattern.</span></span> <span data-ttu-id="55f40-217">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-217">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-218">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="55f40-218">configurationWebUrl</span></span>|<span data-ttu-id="55f40-219">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-219">Boolean</span></span>|<span data-ttu-id="55f40-220">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-220">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="55f40-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="55f40-221">iTunesPairingMode</span></span>|[<span data-ttu-id="55f40-222">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="55f40-222">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="55f40-223">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="55f40-223">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="55f40-224">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="55f40-224">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="55f40-225">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="55f40-225">managementCertificates</span></span>|<span data-ttu-id="55f40-226">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="55f40-226">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="55f40-227">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="55f40-227">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="55f40-228">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-228">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="55f40-229">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-229">Boolean</span></span>|<span data-ttu-id="55f40-230">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-230">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="55f40-231">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="55f40-231">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="55f40-232">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-232">Boolean</span></span>|<span data-ttu-id="55f40-233">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="55f40-233">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="55f40-234">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="55f40-234">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="55f40-235">Int32</span><span class="sxs-lookup"><span data-stu-id="55f40-235">Int32</span></span>|<span data-ttu-id="55f40-236">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="55f40-236">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="55f40-237">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="55f40-237">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="55f40-238">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="55f40-238">enableSharedIPad</span></span>|<span data-ttu-id="55f40-239">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-239">Boolean</span></span>|<span data-ttu-id="55f40-240">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="55f40-240">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="55f40-241">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="55f40-241">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="55f40-242">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="55f40-242">companyPortalVppTokenId</span></span>|<span data-ttu-id="55f40-243">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55f40-243">String</span></span>|<span data-ttu-id="55f40-244">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="55f40-244">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="55f40-245">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="55f40-245">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="55f40-246">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="55f40-246">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="55f40-247">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-247">Boolean</span></span>|<span data-ttu-id="55f40-248">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="55f40-248">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="55f40-249">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="55f40-249">Default is false.</span></span> <span data-ttu-id="55f40-250">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="55f40-250">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="55f40-251">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-251">homeButtonScreenDisabled</span></span>|<span data-ttu-id="55f40-252">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-252">Boolean</span></span>|<span data-ttu-id="55f40-253">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-253">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="55f40-254">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-254">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="55f40-255">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-255">Boolean</span></span>|<span data-ttu-id="55f40-256">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-256">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="55f40-257">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-257">onBoardingScreenDisabled</span></span>|<span data-ttu-id="55f40-258">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-258">Boolean</span></span>|<span data-ttu-id="55f40-259">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-259">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="55f40-260">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-260">simSetupScreenDisabled</span></span>|<span data-ttu-id="55f40-261">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-261">Boolean</span></span>|<span data-ttu-id="55f40-262">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-262">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="55f40-263">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-263">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="55f40-264">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-264">Boolean</span></span>|<span data-ttu-id="55f40-265">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-265">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="55f40-266">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-266">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="55f40-267">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-267">Boolean</span></span>|<span data-ttu-id="55f40-268">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-268">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="55f40-269">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-269">appearanceScreenDisabled</span></span>|<span data-ttu-id="55f40-270">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-270">Boolean</span></span>|<span data-ttu-id="55f40-271">Indica se a tela do apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-271">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="55f40-272">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-272">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="55f40-273">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-273">Boolean</span></span>|<span data-ttu-id="55f40-274">Indica se a tela de idioma expresso está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-274">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="55f40-275">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-275">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="55f40-276">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-276">Boolean</span></span>|<span data-ttu-id="55f40-277">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-277">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="55f40-278">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-278">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="55f40-279">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-279">Boolean</span></span>|<span data-ttu-id="55f40-280">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-280">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="55f40-281">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="55f40-281">welcomeScreenDisabled</span></span>|<span data-ttu-id="55f40-282">Boolean</span><span class="sxs-lookup"><span data-stu-id="55f40-282">Boolean</span></span>|<span data-ttu-id="55f40-283">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="55f40-283">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="55f40-284">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f40-284">Response</span></span>
<span data-ttu-id="55f40-285">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="55f40-285">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55f40-286">Exemplo</span><span class="sxs-lookup"><span data-stu-id="55f40-286">Example</span></span>

### <a name="request"></a><span data-ttu-id="55f40-287">Solicitação</span><span class="sxs-lookup"><span data-stu-id="55f40-287">Request</span></span>
<span data-ttu-id="55f40-288">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="55f40-288">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 2024

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
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
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="55f40-289">Resposta</span><span class="sxs-lookup"><span data-stu-id="55f40-289">Response</span></span>
<span data-ttu-id="55f40-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="55f40-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2073

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
  "screenTimeScreenDisabled": true,
  "deviceNameTemplate": "Device Name Template value",
  "configurationWebUrl": true,
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
  "simSetupScreenDisabled": true,
  "softwareUpdateScreenDisabled": true,
  "watchMigrationScreenDisabled": true,
  "appearanceScreenDisabled": true,
  "expressLanguageScreenDisabled": true,
  "preferredLanguageScreenDisabled": true,
  "deviceToDeviceMigrationDisabled": true,
  "welcomeScreenDisabled": true
}
```






