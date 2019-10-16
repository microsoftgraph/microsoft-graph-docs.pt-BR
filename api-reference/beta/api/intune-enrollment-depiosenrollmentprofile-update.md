---
title: Atualizar depIOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 74e0808201609693bfc9c3949487d5691a9cb620
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37536045"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="d9a0c-103">Atualizar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d9a0c-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="d9a0c-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d9a0c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d9a0c-106">Atualiza as propriedades de um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d9a0c-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d9a0c-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d9a0c-107">Prerequisites</span></span>
<span data-ttu-id="d9a0c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d9a0c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9a0c-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d9a0c-110">Permission type</span></span>|<span data-ttu-id="d9a0c-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9a0c-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d9a0c-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a0c-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d9a0c-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9a0c-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-115">Not supported.</span></span>|
|<span data-ttu-id="d9a0c-116">Application</span><span class="sxs-lookup"><span data-stu-id="d9a0c-116">Application</span></span>|<span data-ttu-id="d9a0c-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9a0c-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9a0c-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d9a0c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d9a0c-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a0c-119">Request headers</span></span>
|<span data-ttu-id="d9a0c-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d9a0c-120">Header</span></span>|<span data-ttu-id="d9a0c-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d9a0c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9a0c-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d9a0c-122">Authorization</span></span>|<span data-ttu-id="d9a0c-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9a0c-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d9a0c-124">Accept</span></span>|<span data-ttu-id="d9a0c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d9a0c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9a0c-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a0c-126">Request body</span></span>
<span data-ttu-id="d9a0c-127">No corpo da solicitação, forneça uma representação JSON do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d9a0c-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d9a0c-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d9a0c-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="d9a0c-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d9a0c-129">Property</span></span>|<span data-ttu-id="d9a0c-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d9a0c-130">Type</span></span>|<span data-ttu-id="d9a0c-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d9a0c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a0c-132">id</span><span class="sxs-lookup"><span data-stu-id="d9a0c-132">id</span></span>|<span data-ttu-id="d9a0c-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9a0c-133">String</span></span>|<span data-ttu-id="d9a0c-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d9a0c-135">displayName</span></span>|<span data-ttu-id="d9a0c-136">String</span><span class="sxs-lookup"><span data-stu-id="d9a0c-136">String</span></span>|<span data-ttu-id="d9a0c-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-138">description</span><span class="sxs-lookup"><span data-stu-id="d9a0c-138">description</span></span>|<span data-ttu-id="d9a0c-139">String</span><span class="sxs-lookup"><span data-stu-id="d9a0c-139">String</span></span>|<span data-ttu-id="d9a0c-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d9a0c-141">requiresUserAuthentication</span></span>|<span data-ttu-id="d9a0c-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-142">Boolean</span></span>|<span data-ttu-id="d9a0c-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d9a0c-144">configurationEndpointUrl</span></span>|<span data-ttu-id="d9a0c-145">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9a0c-145">String</span></span>|<span data-ttu-id="d9a0c-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d9a0c-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-148">Boolean</span></span>|<span data-ttu-id="d9a0c-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d9a0c-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d9a0c-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d9a0c-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-152">Boolean</span></span>|<span data-ttu-id="d9a0c-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="d9a0c-154">isDefault</span></span>|<span data-ttu-id="d9a0c-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-155">Boolean</span></span>|<span data-ttu-id="d9a0c-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-157">supervisedModeEnabled</span></span>|<span data-ttu-id="d9a0c-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-158">Boolean</span></span>|<span data-ttu-id="d9a0c-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d9a0c-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="d9a0c-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="d9a0c-162">supportDepartment</span></span>|<span data-ttu-id="d9a0c-163">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9a0c-163">String</span></span>|<span data-ttu-id="d9a0c-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-165">passCodeDisabled</span></span>|<span data-ttu-id="d9a0c-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-166">Boolean</span></span>|<span data-ttu-id="d9a0c-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="d9a0c-168">isMandatory</span></span>|<span data-ttu-id="d9a0c-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-169">Boolean</span></span>|<span data-ttu-id="d9a0c-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-171">locationDisabled</span></span>|<span data-ttu-id="d9a0c-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-172">Boolean</span></span>|<span data-ttu-id="d9a0c-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d9a0c-174">supportPhoneNumber</span></span>|<span data-ttu-id="d9a0c-175">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9a0c-175">String</span></span>|<span data-ttu-id="d9a0c-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-177">profileRemovalDisabled</span></span>|<span data-ttu-id="d9a0c-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-178">Boolean</span></span>|<span data-ttu-id="d9a0c-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d9a0c-180">restoreBlocked</span></span>|<span data-ttu-id="d9a0c-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-181">Boolean</span></span>|<span data-ttu-id="d9a0c-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-183">appleIdDisabled</span></span>|<span data-ttu-id="d9a0c-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-184">Boolean</span></span>|<span data-ttu-id="d9a0c-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d9a0c-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-187">Boolean</span></span>|<span data-ttu-id="d9a0c-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-189">touchIdDisabled</span></span>|<span data-ttu-id="d9a0c-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-190">Boolean</span></span>|<span data-ttu-id="d9a0c-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-192">applePayDisabled</span></span>|<span data-ttu-id="d9a0c-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-193">Boolean</span></span>|<span data-ttu-id="d9a0c-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-195">zoomDisabled</span></span>|<span data-ttu-id="d9a0c-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-196">Boolean</span></span>|<span data-ttu-id="d9a0c-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-198">siriDisabled</span></span>|<span data-ttu-id="d9a0c-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-199">Boolean</span></span>|<span data-ttu-id="d9a0c-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-201">diagnosticsDisabled</span></span>|<span data-ttu-id="d9a0c-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-202">Boolean</span></span>|<span data-ttu-id="d9a0c-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="d9a0c-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-205">Boolean</span></span>|<span data-ttu-id="d9a0c-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-207">privacyPaneDisabled</span></span>|<span data-ttu-id="d9a0c-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-208">Boolean</span></span>|<span data-ttu-id="d9a0c-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-210">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="d9a0c-211">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-211">Boolean</span></span>|<span data-ttu-id="d9a0c-212">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-213">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="d9a0c-213">deviceNameTemplate</span></span>|<span data-ttu-id="d9a0c-214">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9a0c-214">String</span></span>|<span data-ttu-id="d9a0c-215">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="d9a0c-216">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-217">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="d9a0c-217">configurationWebUrl</span></span>|<span data-ttu-id="d9a0c-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-218">Boolean</span></span>|<span data-ttu-id="d9a0c-219">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d9a0c-220">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d9a0c-220">iTunesPairingMode</span></span>|[<span data-ttu-id="d9a0c-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="d9a0c-221">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="d9a0c-222">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-222">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="d9a0c-223">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-223">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="d9a0c-224">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="d9a0c-224">managementCertificates</span></span>|<span data-ttu-id="d9a0c-225">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="d9a0c-225">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="d9a0c-226">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="d9a0c-226">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="d9a0c-227">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-227">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="d9a0c-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-228">Boolean</span></span>|<span data-ttu-id="d9a0c-229">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-229">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="d9a0c-230">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="d9a0c-230">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="d9a0c-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-231">Boolean</span></span>|<span data-ttu-id="d9a0c-232">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-232">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="d9a0c-233">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="d9a0c-233">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="d9a0c-234">Int32</span><span class="sxs-lookup"><span data-stu-id="d9a0c-234">Int32</span></span>|<span data-ttu-id="d9a0c-235">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-235">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="d9a0c-236">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-236">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="d9a0c-237">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="d9a0c-237">enableSharedIPad</span></span>|<span data-ttu-id="d9a0c-238">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-238">Boolean</span></span>|<span data-ttu-id="d9a0c-239">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-239">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="d9a0c-240">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-240">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="d9a0c-241">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="d9a0c-241">companyPortalVppTokenId</span></span>|<span data-ttu-id="d9a0c-242">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d9a0c-242">String</span></span>|<span data-ttu-id="d9a0c-243">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-243">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="d9a0c-244">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-244">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="d9a0c-245">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="d9a0c-245">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="d9a0c-246">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-246">Boolean</span></span>|<span data-ttu-id="d9a0c-247">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-247">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="d9a0c-248">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-248">Default is false.</span></span> <span data-ttu-id="d9a0c-249">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-249">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="d9a0c-250">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-250">homeButtonScreenDisabled</span></span>|<span data-ttu-id="d9a0c-251">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-251">Boolean</span></span>|<span data-ttu-id="d9a0c-252">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-252">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-253">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-253">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="d9a0c-254">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-254">Boolean</span></span>|<span data-ttu-id="d9a0c-255">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-255">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-256">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-256">onBoardingScreenDisabled</span></span>|<span data-ttu-id="d9a0c-257">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-257">Boolean</span></span>|<span data-ttu-id="d9a0c-258">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-258">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-259">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-259">simSetupScreenDisabled</span></span>|<span data-ttu-id="d9a0c-260">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-260">Boolean</span></span>|<span data-ttu-id="d9a0c-261">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-261">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-262">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-262">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="d9a0c-263">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-263">Boolean</span></span>|<span data-ttu-id="d9a0c-264">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-264">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-265">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-265">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="d9a0c-266">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-266">Boolean</span></span>|<span data-ttu-id="d9a0c-267">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-267">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-268">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-268">appearanceScreenDisabled</span></span>|<span data-ttu-id="d9a0c-269">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-269">Boolean</span></span>|<span data-ttu-id="d9a0c-270">Indica se a tela do apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-270">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-271">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-271">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="d9a0c-272">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-272">Boolean</span></span>|<span data-ttu-id="d9a0c-273">Indica se a tela de idioma expresso está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-273">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-274">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-274">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="d9a0c-275">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-275">Boolean</span></span>|<span data-ttu-id="d9a0c-276">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-276">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="d9a0c-277">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-277">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="d9a0c-278">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-278">Boolean</span></span>|<span data-ttu-id="d9a0c-279">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-279">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="d9a0c-280">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d9a0c-280">welcomeScreenDisabled</span></span>|<span data-ttu-id="d9a0c-281">Booliano</span><span class="sxs-lookup"><span data-stu-id="d9a0c-281">Boolean</span></span>|<span data-ttu-id="d9a0c-282">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d9a0c-282">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="d9a0c-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a0c-283">Response</span></span>
<span data-ttu-id="d9a0c-284">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-284">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9a0c-285">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d9a0c-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="d9a0c-286">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d9a0c-286">Request</span></span>
<span data-ttu-id="d9a0c-287">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-287">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9a0c-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="d9a0c-288">Response</span></span>
<span data-ttu-id="d9a0c-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d9a0c-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






