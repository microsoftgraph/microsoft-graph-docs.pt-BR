---
title: Atualizar depIOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ef081e9902e1a258cd65f27a4f1ff23aeffefa8d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49201944"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="90dd4-103">Atualizar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="90dd4-103">Update depIOSEnrollmentProfile</span></span>

<span data-ttu-id="90dd4-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90dd4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90dd4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="90dd4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90dd4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="90dd4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90dd4-107">Atualiza as propriedades de um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="90dd4-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90dd4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="90dd4-108">Prerequisites</span></span>
<span data-ttu-id="90dd4-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="90dd4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90dd4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="90dd4-111">Permission type</span></span>|<span data-ttu-id="90dd4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="90dd4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90dd4-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="90dd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="90dd4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90dd4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="90dd4-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="90dd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90dd4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="90dd4-116">Not supported.</span></span>|
|<span data-ttu-id="90dd4-117">Application</span><span class="sxs-lookup"><span data-stu-id="90dd4-117">Application</span></span>|<span data-ttu-id="90dd4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="90dd4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="90dd4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="90dd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="90dd4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="90dd4-120">Request headers</span></span>
|<span data-ttu-id="90dd4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="90dd4-121">Header</span></span>|<span data-ttu-id="90dd4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="90dd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90dd4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="90dd4-123">Authorization</span></span>|<span data-ttu-id="90dd4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="90dd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90dd4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="90dd4-125">Accept</span></span>|<span data-ttu-id="90dd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90dd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90dd4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="90dd4-127">Request body</span></span>
<span data-ttu-id="90dd4-128">No corpo da solicitação, forneça uma representação JSON do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="90dd4-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="90dd4-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="90dd4-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="90dd4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="90dd4-130">Property</span></span>|<span data-ttu-id="90dd4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="90dd4-131">Type</span></span>|<span data-ttu-id="90dd4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="90dd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90dd4-133">id</span><span class="sxs-lookup"><span data-stu-id="90dd4-133">id</span></span>|<span data-ttu-id="90dd4-134">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-134">String</span></span>|<span data-ttu-id="90dd4-135">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="90dd4-136">displayName</span></span>|<span data-ttu-id="90dd4-137">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-137">String</span></span>|<span data-ttu-id="90dd4-138">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-139">description</span><span class="sxs-lookup"><span data-stu-id="90dd4-139">description</span></span>|<span data-ttu-id="90dd4-140">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-140">String</span></span>|<span data-ttu-id="90dd4-141">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="90dd4-142">requiresUserAuthentication</span></span>|<span data-ttu-id="90dd4-143">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-143">Boolean</span></span>|<span data-ttu-id="90dd4-144">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="90dd4-145">configurationEndpointUrl</span></span>|<span data-ttu-id="90dd4-146">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-146">String</span></span>|<span data-ttu-id="90dd4-147">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-148">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="90dd4-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="90dd4-149">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-149">Boolean</span></span>|<span data-ttu-id="90dd4-150">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="90dd4-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="90dd4-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="90dd4-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="90dd4-153">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-153">Boolean</span></span>|<span data-ttu-id="90dd4-154">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="90dd4-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="90dd4-155">isDefault</span></span>|<span data-ttu-id="90dd4-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-156">Boolean</span></span>|<span data-ttu-id="90dd4-157">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-158">supervisedModeEnabled</span></span>|<span data-ttu-id="90dd4-159">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-159">Boolean</span></span>|<span data-ttu-id="90dd4-160">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="90dd4-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="90dd4-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="90dd4-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="90dd4-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="90dd4-163">supportDepartment</span></span>|<span data-ttu-id="90dd4-164">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-164">String</span></span>|<span data-ttu-id="90dd4-165">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-166">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="90dd4-166">isMandatory</span></span>|<span data-ttu-id="90dd4-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-167">Boolean</span></span>|<span data-ttu-id="90dd4-168">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-169">locationDisabled</span></span>|<span data-ttu-id="90dd4-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-170">Boolean</span></span>|<span data-ttu-id="90dd4-171">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="90dd4-172">supportPhoneNumber</span></span>|<span data-ttu-id="90dd4-173">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-173">String</span></span>|<span data-ttu-id="90dd4-174">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-175">profileRemovalDisabled</span></span>|<span data-ttu-id="90dd4-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-176">Boolean</span></span>|<span data-ttu-id="90dd4-177">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="90dd4-178">restoreBlocked</span></span>|<span data-ttu-id="90dd4-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-179">Boolean</span></span>|<span data-ttu-id="90dd4-180">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-181">appleIdDisabled</span></span>|<span data-ttu-id="90dd4-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-182">Boolean</span></span>|<span data-ttu-id="90dd4-183">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="90dd4-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-185">Boolean</span></span>|<span data-ttu-id="90dd4-186">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-187">touchIdDisabled</span></span>|<span data-ttu-id="90dd4-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-188">Boolean</span></span>|<span data-ttu-id="90dd4-189">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-190">applePayDisabled</span></span>|<span data-ttu-id="90dd4-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-191">Boolean</span></span>|<span data-ttu-id="90dd4-192">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-193">siriDisabled</span></span>|<span data-ttu-id="90dd4-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-194">Boolean</span></span>|<span data-ttu-id="90dd4-195">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-196">diagnosticsDisabled</span></span>|<span data-ttu-id="90dd4-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-197">Boolean</span></span>|<span data-ttu-id="90dd4-198">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="90dd4-200">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-200">Boolean</span></span>|<span data-ttu-id="90dd4-201">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-202">privacyPaneDisabled</span></span>|<span data-ttu-id="90dd4-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-203">Boolean</span></span>|<span data-ttu-id="90dd4-204">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="90dd4-206">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-206">Boolean</span></span>|<span data-ttu-id="90dd4-207">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="90dd4-208">deviceNameTemplate</span></span>|<span data-ttu-id="90dd4-209">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-209">String</span></span>|<span data-ttu-id="90dd4-210">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="90dd4-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="90dd4-211">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="90dd4-212">configurationWebUrl</span></span>|<span data-ttu-id="90dd4-213">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-213">Boolean</span></span>|<span data-ttu-id="90dd4-214">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="90dd4-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="90dd4-215">iTunesPairingMode</span></span>|[<span data-ttu-id="90dd4-216">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="90dd4-216">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="90dd4-217">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="90dd4-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="90dd4-218">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="90dd4-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="90dd4-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="90dd4-219">managementCertificates</span></span>|<span data-ttu-id="90dd4-220">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="90dd4-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="90dd4-221">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="90dd4-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="90dd4-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="90dd4-223">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-223">Boolean</span></span>|<span data-ttu-id="90dd4-224">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="90dd4-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="90dd4-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="90dd4-226">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-226">Boolean</span></span>|<span data-ttu-id="90dd4-227">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="90dd4-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="90dd4-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="90dd4-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="90dd4-229">Int32</span><span class="sxs-lookup"><span data-stu-id="90dd4-229">Int32</span></span>|<span data-ttu-id="90dd4-230">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="90dd4-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="90dd4-231">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="90dd4-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="90dd4-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="90dd4-232">enableSharedIPad</span></span>|<span data-ttu-id="90dd4-233">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-233">Boolean</span></span>|<span data-ttu-id="90dd4-234">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="90dd4-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="90dd4-235">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="90dd4-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="90dd4-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="90dd4-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="90dd4-237">String</span><span class="sxs-lookup"><span data-stu-id="90dd4-237">String</span></span>|<span data-ttu-id="90dd4-238">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="90dd4-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="90dd4-239">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="90dd4-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="90dd4-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="90dd4-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="90dd4-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-241">Boolean</span></span>|<span data-ttu-id="90dd4-242">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="90dd4-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="90dd4-243">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="90dd4-243">Default is false.</span></span> <span data-ttu-id="90dd4-244">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="90dd4-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="90dd4-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="90dd4-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-246">Boolean</span></span>|<span data-ttu-id="90dd4-247">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="90dd4-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="90dd4-249">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-249">Boolean</span></span>|<span data-ttu-id="90dd4-250">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="90dd4-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="90dd4-252">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-252">Boolean</span></span>|<span data-ttu-id="90dd4-253">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="90dd4-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="90dd4-255">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-255">Boolean</span></span>|<span data-ttu-id="90dd4-256">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="90dd4-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="90dd4-258">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-258">Boolean</span></span>|<span data-ttu-id="90dd4-259">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="90dd4-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="90dd4-261">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-261">Boolean</span></span>|<span data-ttu-id="90dd4-262">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="90dd4-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="90dd4-264">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-264">Boolean</span></span>|<span data-ttu-id="90dd4-265">Indica se a tela do apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="90dd4-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="90dd4-267">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-267">Boolean</span></span>|<span data-ttu-id="90dd4-268">Indica se a tela de idioma expresso está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="90dd4-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="90dd4-270">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-270">Boolean</span></span>|<span data-ttu-id="90dd4-271">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="90dd4-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="90dd4-273">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-273">Boolean</span></span>|<span data-ttu-id="90dd4-274">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="90dd4-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="90dd4-276">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-276">Boolean</span></span>|<span data-ttu-id="90dd4-277">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="90dd4-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-278">passCodeDisabled</span></span>|<span data-ttu-id="90dd4-279">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-279">Boolean</span></span>|<span data-ttu-id="90dd4-280">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="90dd4-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="90dd4-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-281">zoomDisabled</span></span>|<span data-ttu-id="90dd4-282">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-282">Boolean</span></span>|<span data-ttu-id="90dd4-283">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="90dd4-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="90dd4-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="90dd4-285">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-285">Boolean</span></span>|<span data-ttu-id="90dd4-286">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="90dd4-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="90dd4-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="90dd4-288">Booliano</span><span class="sxs-lookup"><span data-stu-id="90dd4-288">Boolean</span></span>|<span data-ttu-id="90dd4-289">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="90dd4-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="90dd4-290">Resposta</span><span class="sxs-lookup"><span data-stu-id="90dd4-290">Response</span></span>
<span data-ttu-id="90dd4-291">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="90dd4-291">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90dd4-292">Exemplo</span><span class="sxs-lookup"><span data-stu-id="90dd4-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="90dd4-293">Solicitação</span><span class="sxs-lookup"><span data-stu-id="90dd4-293">Request</span></span>
<span data-ttu-id="90dd4-294">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="90dd4-294">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
Content-type: application/json
Content-length: 2108

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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
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
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="90dd4-295">Resposta</span><span class="sxs-lookup"><span data-stu-id="90dd4-295">Response</span></span>
<span data-ttu-id="90dd4-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="90dd4-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2157

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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "Support Phone Number value",
  "profileRemovalDisabled": true,
  "restoreBlocked": true,
  "appleIdDisabled": true,
  "termsAndConditionsDisabled": true,
  "touchIdDisabled": true,
  "applePayDisabled": true,
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
  "welcomeScreenDisabled": true,
  "passCodeDisabled": true,
  "zoomDisabled": true,
  "restoreCompletedScreenDisabled": true,
  "updateCompleteScreenDisabled": true
}
```




