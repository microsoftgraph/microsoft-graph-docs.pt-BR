---
title: Criar depIOSEnrollmentProfile
description: Criar um novo objeto depIOSEnrollmentProfile.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 45086b13a885183d9e4ecd214a009d0d2f9baba0
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943996"
---
# <a name="create-depiosenrollmentprofile"></a><span data-ttu-id="1d4e2-103">Criar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="1d4e2-103">Create depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="1d4e2-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1d4e2-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1d4e2-106">Criar um novo objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="1d4e2-106">Create a new [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1d4e2-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1d4e2-107">Prerequisites</span></span>
<span data-ttu-id="1d4e2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1d4e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1d4e2-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1d4e2-110">Permission type</span></span>|<span data-ttu-id="1d4e2-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1d4e2-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1d4e2-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4e2-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="1d4e2-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1d4e2-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-115">Not supported.</span></span>|
|<span data-ttu-id="1d4e2-116">Application</span><span class="sxs-lookup"><span data-stu-id="1d4e2-116">Application</span></span>|<span data-ttu-id="1d4e2-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1d4e2-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1d4e2-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1d4e2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="1d4e2-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4e2-119">Request headers</span></span>
|<span data-ttu-id="1d4e2-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1d4e2-120">Header</span></span>|<span data-ttu-id="1d4e2-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1d4e2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1d4e2-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1d4e2-122">Authorization</span></span>|<span data-ttu-id="1d4e2-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1d4e2-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1d4e2-124">Accept</span></span>|<span data-ttu-id="1d4e2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1d4e2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1d4e2-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4e2-126">Request body</span></span>
<span data-ttu-id="1d4e2-127">No corpo da solicitação, forneça uma representação JSON do objeto depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-127">In the request body, supply a JSON representation for the depIOSEnrollmentProfile object.</span></span>

<span data-ttu-id="1d4e2-128">A tabela a seguir mostra as propriedades que são necessárias ao criar depIOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-128">The following table shows the properties that are required when you create the depIOSEnrollmentProfile.</span></span>

