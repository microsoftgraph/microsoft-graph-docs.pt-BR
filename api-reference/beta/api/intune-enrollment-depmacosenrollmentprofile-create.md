---
title: Criar depMacOSEnrollmentProfile
description: Crie um novo objeto de depMacOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b7fd29ee598507b982ecd48ea58b6a09ccf90972
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420588"
---
# <a name="create-depmacosenrollmentprofile"></a><span data-ttu-id="e44b4-103">Criar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="e44b4-103">Create depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="e44b4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e44b4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e44b4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e44b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e44b4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e44b4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e44b4-107">Crie um novo objeto de [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="e44b4-107">Create a new [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e44b4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e44b4-108">Prerequisites</span></span>
<span data-ttu-id="e44b4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e44b4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e44b4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e44b4-111">Permission type</span></span>|<span data-ttu-id="e44b4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e44b4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e44b4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e44b4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e44b4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e44b4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e44b4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e44b4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e44b4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44b4-116">Not supported.</span></span>|
|<span data-ttu-id="e44b4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e44b4-117">Application</span></span>|<span data-ttu-id="e44b4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e44b4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e44b4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e44b4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="e44b4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e44b4-120">Request headers</span></span>
|<span data-ttu-id="e44b4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e44b4-121">Header</span></span>|<span data-ttu-id="e44b4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e44b4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e44b4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e44b4-123">Authorization</span></span>|<span data-ttu-id="e44b4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e44b4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e44b4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e44b4-125">Accept</span></span>|<span data-ttu-id="e44b4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e44b4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e44b4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e44b4-127">Request body</span></span>
<span data-ttu-id="e44b4-128">No corpo da solicitação, fornece uma representação JSON para o objeto depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e44b4-128">In the request body, supply a JSON representation for the depMacOSEnrollmentProfile object.</span></span>

<span data-ttu-id="e44b4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o depMacOSEnrollmentProfile.</span><span class="sxs-lookup"><span data-stu-id="e44b4-129">The following table shows the properties that are required when you create the depMacOSEnrollmentProfile.</span></span>

