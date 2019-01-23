---
title: Atualizar depMacOSEnrollmentProfile
description: Atualize as propriedades de um objeto depMacOSEnrollmentProfile.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f86e520160e988e72aaa2473b256613a997cae0c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420112"
---
# <a name="update-depmacosenrollmentprofile"></a><span data-ttu-id="f03d3-103">Atualizar depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f03d3-103">Update depMacOSEnrollmentProfile</span></span>

> <span data-ttu-id="f03d3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="f03d3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f03d3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f03d3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f03d3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="f03d3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f03d3-107">Atualize as propriedades de um objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f03d3-107">Update the properties of a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f03d3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f03d3-108">Prerequisites</span></span>
<span data-ttu-id="f03d3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="f03d3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f03d3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f03d3-111">Permission type</span></span>|<span data-ttu-id="f03d3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f03d3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f03d3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f03d3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f03d3-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f03d3-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f03d3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f03d3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f03d3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f03d3-116">Not supported.</span></span>|
|<span data-ttu-id="f03d3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f03d3-117">Application</span></span>|<span data-ttu-id="f03d3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f03d3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f03d3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f03d3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="f03d3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f03d3-120">Request headers</span></span>
|<span data-ttu-id="f03d3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f03d3-121">Header</span></span>|<span data-ttu-id="f03d3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f03d3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f03d3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f03d3-123">Authorization</span></span>|<span data-ttu-id="f03d3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f03d3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f03d3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f03d3-125">Accept</span></span>|<span data-ttu-id="f03d3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f03d3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f03d3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f03d3-127">Request body</span></span>
<span data-ttu-id="f03d3-128">No corpo da solicitação, fornece uma representação JSON para o objeto [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f03d3-128">In the request body, supply a JSON representation for the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="f03d3-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="f03d3-129">The following table shows the properties that are required when you create the [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

|<span data-ttu-id="f03d3-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f03d3-130">Property</span></span>|<span data-ttu-id="f03d3-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f03d3-131">Type</span></span>|<span data-ttu-id="f03d3-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f03d3-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f03d3-133">id</span><span class="sxs-lookup"><span data-stu-id="f03d3-133">id</span></span>|<span data-ttu-id="f03d3-134">String</span><span class="sxs-lookup"><span data-stu-id="f03d3-134">String</span></span>|<span data-ttu-id="f03d3-135">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-136">displayName</span><span class="sxs-lookup"><span data-stu-id="f03d3-136">displayName</span></span>|<span data-ttu-id="f03d3-137">String</span><span class="sxs-lookup"><span data-stu-id="f03d3-137">String</span></span>|<span data-ttu-id="f03d3-138">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-139">description</span><span class="sxs-lookup"><span data-stu-id="f03d3-139">description</span></span>|<span data-ttu-id="f03d3-140">String</span><span class="sxs-lookup"><span data-stu-id="f03d3-140">String</span></span>|<span data-ttu-id="f03d3-141">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f03d3-142">requiresUserAuthentication</span></span>|<span data-ttu-id="f03d3-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-143">Boolean</span></span>|<span data-ttu-id="f03d3-144">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f03d3-145">configurationEndpointUrl</span></span>|<span data-ttu-id="f03d3-146">String</span><span class="sxs-lookup"><span data-stu-id="f03d3-146">String</span></span>|<span data-ttu-id="f03d3-147">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="f03d3-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f03d3-149">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-149">Boolean</span></span>|<span data-ttu-id="f03d3-150">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="f03d3-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f03d3-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f03d3-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f03d3-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-153">Boolean</span></span>|<span data-ttu-id="f03d3-154">Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f03d3-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="f03d3-155">isDefault</span></span>|<span data-ttu-id="f03d3-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-156">Boolean</span></span>|<span data-ttu-id="f03d3-157">Indica se esse é o perfil padrão Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-158">supervisedModeEnabled</span></span>|<span data-ttu-id="f03d3-159">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-159">Boolean</span></span>|<span data-ttu-id="f03d3-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="f03d3-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f03d3-161">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f03d3-161">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="f03d3-162">Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f03d3-163">supportDepartment</span></span>|<span data-ttu-id="f03d3-164">String</span><span class="sxs-lookup"><span data-stu-id="f03d3-164">String</span></span>|<span data-ttu-id="f03d3-165">Informações de departamento de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-166">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-166">passCodeDisabled</span></span>|<span data-ttu-id="f03d3-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-167">Boolean</span></span>|<span data-ttu-id="f03d3-168">Indica se a senha instalação painel está desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-168">Indicates if Passcode setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-169">isMandatory</span><span class="sxs-lookup"><span data-stu-id="f03d3-169">isMandatory</span></span>|<span data-ttu-id="f03d3-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-170">Boolean</span></span>|<span data-ttu-id="f03d3-171">Indica se o perfil é obrigatória herdar de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-171">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-172">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-172">locationDisabled</span></span>|<span data-ttu-id="f03d3-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-173">Boolean</span></span>|<span data-ttu-id="f03d3-174">Indica se o local do painel de configuração do serviço é desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-174">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-175">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f03d3-175">supportPhoneNumber</span></span>|<span data-ttu-id="f03d3-176">String</span><span class="sxs-lookup"><span data-stu-id="f03d3-176">String</span></span>|<span data-ttu-id="f03d3-177">Número de telefone de suporte Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-177">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-178">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-178">profileRemovalDisabled</span></span>|<span data-ttu-id="f03d3-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-179">Boolean</span></span>|<span data-ttu-id="f03d3-180">Indica se a opção de remoção de perfil será desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-180">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-181">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f03d3-181">restoreBlocked</span></span>|<span data-ttu-id="f03d3-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-182">Boolean</span></span>|<span data-ttu-id="f03d3-183">Indica se o painel de configuração de restauração será bloqueado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-183">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-184">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-184">appleIdDisabled</span></span>|<span data-ttu-id="f03d3-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-185">Boolean</span></span>|<span data-ttu-id="f03d3-186">Indica se o Apple painel de configuração de id estará desabilitada Inherited de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-186">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-187">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-187">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f03d3-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-188">Boolean</span></span>|<span data-ttu-id="f03d3-189">Indica se o painel de configuração de 'Termos e condições' está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-189">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-190">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-190">touchIdDisabled</span></span>|<span data-ttu-id="f03d3-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-191">Boolean</span></span>|<span data-ttu-id="f03d3-192">Indica se o painel de configuração de id de toque está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-192">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-193">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-193">applePayDisabled</span></span>|<span data-ttu-id="f03d3-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-194">Boolean</span></span>|<span data-ttu-id="f03d3-195">Indica se o painel de configuração de pagamento do Apple está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-195">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-196">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-196">zoomDisabled</span></span>|<span data-ttu-id="f03d3-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-197">Boolean</span></span>|<span data-ttu-id="f03d3-198">Indica se o painel de configuração de zoom está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-198">Indicates if zoom setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-199">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-199">siriDisabled</span></span>|<span data-ttu-id="f03d3-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-200">Boolean</span></span>|<span data-ttu-id="f03d3-201">Indica se o painel de configuração de siri está desabilitado herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-201">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-202">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-202">diagnosticsDisabled</span></span>|<span data-ttu-id="f03d3-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-203">Boolean</span></span>|<span data-ttu-id="f03d3-204">Indica se o diagnóstico do painel de instalação está desabilitada Inherited em [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-204">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-205">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-205">displayToneSetupDisabled</span></span>|<span data-ttu-id="f03d3-206">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-206">Boolean</span></span>|<span data-ttu-id="f03d3-207">Indica se a tela de instalação do displaytone está desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-207">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-208">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-208">privacyPaneDisabled</span></span>|<span data-ttu-id="f03d3-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-209">Boolean</span></span>|<span data-ttu-id="f03d3-210">Indica se a tela de privacidade está desabilitada herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f03d3-210">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="f03d3-211">registrationDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-211">registrationDisabled</span></span>|<span data-ttu-id="f03d3-212">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-212">Boolean</span></span>|<span data-ttu-id="f03d3-213">Indica se o registro está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f03d3-213">Indicates if registration is disabled</span></span>|
|<span data-ttu-id="f03d3-214">fileVaultDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-214">fileVaultDisabled</span></span>|<span data-ttu-id="f03d3-215">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-215">Boolean</span></span>|<span data-ttu-id="f03d3-216">Indica se o armazenamento de arquivo está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f03d3-216">Indicates if file vault is disabled</span></span>|
|<span data-ttu-id="f03d3-217">iCloudDiagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f03d3-217">iCloudDiagnosticsDisabled</span></span>|<span data-ttu-id="f03d3-218">Boolean</span><span class="sxs-lookup"><span data-stu-id="f03d3-218">Boolean</span></span>|<span data-ttu-id="f03d3-219">Indica se a tela de análise de iCloud está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f03d3-219">Indicates if iCloud Analytics screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="f03d3-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="f03d3-220">Response</span></span>
<span data-ttu-id="f03d3-221">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f03d3-221">If successful, this method returns a `200 OK` response code and an updated [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f03d3-222">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f03d3-222">Example</span></span>

### <a name="request"></a><span data-ttu-id="f03d3-223">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f03d3-223">Request</span></span>
<span data-ttu-id="f03d3-224">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f03d3-224">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
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

### <a name="response"></a><span data-ttu-id="f03d3-225">Resposta</span><span class="sxs-lookup"><span data-stu-id="f03d3-225">Response</span></span>
<span data-ttu-id="f03d3-p105">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f03d3-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