|<span data-ttu-id="1d4e2-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1d4e2-129">Property</span></span>|<span data-ttu-id="1d4e2-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1d4e2-130">Type</span></span>|<span data-ttu-id="1d4e2-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1d4e2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1d4e2-132">id</span><span class="sxs-lookup"><span data-stu-id="1d4e2-132">id</span></span>|<span data-ttu-id="1d4e2-133">String</span><span class="sxs-lookup"><span data-stu-id="1d4e2-133">String</span></span>|<span data-ttu-id="1d4e2-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1d4e2-135">displayName</span></span>|<span data-ttu-id="1d4e2-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4e2-136">String</span></span>|<span data-ttu-id="1d4e2-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-138">description</span><span class="sxs-lookup"><span data-stu-id="1d4e2-138">description</span></span>|<span data-ttu-id="1d4e2-139">String</span><span class="sxs-lookup"><span data-stu-id="1d4e2-139">String</span></span>|<span data-ttu-id="1d4e2-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="1d4e2-141">requiresUserAuthentication</span></span>|<span data-ttu-id="1d4e2-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-142">Boolean</span></span>|<span data-ttu-id="1d4e2-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="1d4e2-144">configurationEndpointUrl</span></span>|<span data-ttu-id="1d4e2-145">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4e2-145">String</span></span>|<span data-ttu-id="1d4e2-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="1d4e2-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-148">Boolean</span></span>|<span data-ttu-id="1d4e2-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="1d4e2-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="1d4e2-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="1d4e2-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-152">Boolean</span></span>|<span data-ttu-id="1d4e2-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="1d4e2-154">isDefault</span></span>|<span data-ttu-id="1d4e2-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="1d4e2-155">Boolean</span></span>|<span data-ttu-id="1d4e2-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-157">supervisedModeEnabled</span></span>|<span data-ttu-id="1d4e2-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-158">Boolean</span></span>|<span data-ttu-id="1d4e2-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="1d4e2-160">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-160">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="1d4e2-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="1d4e2-162">supportDepartment</span></span>|<span data-ttu-id="1d4e2-163">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4e2-163">String</span></span>|<span data-ttu-id="1d4e2-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-165">passCodeDisabled</span></span>|<span data-ttu-id="1d4e2-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-166">Boolean</span></span>|<span data-ttu-id="1d4e2-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-168">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="1d4e2-168">isMandatory</span></span>|<span data-ttu-id="1d4e2-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-169">Boolean</span></span>|<span data-ttu-id="1d4e2-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-171">locationDisabled</span></span>|<span data-ttu-id="1d4e2-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-172">Boolean</span></span>|<span data-ttu-id="1d4e2-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="1d4e2-174">supportPhoneNumber</span></span>|<span data-ttu-id="1d4e2-175">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4e2-175">String</span></span>|<span data-ttu-id="1d4e2-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-177">profileRemovalDisabled</span></span>|<span data-ttu-id="1d4e2-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-178">Boolean</span></span>|<span data-ttu-id="1d4e2-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="1d4e2-180">restoreBlocked</span></span>|<span data-ttu-id="1d4e2-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-181">Boolean</span></span>|<span data-ttu-id="1d4e2-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-183">appleIdDisabled</span></span>|<span data-ttu-id="1d4e2-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-184">Boolean</span></span>|<span data-ttu-id="1d4e2-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="1d4e2-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-187">Boolean</span></span>|<span data-ttu-id="1d4e2-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-189">touchIdDisabled</span></span>|<span data-ttu-id="1d4e2-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-190">Boolean</span></span>|<span data-ttu-id="1d4e2-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-192">applePayDisabled</span></span>|<span data-ttu-id="1d4e2-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-193">Boolean</span></span>|<span data-ttu-id="1d4e2-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-195">zoomDisabled</span></span>|<span data-ttu-id="1d4e2-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-196">Boolean</span></span>|<span data-ttu-id="1d4e2-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-198">siriDisabled</span></span>|<span data-ttu-id="1d4e2-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-199">Boolean</span></span>|<span data-ttu-id="1d4e2-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-201">diagnosticsDisabled</span></span>|<span data-ttu-id="1d4e2-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-202">Boolean</span></span>|<span data-ttu-id="1d4e2-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="1d4e2-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-205">Boolean</span></span>|<span data-ttu-id="1d4e2-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-207">privacyPaneDisabled</span></span>|<span data-ttu-id="1d4e2-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-208">Boolean</span></span>|<span data-ttu-id="1d4e2-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-210">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-210">screenTimeScreenDisabled</span></span>|<span data-ttu-id="1d4e2-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-211">Boolean</span></span>|<span data-ttu-id="1d4e2-212">Indica se a configuração de tempo limite da tela está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-212">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-213">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="1d4e2-213">deviceNameTemplate</span></span>|<span data-ttu-id="1d4e2-214">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4e2-214">String</span></span>|<span data-ttu-id="1d4e2-215">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-215">Sets a literal or name pattern.</span></span> <span data-ttu-id="1d4e2-216">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-216">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-217">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="1d4e2-217">configurationWebUrl</span></span>|<span data-ttu-id="1d4e2-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-218">Boolean</span></span>|<span data-ttu-id="1d4e2-219">URL do logon do assistente de configuração herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-219">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="1d4e2-220">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="1d4e2-220">iTunesPairingMode</span></span>|[<span data-ttu-id="1d4e2-221">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="1d4e2-221">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="1d4e2-222">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-222">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="1d4e2-223">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-223">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="1d4e2-224">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="1d4e2-224">managementCertificates</span></span>|<span data-ttu-id="1d4e2-225">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="1d4e2-225">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="1d4e2-226">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="1d4e2-226">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="1d4e2-227">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-227">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="1d4e2-228">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-228">Boolean</span></span>|<span data-ttu-id="1d4e2-229">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-229">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="1d4e2-230">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="1d4e2-230">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="1d4e2-231">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-231">Boolean</span></span>|<span data-ttu-id="1d4e2-232">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-232">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="1d4e2-233">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="1d4e2-233">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="1d4e2-234">Int32</span><span class="sxs-lookup"><span data-stu-id="1d4e2-234">Int32</span></span>|<span data-ttu-id="1d4e2-235">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-235">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="1d4e2-236">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-236">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="1d4e2-237">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="1d4e2-237">enableSharedIPad</span></span>|<span data-ttu-id="1d4e2-238">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-238">Boolean</span></span>|<span data-ttu-id="1d4e2-239">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-239">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="1d4e2-240">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-240">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="1d4e2-241">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="1d4e2-241">companyPortalVppTokenId</span></span>|<span data-ttu-id="1d4e2-242">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="1d4e2-242">String</span></span>|<span data-ttu-id="1d4e2-243">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-243">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="1d4e2-244">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-244">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="1d4e2-245">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="1d4e2-245">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="1d4e2-246">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-246">Boolean</span></span>|<span data-ttu-id="1d4e2-247">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-247">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="1d4e2-248">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-248">Default is false.</span></span> <span data-ttu-id="1d4e2-249">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-249">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="1d4e2-250">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-250">homeButtonScreenDisabled</span></span>|<span data-ttu-id="1d4e2-251">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-251">Boolean</span></span>|<span data-ttu-id="1d4e2-252">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-252">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-253">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-253">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="1d4e2-254">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-254">Boolean</span></span>|<span data-ttu-id="1d4e2-255">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-255">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-256">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-256">onBoardingScreenDisabled</span></span>|<span data-ttu-id="1d4e2-257">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-257">Boolean</span></span>|<span data-ttu-id="1d4e2-258">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-258">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-259">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-259">simSetupScreenDisabled</span></span>|<span data-ttu-id="1d4e2-260">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-260">Boolean</span></span>|<span data-ttu-id="1d4e2-261">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-261">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-262">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-262">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="1d4e2-263">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-263">Boolean</span></span>|<span data-ttu-id="1d4e2-264">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-264">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-265">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-265">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="1d4e2-266">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-266">Boolean</span></span>|<span data-ttu-id="1d4e2-267">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-267">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-268">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-268">appearanceScreenDisabled</span></span>|<span data-ttu-id="1d4e2-269">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-269">Boolean</span></span>|<span data-ttu-id="1d4e2-270">Indica se a tela do apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-270">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-271">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-271">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="1d4e2-272">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-272">Boolean</span></span>|<span data-ttu-id="1d4e2-273">Indica se a tela de idioma expresso está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-273">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-274">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-274">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="1d4e2-275">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-275">Boolean</span></span>|<span data-ttu-id="1d4e2-276">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-276">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="1d4e2-277">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-277">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="1d4e2-278">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-278">Boolean</span></span>|<span data-ttu-id="1d4e2-279">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-279">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="1d4e2-280">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="1d4e2-280">welcomeScreenDisabled</span></span>|<span data-ttu-id="1d4e2-281">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d4e2-281">Boolean</span></span>|<span data-ttu-id="1d4e2-282">Indica se a tela do weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="1d4e2-282">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="1d4e2-283">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d4e2-283">Response</span></span>
<span data-ttu-id="1d4e2-284">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-284">If successful, this method returns a `201 Created` response code and a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1d4e2-285">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1d4e2-285">Example</span></span>

### <a name="request"></a><span data-ttu-id="1d4e2-286">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1d4e2-286">Request</span></span>
<span data-ttu-id="1d4e2-287">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-287">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
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

### <a name="response"></a><span data-ttu-id="1d4e2-288">Resposta</span><span class="sxs-lookup"><span data-stu-id="1d4e2-288">Response</span></span>
<span data-ttu-id="1d4e2-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1d4e2-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