|<span data-ttu-id="e44b4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e44b4-130">Property</span></span>|<span data-ttu-id="e44b4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e44b4-131">Type</span></span>|<span data-ttu-id="e44b4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e44b4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e44b4-133">id</span><span class="sxs-lookup"><span data-stu-id="e44b4-133">id</span></span>|<span data-ttu-id="e44b4-134">String</span><span class="sxs-lookup"><span data-stu-id="e44b4-134">String</span></span>|<span data-ttu-id="e44b4-135">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e44b4-136">displayName</span></span>|<span data-ttu-id="e44b4-137">String</span><span class="sxs-lookup"><span data-stu-id="e44b4-137">String</span></span>|<span data-ttu-id="e44b4-138">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-139">description</span><span class="sxs-lookup"><span data-stu-id="e44b4-139">description</span></span>|<span data-ttu-id="e44b4-140">String</span><span class="sxs-lookup"><span data-stu-id="e44b4-140">String</span></span>|<span data-ttu-id="e44b4-141">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="e44b4-142">requiresUserAuthentication</span></span>|<span data-ttu-id="e44b4-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-143">Boolean</span></span>|<span data-ttu-id="e44b4-144">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="e44b4-145">configurationEndpointUrl</span></span>|<span data-ttu-id="e44b4-146">String</span><span class="sxs-lookup"><span data-stu-id="e44b4-146">String</span></span>|<span data-ttu-id="e44b4-147">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="e44b4-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="e44b4-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-149">Boolean</span></span>|<span data-ttu-id="e44b4-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="e44b4-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="e44b4-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="e44b4-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="e44b4-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-153">Boolean</span></span>|<span data-ttu-id="e44b4-154">Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="e44b4-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="e44b4-155">isDefault</span></span>|<span data-ttu-id="e44b4-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-156">Boolean</span></span>|<span data-ttu-id="e44b4-157">Indica se esse é o perfil padrão Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-158">supervisedModeEnabled</span></span>|<span data-ttu-id="e44b4-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-159">Boolean</span></span>|<span data-ttu-id="e44b4-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="e44b4-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="e44b4-161">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="e44b4-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="e44b4-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="e44b4-163">supportDepartment</span></span>|<span data-ttu-id="e44b4-164">String</span><span class="sxs-lookup"><span data-stu-id="e44b4-164">String</span></span>|<span data-ttu-id="e44b4-165">Informações de departamento de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-166">passCodeDisabled</span></span>|<span data-ttu-id="e44b4-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-167">Boolean</span></span>|<span data-ttu-id="e44b4-168">Indica se a senha instalação painel está desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="e44b4-169">isMandatory</span></span>|<span data-ttu-id="e44b4-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-170">Boolean</span></span>|<span data-ttu-id="e44b4-171">Indica se o perfil é obrigatória herdar de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-172">locationDisabled</span></span>|<span data-ttu-id="e44b4-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-173">Boolean</span></span>|<span data-ttu-id="e44b4-174">Indica se o local do painel de configuração do serviço é desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="e44b4-175">supportPhoneNumber</span></span>|<span data-ttu-id="e44b4-176">String</span><span class="sxs-lookup"><span data-stu-id="e44b4-176">String</span></span>|<span data-ttu-id="e44b4-177">Número de telefone de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-178">profileRemovalDisabled</span></span>|<span data-ttu-id="e44b4-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-179">Boolean</span></span>|<span data-ttu-id="e44b4-180">Indica se a opção de remoção de perfil será desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="e44b4-181">restoreBlocked</span></span>|<span data-ttu-id="e44b4-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-182">Boolean</span></span>|<span data-ttu-id="e44b4-183">Indica se o painel de configuração de restauração será bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-184">appleIdDisabled</span></span>|<span data-ttu-id="e44b4-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-185">Boolean</span></span>|<span data-ttu-id="e44b4-186">Indica se o Apple painel de configuração de id estará desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="e44b4-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-188">Boolean</span></span>|<span data-ttu-id="e44b4-189">Indica se o painel de configuração de 'Termos e condições' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-190">touchIdDisabled</span></span>|<span data-ttu-id="e44b4-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-191">Boolean</span></span>|<span data-ttu-id="e44b4-192">Indica se o painel de configuração de id de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-193">applePayDisabled</span></span>|<span data-ttu-id="e44b4-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-194">Boolean</span></span>|<span data-ttu-id="e44b4-195">Indica se o painel de configuração de pagamento do Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-196">zoomDisabled</span></span>|<span data-ttu-id="e44b4-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-197">Boolean</span></span>|<span data-ttu-id="e44b4-198">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-199">siriDisabled</span></span>|<span data-ttu-id="e44b4-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-200">Boolean</span></span>|<span data-ttu-id="e44b4-201">Indica se o painel de configuração de siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-202">diagnosticsDisabled</span></span>|<span data-ttu-id="e44b4-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-203">Boolean</span></span>|<span data-ttu-id="e44b4-204">Indica se o diagnóstico do painel de instalação está desabilitada Inherited em [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="e44b4-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-206">Boolean</span></span>|<span data-ttu-id="e44b4-207">Indica se a tela de instalação do displaytone está desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-208">privacyPaneDisabled</span></span>|<span data-ttu-id="e44b4-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-209">Boolean</span></span>|<span data-ttu-id="e44b4-210">Indica se a tela de privacidade está desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="e44b4-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="e44b4-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-211">registrationDisabled</span></span>|<span data-ttu-id="e44b4-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-212">Boolean</span></span>|<span data-ttu-id="e44b4-213">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e44b4-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="e44b4-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-214">fileVaultDisabled</span></span>|<span data-ttu-id="e44b4-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-215">Boolean</span></span>|<span data-ttu-id="e44b4-216">Indica se o armazenamento de arquivo está desabilitado</span><span class="sxs-lookup"><span data-stu-id="e44b4-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="e44b4-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="e44b4-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="e44b4-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="e44b4-218">Boolean</span></span>|<span data-ttu-id="e44b4-219">Indica se a tela de análise de iCloud está desabilitada</span><span class="sxs-lookup"><span data-stu-id="e44b4-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="e44b4-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44b4-220">Response</span></span>
<span data-ttu-id="e44b4-221">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e44b4-221">If successful, this method returns a `201 Created` response code and a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e44b4-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e44b4-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="e44b4-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e44b4-223">Request</span></span>
<span data-ttu-id="e44b4-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e44b4-224">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles
Content-type: application/json
Content-length: 1061

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
  "iCloudDiagnosticsDisabled": true
}
```

### <a name="response"></a><span data-ttu-id="e44b4-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="e44b4-225">Response</span></span>
<span data-ttu-id="e44b4-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e44b4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1110

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
  "iCloudDiagnosticsDisabled": true
}
```




