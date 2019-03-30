---
title: Atualizar depIOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depIOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ea708a5ffe661f8024c027d1ac9ef10877474cd6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30986940"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="78ea0-103">Atualizar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78ea0-103">Update depIOSEnrollmentProfile</span></span>

> <span data-ttu-id="78ea0-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78ea0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78ea0-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78ea0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78ea0-106">Atualiza as propriedades de um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="78ea0-106">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="78ea0-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="78ea0-107">Prerequisites</span></span>
<span data-ttu-id="78ea0-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="78ea0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78ea0-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="78ea0-110">Permission type</span></span>|<span data-ttu-id="78ea0-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="78ea0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78ea0-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="78ea0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="78ea0-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78ea0-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="78ea0-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="78ea0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78ea0-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78ea0-115">Not supported.</span></span>|
|<span data-ttu-id="78ea0-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="78ea0-116">Application</span></span>|<span data-ttu-id="78ea0-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="78ea0-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78ea0-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="78ea0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="78ea0-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="78ea0-119">Request headers</span></span>
|<span data-ttu-id="78ea0-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="78ea0-120">Header</span></span>|<span data-ttu-id="78ea0-121">Valor</span><span class="sxs-lookup"><span data-stu-id="78ea0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78ea0-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="78ea0-122">Authorization</span></span>|<span data-ttu-id="78ea0-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="78ea0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78ea0-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="78ea0-124">Accept</span></span>|<span data-ttu-id="78ea0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="78ea0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78ea0-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="78ea0-126">Request body</span></span>
<span data-ttu-id="78ea0-127">No corpo da solicitação, forneça uma representação JSON do objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="78ea0-127">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="78ea0-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="78ea0-128">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="78ea0-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78ea0-129">Property</span></span>|<span data-ttu-id="78ea0-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="78ea0-130">Type</span></span>|<span data-ttu-id="78ea0-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="78ea0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78ea0-132">id</span><span class="sxs-lookup"><span data-stu-id="78ea0-132">id</span></span>|<span data-ttu-id="78ea0-133">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-133">String</span></span>|<span data-ttu-id="78ea0-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-135">displayName</span><span class="sxs-lookup"><span data-stu-id="78ea0-135">displayName</span></span>|<span data-ttu-id="78ea0-136">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-136">String</span></span>|<span data-ttu-id="78ea0-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-138">description</span><span class="sxs-lookup"><span data-stu-id="78ea0-138">description</span></span>|<span data-ttu-id="78ea0-139">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-139">String</span></span>|<span data-ttu-id="78ea0-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="78ea0-141">requiresUserAuthentication</span></span>|<span data-ttu-id="78ea0-142">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-142">Boolean</span></span>|<span data-ttu-id="78ea0-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="78ea0-144">configurationEndpointUrl</span></span>|<span data-ttu-id="78ea0-145">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-145">String</span></span>|<span data-ttu-id="78ea0-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="78ea0-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="78ea0-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-148">Boolean</span></span>|<span data-ttu-id="78ea0-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="78ea0-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="78ea0-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="78ea0-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="78ea0-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-152">Boolean</span></span>|<span data-ttu-id="78ea0-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="78ea0-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="78ea0-154">isDefault</span></span>|<span data-ttu-id="78ea0-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-155">Boolean</span></span>|<span data-ttu-id="78ea0-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-157">supervisedModeEnabled</span></span>|<span data-ttu-id="78ea0-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-158">Boolean</span></span>|<span data-ttu-id="78ea0-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="78ea0-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="78ea0-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="78ea0-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="78ea0-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="78ea0-162">supportDepartment</span></span>|<span data-ttu-id="78ea0-163">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-163">String</span></span>|<span data-ttu-id="78ea0-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-165">passCodeDisabled</span></span>|<span data-ttu-id="78ea0-166">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-166">Boolean</span></span>|<span data-ttu-id="78ea0-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="78ea0-168">isMandatory</span></span>|<span data-ttu-id="78ea0-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-169">Boolean</span></span>|<span data-ttu-id="78ea0-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-171">locationDisabled</span></span>|<span data-ttu-id="78ea0-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-172">Boolean</span></span>|<span data-ttu-id="78ea0-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="78ea0-174">supportPhoneNumber</span></span>|<span data-ttu-id="78ea0-175">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-175">String</span></span>|<span data-ttu-id="78ea0-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-177">profileRemovalDisabled</span></span>|<span data-ttu-id="78ea0-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-178">Boolean</span></span>|<span data-ttu-id="78ea0-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="78ea0-180">restoreBlocked</span></span>|<span data-ttu-id="78ea0-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-181">Boolean</span></span>|<span data-ttu-id="78ea0-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-183">appleIdDisabled</span></span>|<span data-ttu-id="78ea0-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-184">Boolean</span></span>|<span data-ttu-id="78ea0-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="78ea0-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-187">Boolean</span></span>|<span data-ttu-id="78ea0-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-189">touchIdDisabled</span></span>|<span data-ttu-id="78ea0-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-190">Boolean</span></span>|<span data-ttu-id="78ea0-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-192">applePayDisabled</span></span>|<span data-ttu-id="78ea0-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-193">Boolean</span></span>|<span data-ttu-id="78ea0-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-195">zoomDisabled</span></span>|<span data-ttu-id="78ea0-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-196">Boolean</span></span>|<span data-ttu-id="78ea0-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-198">siriDisabled</span></span>|<span data-ttu-id="78ea0-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-199">Boolean</span></span>|<span data-ttu-id="78ea0-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-201">diagnosticsDisabled</span></span>|<span data-ttu-id="78ea0-202">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-202">Boolean</span></span>|<span data-ttu-id="78ea0-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="78ea0-205">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-205">Boolean</span></span>|<span data-ttu-id="78ea0-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-207">privacyPaneDisabled</span></span>|<span data-ttu-id="78ea0-208">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-208">Boolean</span></span>|<span data-ttu-id="78ea0-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="78ea0-210">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="78ea0-210">iTunesPairingMode</span></span>|[<span data-ttu-id="78ea0-211">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="78ea0-211">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="78ea0-212">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="78ea0-212">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="78ea0-213">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="78ea0-213">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="78ea0-214">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="78ea0-214">managementCertificates</span></span>|<span data-ttu-id="78ea0-215">coleção [managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="78ea0-215">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="78ea0-216">Certificados de gerenciamento para o Apple conFigurator</span><span class="sxs-lookup"><span data-stu-id="78ea0-216">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="78ea0-217">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-217">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="78ea0-218">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-218">Boolean</span></span>|<span data-ttu-id="78ea0-219">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-219">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="78ea0-220">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="78ea0-220">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="78ea0-221">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-221">Boolean</span></span>|<span data-ttu-id="78ea0-222">Indica se o dispositivo deverá aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="78ea0-222">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="78ea0-223">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="78ea0-223">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="78ea0-224">Int32</span><span class="sxs-lookup"><span data-stu-id="78ea0-224">Int32</span></span>|<span data-ttu-id="78ea0-225">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="78ea0-225">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="78ea0-226">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="78ea0-226">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="78ea0-227">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="78ea0-227">enableSharedIPad</span></span>|<span data-ttu-id="78ea0-228">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-228">Boolean</span></span>|<span data-ttu-id="78ea0-229">Isso indica se o dispositivo deve ser inscrito em um modo que permite cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="78ea0-229">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="78ea0-230">Aplicável somente no iPads compartilhado.</span><span class="sxs-lookup"><span data-stu-id="78ea0-230">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="78ea0-231">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="78ea0-231">companyPortalVppTokenId</span></span>|<span data-ttu-id="78ea0-232">String</span><span class="sxs-lookup"><span data-stu-id="78ea0-232">String</span></span>|<span data-ttu-id="78ea0-233">Se definido, indica qual token VPP deve ser usado para implantar o portal da empresa com licenciamento de dispositivo.</span><span class="sxs-lookup"><span data-stu-id="78ea0-233">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="78ea0-234">"Enableauthenticationviacompanyportal foi adicionada" deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="78ea0-234">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="78ea0-235">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="78ea0-235">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="78ea0-236">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-236">Boolean</span></span>|<span data-ttu-id="78ea0-237">Informa ao dispositivo para habilitar o modo de um único aplicativo e aplicar o aplicativo-bloquear durante o registro.</span><span class="sxs-lookup"><span data-stu-id="78ea0-237">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="78ea0-238">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="78ea0-238">Default is false.</span></span> <span data-ttu-id="78ea0-239">' Enableauthenticationviacompanyportal foi adicionada ' e ' companyPortalVppTokenId ' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="78ea0-239">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="78ea0-240">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-240">homeButtonScreenDisabled</span></span>|<span data-ttu-id="78ea0-241">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-241">Boolean</span></span>|<span data-ttu-id="78ea0-242">Indica se a tela de sensibilidade do botão da página inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-242">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="78ea0-243">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-243">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="78ea0-244">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-244">Boolean</span></span>|<span data-ttu-id="78ea0-245">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-245">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="78ea0-246">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-246">onBoardingScreenDisabled</span></span>|<span data-ttu-id="78ea0-247">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-247">Boolean</span></span>|<span data-ttu-id="78ea0-248">Indica se a tela de configuração de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-248">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="78ea0-249">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-249">screenTimeScreenDisabled</span></span>|<span data-ttu-id="78ea0-250">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-250">Boolean</span></span>|<span data-ttu-id="78ea0-251">Indica se a configuração de tempo limite da tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-251">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="78ea0-252">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-252">simSetupScreenDisabled</span></span>|<span data-ttu-id="78ea0-253">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-253">Boolean</span></span>|<span data-ttu-id="78ea0-254">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-254">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="78ea0-255">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-255">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="78ea0-256">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-256">Boolean</span></span>|<span data-ttu-id="78ea0-257">Indica se a tela obrigatória atualização de sofware está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-257">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="78ea0-258">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="78ea0-258">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="78ea0-259">Booliano</span><span class="sxs-lookup"><span data-stu-id="78ea0-259">Boolean</span></span>|<span data-ttu-id="78ea0-260">Indica se a tela Watch Migration está desabilitada</span><span class="sxs-lookup"><span data-stu-id="78ea0-260">Indicates if the watch migration screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="78ea0-261">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ea0-261">Response</span></span>
<span data-ttu-id="78ea0-262">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="78ea0-262">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78ea0-263">Exemplo</span><span class="sxs-lookup"><span data-stu-id="78ea0-263">Example</span></span>

### <a name="request"></a><span data-ttu-id="78ea0-264">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78ea0-264">Request</span></span>
<span data-ttu-id="78ea0-265">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="78ea0-265">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="78ea0-266">Resposta</span><span class="sxs-lookup"><span data-stu-id="78ea0-266">Response</span></span>
<span data-ttu-id="78ea0-p109">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="78ea0-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




