---
title: Atualizar depMacOSEnrollmentProfile
description: Atualiza as propriedades de um objeto depMacOSEnrollmentProfile.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f386801f1edf03544f46f4f730e830ef70130f7
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2019
ms.locfileid: "30978476"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="d69f5-103">Atualizar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d69f5-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="d69f5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d69f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d69f5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d69f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d69f5-106">Atualiza as propriedades de um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d69f5-106">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d69f5-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d69f5-107">Prerequisites</span></span>
<span data-ttu-id="d69f5-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d69f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d69f5-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d69f5-110">Permission type</span></span>|<span data-ttu-id="d69f5-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d69f5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d69f5-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d69f5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d69f5-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d69f5-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d69f5-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d69f5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d69f5-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d69f5-115">Not supported.</span></span>|
|<span data-ttu-id="d69f5-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d69f5-116">Application</span></span>|<span data-ttu-id="d69f5-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d69f5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d69f5-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d69f5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="d69f5-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d69f5-119">Request headers</span></span>
|<span data-ttu-id="d69f5-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d69f5-120">Header</span></span>|<span data-ttu-id="d69f5-121">Valor</span><span class="sxs-lookup"><span data-stu-id="d69f5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d69f5-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="d69f5-122">Authorization</span></span>|<span data-ttu-id="d69f5-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d69f5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d69f5-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d69f5-124">Accept</span></span>|<span data-ttu-id="d69f5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d69f5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d69f5-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d69f5-126">Request body</span></span>
<span data-ttu-id="d69f5-127">No corpo da solicitação, forneça uma representação JSON do objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d69f5-127">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="d69f5-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d69f5-128">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="d69f5-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d69f5-129">Property</span></span>|<span data-ttu-id="d69f5-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="d69f5-130">Type</span></span>|<span data-ttu-id="d69f5-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="d69f5-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d69f5-132">id</span><span class="sxs-lookup"><span data-stu-id="d69f5-132">id</span></span>|<span data-ttu-id="d69f5-133">String</span><span class="sxs-lookup"><span data-stu-id="d69f5-133">String</span></span>|<span data-ttu-id="d69f5-134">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-134">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d69f5-135">displayName</span></span>|<span data-ttu-id="d69f5-136">String</span><span class="sxs-lookup"><span data-stu-id="d69f5-136">String</span></span>|<span data-ttu-id="d69f5-137">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-137">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-138">descrição</span><span class="sxs-lookup"><span data-stu-id="d69f5-138">description</span></span>|<span data-ttu-id="d69f5-139">String</span><span class="sxs-lookup"><span data-stu-id="d69f5-139">String</span></span>|<span data-ttu-id="d69f5-140">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-140">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-141">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="d69f5-141">requiresUserAuthentication</span></span>|<span data-ttu-id="d69f5-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-142">Boolean</span></span>|<span data-ttu-id="d69f5-143">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-143">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-144">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="d69f5-144">configurationEndpointUrl</span></span>|<span data-ttu-id="d69f5-145">String</span><span class="sxs-lookup"><span data-stu-id="d69f5-145">String</span></span>|<span data-ttu-id="d69f5-146">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-146">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-147">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="d69f5-147">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="d69f5-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-148">Boolean</span></span>|<span data-ttu-id="d69f5-149">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="d69f5-149">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="d69f5-150">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-150">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="d69f5-151">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="d69f5-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-152">Boolean</span></span>|<span data-ttu-id="d69f5-153">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-153">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="d69f5-154">isDefault</span><span class="sxs-lookup"><span data-stu-id="d69f5-154">isDefault</span></span>|<span data-ttu-id="d69f5-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="d69f5-155">Boolean</span></span>|<span data-ttu-id="d69f5-156">Indica se este é o perfil padrão herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-156">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-157">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-157">supervisedModeEnabled</span></span>|<span data-ttu-id="d69f5-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-158">Boolean</span></span>|<span data-ttu-id="d69f5-159">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="d69f5-159">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="d69f5-160">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="d69f5-160">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="d69f5-161">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-161">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-162">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="d69f5-162">supportDepartment</span></span>|<span data-ttu-id="d69f5-163">String</span><span class="sxs-lookup"><span data-stu-id="d69f5-163">String</span></span>|<span data-ttu-id="d69f5-164">Informações do departamento de suporte herdadas de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-164">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-165">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-165">passCodeDisabled</span></span>|<span data-ttu-id="d69f5-166">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-166">Boolean</span></span>|<span data-ttu-id="d69f5-167">Indica se o painel de configuração de senha está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-167">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-168">isMandatory</span><span class="sxs-lookup"><span data-stu-id="d69f5-168">isMandatory</span></span>|<span data-ttu-id="d69f5-169">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-169">Boolean</span></span>|<span data-ttu-id="d69f5-170">Indica se o perfil é obrigatório herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-170">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-171">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-171">locationDisabled</span></span>|<span data-ttu-id="d69f5-172">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-172">Boolean</span></span>|<span data-ttu-id="d69f5-173">Indica se o painel de instalação do serviço de localização está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-173">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-174">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="d69f5-174">supportPhoneNumber</span></span>|<span data-ttu-id="d69f5-175">String</span><span class="sxs-lookup"><span data-stu-id="d69f5-175">String</span></span>|<span data-ttu-id="d69f5-176">Número de telefone de suporte herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-176">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-177">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-177">profileRemovalDisabled</span></span>|<span data-ttu-id="d69f5-178">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-178">Boolean</span></span>|<span data-ttu-id="d69f5-179">Indica se a opção de remoção de perfil está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-179">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-180">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="d69f5-180">restoreBlocked</span></span>|<span data-ttu-id="d69f5-181">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-181">Boolean</span></span>|<span data-ttu-id="d69f5-182">Indica se o painel de configuração de restauração é bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-182">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-183">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-183">appleIdDisabled</span></span>|<span data-ttu-id="d69f5-184">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-184">Boolean</span></span>|<span data-ttu-id="d69f5-185">Indica se o painel de configuração da Apple ID está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-185">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-186">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-186">termsAndConditionsDisabled</span></span>|<span data-ttu-id="d69f5-187">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-187">Boolean</span></span>|<span data-ttu-id="d69f5-188">Indica se o painel de configuração ' termos e condições ' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-188">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-189">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-189">touchIdDisabled</span></span>|<span data-ttu-id="d69f5-190">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-190">Boolean</span></span>|<span data-ttu-id="d69f5-191">Indica se o painel de configuração de ID de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-191">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-192">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-192">applePayDisabled</span></span>|<span data-ttu-id="d69f5-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-193">Boolean</span></span>|<span data-ttu-id="d69f5-194">Indica se o painel de configuração de pagamento da Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-194">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-195">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-195">zoomDisabled</span></span>|<span data-ttu-id="d69f5-196">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-196">Boolean</span></span>|<span data-ttu-id="d69f5-197">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-197">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-198">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-198">siriDisabled</span></span>|<span data-ttu-id="d69f5-199">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-199">Boolean</span></span>|<span data-ttu-id="d69f5-200">Indica se o painel de configuração do Siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-200">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-201">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-201">diagnosticsDisabled</span></span>|<span data-ttu-id="d69f5-202">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-202">Boolean</span></span>|<span data-ttu-id="d69f5-203">Indica se o painel de configuração de diagnóstico está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-203">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-204">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-204">displayToneSetupDisabled</span></span>|<span data-ttu-id="d69f5-205">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-205">Boolean</span></span>|<span data-ttu-id="d69f5-206">Indica se a tela de configuração do displaytone está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-206">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-207">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-207">privacyPaneDisabled</span></span>|<span data-ttu-id="d69f5-208">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-208">Boolean</span></span>|<span data-ttu-id="d69f5-209">Indica se a tela de privacidade está desabilitada herdada de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d69f5-209">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="d69f5-210">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-210">registrationDisabled</span></span>|<span data-ttu-id="d69f5-211">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-211">Boolean</span></span>|<span data-ttu-id="d69f5-212">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="d69f5-212">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="d69f5-213">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-213">fileVaultDisabled</span></span>|<span data-ttu-id="d69f5-214">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-214">Boolean</span></span>|<span data-ttu-id="d69f5-215">Indica se o compartimento de arquivos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="d69f5-215">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="d69f5-216">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-216">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="d69f5-217">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-217">Boolean</span></span>|<span data-ttu-id="d69f5-218">Indica se a tela do iCloud Analytics está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d69f5-218">Indicates if iCloud Analytics screen is disabled</span></span>|
|<span data-ttu-id="d69f5-219">iCloudStorageDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-219">iCloudStorageDisabled</span></span>|<span data-ttu-id="d69f5-220">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-220">Boolean</span></span>|<span data-ttu-id="d69f5-221">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d69f5-221">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|
|<span data-ttu-id="d69f5-222">chooseYourLockScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="d69f5-222">chooseYourLockScreenDisabled</span></span>|<span data-ttu-id="d69f5-223">Boolean</span><span class="sxs-lookup"><span data-stu-id="d69f5-223">Boolean</span></span>|<span data-ttu-id="d69f5-224">Indica se a tela documentos do iCloud e área de trabalho está desabilitada</span><span class="sxs-lookup"><span data-stu-id="d69f5-224">Indicates if iCloud Documents and Desktop screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="d69f5-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="d69f5-225">Response</span></span>
<span data-ttu-id="d69f5-226">Se tiver êxito, este método retornará `200 OK` um código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="d69f5-226">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d69f5-227">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d69f5-227">Example</span></span>

### <a name="request"></a><span data-ttu-id="d69f5-228">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d69f5-228">Request</span></span>
<span data-ttu-id="d69f5-229">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d69f5-229">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
Content-type: application/json
Content-length: 1136

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="d69f5-230">Resposta</span><span class="sxs-lookup"><span data-stu-id="d69f5-230">Response</span></span>
<span data-ttu-id="d69f5-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d69f5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1185

{
  "@odata.type": "#microsoft.graph.depMacOSEnrollmentProfile",
  "id": "e433c95c-c95c-e433-5cc9-33e45cc933e4",
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
  "registrationDisabled": true,
  "fileVaultDisabled": true,
  "iCloudDiagnosticsDisabled": true,
  "iCloudStorageDisabled": true,
  "chooseYourLockScreenDisabled": true
}
```




