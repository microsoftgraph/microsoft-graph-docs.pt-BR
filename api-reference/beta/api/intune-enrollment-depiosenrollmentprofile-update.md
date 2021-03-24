---
title: Atualizar depIOSEnrollmentProfile
description: Atualize as propriedades de um objeto depIOSEnrollmentProfile.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6052f3896e6f9311034b1ea2efcb0e1f084cb18a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135786"
---
# <a name="update-depiosenrollmentprofile"></a><span data-ttu-id="86585-103">Atualizar depIOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="86585-103">Update depIOSEnrollmentProfile</span></span>

<span data-ttu-id="86585-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="86585-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="86585-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="86585-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="86585-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="86585-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="86585-107">Atualize as propriedades de [um objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-107">Update the properties of a [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="86585-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="86585-108">Prerequisites</span></span>
<span data-ttu-id="86585-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="86585-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="86585-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="86585-111">Permission type</span></span>|<span data-ttu-id="86585-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="86585-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="86585-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="86585-113">Delegated (work or school account)</span></span>|<span data-ttu-id="86585-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86585-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="86585-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="86585-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="86585-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="86585-116">Not supported.</span></span>|
|<span data-ttu-id="86585-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="86585-117">Application</span></span>|<span data-ttu-id="86585-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="86585-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="86585-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="86585-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultIosEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="86585-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="86585-120">Request headers</span></span>
|<span data-ttu-id="86585-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="86585-121">Header</span></span>|<span data-ttu-id="86585-122">Valor</span><span class="sxs-lookup"><span data-stu-id="86585-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="86585-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="86585-123">Authorization</span></span>|<span data-ttu-id="86585-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="86585-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="86585-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="86585-125">Accept</span></span>|<span data-ttu-id="86585-126">application/json</span><span class="sxs-lookup"><span data-stu-id="86585-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="86585-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="86585-127">Request body</span></span>
<span data-ttu-id="86585-128">No corpo da solicitação, fornece uma representação JSON para o [objeto depIOSEnrollmentProfile.](../resources/intune-enrollment-depiosenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-128">In the request body, supply a JSON representation for the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object.</span></span>

<span data-ttu-id="86585-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [o depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="86585-129">The following table shows the properties that are required when you create the [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md).</span></span>

|<span data-ttu-id="86585-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="86585-130">Property</span></span>|<span data-ttu-id="86585-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="86585-131">Type</span></span>|<span data-ttu-id="86585-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="86585-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="86585-133">id</span><span class="sxs-lookup"><span data-stu-id="86585-133">id</span></span>|<span data-ttu-id="86585-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-134">String</span></span>|<span data-ttu-id="86585-135">O GUID do objeto Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-135">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-136">displayName</span><span class="sxs-lookup"><span data-stu-id="86585-136">displayName</span></span>|<span data-ttu-id="86585-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-137">String</span></span>|<span data-ttu-id="86585-138">Nome do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-138">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-139">descrição</span><span class="sxs-lookup"><span data-stu-id="86585-139">description</span></span>|<span data-ttu-id="86585-140">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-140">String</span></span>|<span data-ttu-id="86585-141">Descrição do perfil Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-141">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-142">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="86585-142">requiresUserAuthentication</span></span>|<span data-ttu-id="86585-143">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-143">Boolean</span></span>|<span data-ttu-id="86585-144">Indica se o perfil requer autenticação de usuário Herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-144">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-145">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="86585-145">configurationEndpointUrl</span></span>|<span data-ttu-id="86585-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-146">String</span></span>|<span data-ttu-id="86585-147">URL do ponto de extremidade de configuração a ser usada para Registro Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-147">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-148">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="86585-148">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="86585-149">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-149">Boolean</span></span>|<span data-ttu-id="86585-150">Indica a autenticação com o Assistente de Instalação da Apple em vez do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="86585-150">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="86585-151">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-151">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="86585-152">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="86585-153">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-153">Boolean</span></span>|<span data-ttu-id="86585-154">Indica que o Portal da Empresa é necessário em dispositivos inscritos pelo assistente de instalação Herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-154">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="86585-155">isDefault</span><span class="sxs-lookup"><span data-stu-id="86585-155">isDefault</span></span>|<span data-ttu-id="86585-156">Booliano</span><span class="sxs-lookup"><span data-stu-id="86585-156">Boolean</span></span>|<span data-ttu-id="86585-157">Indica se esse é o perfil padrão Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-157">Indicates if this is the default profile Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-158">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="86585-158">supervisedModeEnabled</span></span>|<span data-ttu-id="86585-159">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-159">Boolean</span></span>|<span data-ttu-id="86585-160">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="86585-160">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="86585-161">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="86585-161">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span> <span data-ttu-id="86585-162">Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-162">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-163">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="86585-163">supportDepartment</span></span>|<span data-ttu-id="86585-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-164">String</span></span>|<span data-ttu-id="86585-165">Informações do departamento de suporte Herdadas [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-165">Support department information Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-166">isMandatory</span><span class="sxs-lookup"><span data-stu-id="86585-166">isMandatory</span></span>|<span data-ttu-id="86585-167">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-167">Boolean</span></span>|<span data-ttu-id="86585-168">Indica se o perfil é obrigatório Herdado de [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-168">Indicates if the profile is mandatory Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-169">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-169">locationDisabled</span></span>|<span data-ttu-id="86585-170">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-170">Boolean</span></span>|<span data-ttu-id="86585-171">Indica se o painel de configuração do serviço de local está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-171">Indicates if Location service setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-172">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="86585-172">supportPhoneNumber</span></span>|<span data-ttu-id="86585-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-173">String</span></span>|<span data-ttu-id="86585-174">Número de telefone de suporte Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-174">Support phone number Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-175">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-175">profileRemovalDisabled</span></span>|<span data-ttu-id="86585-176">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-176">Boolean</span></span>|<span data-ttu-id="86585-177">Indica se a opção de remoção de perfil está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-177">Indicates if the profile removal option is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-178">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="86585-178">restoreBlocked</span></span>|<span data-ttu-id="86585-179">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-179">Boolean</span></span>|<span data-ttu-id="86585-180">Indica se o painel restaurar instalação está bloqueado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-180">Indicates if Restore setup pane is blocked Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-181">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-181">appleIdDisabled</span></span>|<span data-ttu-id="86585-182">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-182">Boolean</span></span>|<span data-ttu-id="86585-183">Indica se o painel de configuração de ID da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-183">Indicates if Apple id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-184">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-184">termsAndConditionsDisabled</span></span>|<span data-ttu-id="86585-185">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-185">Boolean</span></span>|<span data-ttu-id="86585-186">Indica se o painel de configuração 'Termos e Condições' está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-186">Indicates if 'Terms and Conditions' setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-187">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-187">touchIdDisabled</span></span>|<span data-ttu-id="86585-188">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-188">Boolean</span></span>|<span data-ttu-id="86585-189">Indica se o painel de configuração de id por toque está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-189">Indicates if touch id setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-190">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-190">applePayDisabled</span></span>|<span data-ttu-id="86585-191">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-191">Boolean</span></span>|<span data-ttu-id="86585-192">Indica se o painel de configuração de pagamento da Apple está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-192">Indicates if Apple pay setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-193">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-193">siriDisabled</span></span>|<span data-ttu-id="86585-194">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-194">Boolean</span></span>|<span data-ttu-id="86585-195">Indica se o painel de configuração de siri está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-195">Indicates if siri setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-196">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-196">diagnosticsDisabled</span></span>|<span data-ttu-id="86585-197">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-197">Boolean</span></span>|<span data-ttu-id="86585-198">Indica se o painel de configuração de diagnósticos está desabilitado Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-198">Indicates if diagnostics setup pane is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-199">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-199">displayToneSetupDisabled</span></span>|<span data-ttu-id="86585-200">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-200">Boolean</span></span>|<span data-ttu-id="86585-201">Indica se a tela de instalação de displaytone está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-201">Indicates if displaytone setup screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-202">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-202">privacyPaneDisabled</span></span>|<span data-ttu-id="86585-203">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-203">Boolean</span></span>|<span data-ttu-id="86585-204">Indica se a tela de privacidade está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-204">Indicates if privacy screen is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-205">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-205">screenTimeScreenDisabled</span></span>|<span data-ttu-id="86585-206">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-206">Boolean</span></span>|<span data-ttu-id="86585-207">Indica se a configuração do tempo de tempo de tela está desabilitada Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-207">Indicates if screen timeout setup is disabled Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-208">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="86585-208">deviceNameTemplate</span></span>|<span data-ttu-id="86585-209">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-209">String</span></span>|<span data-ttu-id="86585-210">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="86585-210">Sets a literal or name pattern.</span></span> <span data-ttu-id="86585-211">Herdado [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-211">Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-212">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="86585-212">configurationWebUrl</span></span>|<span data-ttu-id="86585-213">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-213">Boolean</span></span>|<span data-ttu-id="86585-214">URL para logon do assistente de instalação Herdada [de depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="86585-214">URL for setup assistant login Inherited from [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span></span>|
|<span data-ttu-id="86585-215">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="86585-215">iTunesPairingMode</span></span>|[<span data-ttu-id="86585-216">iTunesPairingMode</span><span class="sxs-lookup"><span data-stu-id="86585-216">iTunesPairingMode</span></span>](../resources/intune-enrollment-itunespairingmode.md)|<span data-ttu-id="86585-217">Indica o modo de emparelhamento do iTunes.</span><span class="sxs-lookup"><span data-stu-id="86585-217">Indicates the iTunes pairing mode.</span></span> <span data-ttu-id="86585-218">Os valores possíveis são: `disallow`, `allow`, `requiresCertificate`.</span><span class="sxs-lookup"><span data-stu-id="86585-218">Possible values are: `disallow`, `allow`, `requiresCertificate`.</span></span>|
|<span data-ttu-id="86585-219">managementCertificates</span><span class="sxs-lookup"><span data-stu-id="86585-219">managementCertificates</span></span>|<span data-ttu-id="86585-220">[coleção managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md)</span><span class="sxs-lookup"><span data-stu-id="86585-220">[managementCertificateWithThumbprint](../resources/intune-enrollment-managementcertificatewiththumbprint.md) collection</span></span>|<span data-ttu-id="86585-221">Certificados de gerenciamento para o Apple Configurator</span><span class="sxs-lookup"><span data-stu-id="86585-221">Management certificates for Apple Configurator</span></span>|
|<span data-ttu-id="86585-222">restoreFromAndroidDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-222">restoreFromAndroidDisabled</span></span>|<span data-ttu-id="86585-223">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-223">Boolean</span></span>|<span data-ttu-id="86585-224">Indica se a restauração do Android está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-224">Indicates if Restore from Android is disabled</span></span>|
|<span data-ttu-id="86585-225">awaitDeviceConfiguredConfirmation</span><span class="sxs-lookup"><span data-stu-id="86585-225">awaitDeviceConfiguredConfirmation</span></span>|<span data-ttu-id="86585-226">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-226">Boolean</span></span>|<span data-ttu-id="86585-227">Indica se o dispositivo precisará aguardar a confirmação configurada</span><span class="sxs-lookup"><span data-stu-id="86585-227">Indicates if the device will need to wait for configured confirmation</span></span>|
|<span data-ttu-id="86585-228">sharedIPadMaximumUserCount</span><span class="sxs-lookup"><span data-stu-id="86585-228">sharedIPadMaximumUserCount</span></span>|<span data-ttu-id="86585-229">Int32</span><span class="sxs-lookup"><span data-stu-id="86585-229">Int32</span></span>|<span data-ttu-id="86585-230">Isso especifica o número máximo de usuários que podem usar um iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="86585-230">This specifies the maximum number of users that can use a shared iPad.</span></span> <span data-ttu-id="86585-231">Aplicável somente no modo iPad compartilhado.</span><span class="sxs-lookup"><span data-stu-id="86585-231">Only applicable in shared iPad mode.</span></span>|
|<span data-ttu-id="86585-232">enableSharedIPad</span><span class="sxs-lookup"><span data-stu-id="86585-232">enableSharedIPad</span></span>|<span data-ttu-id="86585-233">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-233">Boolean</span></span>|<span data-ttu-id="86585-234">Isso indica se o dispositivo deve ser inscrito em um modo que habilita cenários de vários usuários.</span><span class="sxs-lookup"><span data-stu-id="86585-234">This indicates whether the device is to be enrolled in a mode which enables multi user scenarios.</span></span> <span data-ttu-id="86585-235">Aplicável somente em iPads compartilhados.</span><span class="sxs-lookup"><span data-stu-id="86585-235">Only applicable in shared iPads.</span></span>|
|<span data-ttu-id="86585-236">companyPortalVppTokenId</span><span class="sxs-lookup"><span data-stu-id="86585-236">companyPortalVppTokenId</span></span>|<span data-ttu-id="86585-237">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="86585-237">String</span></span>|<span data-ttu-id="86585-238">Se definido, indica qual token Vpp deve ser usado para implantar o licenciamento de dispositivo do Portal da Empresa.</span><span class="sxs-lookup"><span data-stu-id="86585-238">If set, indicates which Vpp token should be used to deploy the Company Portal w/ device licensing.</span></span> <span data-ttu-id="86585-239">'enableAuthenticationViaCompanyPortal' deve ser definido para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="86585-239">'enableAuthenticationViaCompanyPortal' must be set in order for this property to be set.</span></span>|
|<span data-ttu-id="86585-240">enableSingleAppEnrollmentMode</span><span class="sxs-lookup"><span data-stu-id="86585-240">enableSingleAppEnrollmentMode</span></span>|<span data-ttu-id="86585-241">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-241">Boolean</span></span>|<span data-ttu-id="86585-242">Informa ao dispositivo para habilitar o modo de aplicativo único e aplicar o bloqueio de aplicativo durante o registro.</span><span class="sxs-lookup"><span data-stu-id="86585-242">Tells the device to enable single app mode and apply app-lock during enrollment.</span></span> <span data-ttu-id="86585-243">O padrão é false.</span><span class="sxs-lookup"><span data-stu-id="86585-243">Default is false.</span></span> <span data-ttu-id="86585-244">'enableAuthenticationViaCompanyPortal' e 'companyPortalVppTokenId' devem ser definidos para que essa propriedade seja definida.</span><span class="sxs-lookup"><span data-stu-id="86585-244">'enableAuthenticationViaCompanyPortal' and 'companyPortalVppTokenId' must be set for this property to be set.</span></span>|
|<span data-ttu-id="86585-245">homeButtonScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-245">homeButtonScreenDisabled</span></span>|<span data-ttu-id="86585-246">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-246">Boolean</span></span>|<span data-ttu-id="86585-247">Indica se a tela de sensibilidade do botão inicial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-247">Indicates if home button sensitivity screen is disabled</span></span>|
|<span data-ttu-id="86585-248">iMessageAndFaceTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-248">iMessageAndFaceTimeScreenDisabled</span></span>|<span data-ttu-id="86585-249">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-249">Boolean</span></span>|<span data-ttu-id="86585-250">Indica se a tela iMessage e FaceTime está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-250">Indicates if iMessage and FaceTime screen is disabled</span></span>|
|<span data-ttu-id="86585-251">onBoardingScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-251">onBoardingScreenDisabled</span></span>|<span data-ttu-id="86585-252">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-252">Boolean</span></span>|<span data-ttu-id="86585-253">Indica se a tela de instalação de integração está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-253">Indicates if onboarding setup screen is disabled</span></span>|
|<span data-ttu-id="86585-254">simSetupScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-254">simSetupScreenDisabled</span></span>|<span data-ttu-id="86585-255">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-255">Boolean</span></span>|<span data-ttu-id="86585-256">Indica se a tela SIMSetup está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-256">Indicates if the SIMSetup screen is disabled</span></span>|
|<span data-ttu-id="86585-257">softwareUpdateScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-257">softwareUpdateScreenDisabled</span></span>|<span data-ttu-id="86585-258">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-258">Boolean</span></span>|<span data-ttu-id="86585-259">Indica se a tela de atualização de sofware obrigatória está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-259">Indicates if the mandatory sofware update screen is disabled</span></span>|
|<span data-ttu-id="86585-260">watchMigrationScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-260">watchMigrationScreenDisabled</span></span>|<span data-ttu-id="86585-261">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-261">Boolean</span></span>|<span data-ttu-id="86585-262">Indica se a tela de migração do relógio está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-262">Indicates if the watch migration screen is disabled</span></span>|
|<span data-ttu-id="86585-263">appearanceScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-263">appearanceScreenDisabled</span></span>|<span data-ttu-id="86585-264">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-264">Boolean</span></span>|<span data-ttu-id="86585-265">Indica se a tela do Apperance está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-265">Indicates if Apperance screen is disabled</span></span>|
|<span data-ttu-id="86585-266">expressLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-266">expressLanguageScreenDisabled</span></span>|<span data-ttu-id="86585-267">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-267">Boolean</span></span>|<span data-ttu-id="86585-268">Indica se a tela linguagem expressa está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-268">Indicates if Express Language screen is disabled</span></span>|
|<span data-ttu-id="86585-269">preferredLanguageScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-269">preferredLanguageScreenDisabled</span></span>|<span data-ttu-id="86585-270">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-270">Boolean</span></span>|<span data-ttu-id="86585-271">Indica se a tela de idioma preferencial está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-271">Indicates if Preferred language screen is disabled</span></span>|
|<span data-ttu-id="86585-272">deviceToDeviceMigrationDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-272">deviceToDeviceMigrationDisabled</span></span>|<span data-ttu-id="86585-273">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-273">Boolean</span></span>|<span data-ttu-id="86585-274">Indica se a migração de dispositivo para dispositivo está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-274">Indicates if Device To Device Migration is disabled</span></span>|
|<span data-ttu-id="86585-275">welcomeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-275">welcomeScreenDisabled</span></span>|<span data-ttu-id="86585-276">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-276">Boolean</span></span>|<span data-ttu-id="86585-277">Indica se a tela Weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-277">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="86585-278">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-278">passCodeDisabled</span></span>|<span data-ttu-id="86585-279">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-279">Boolean</span></span>|<span data-ttu-id="86585-280">Indica se o painel de configuração senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="86585-280">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="86585-281">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-281">zoomDisabled</span></span>|<span data-ttu-id="86585-282">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-282">Boolean</span></span>|<span data-ttu-id="86585-283">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="86585-283">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="86585-284">restoreCompletedScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-284">restoreCompletedScreenDisabled</span></span>|<span data-ttu-id="86585-285">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-285">Boolean</span></span>|<span data-ttu-id="86585-286">Indica se a tela Weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-286">Indicates if Weclome screen is disabled</span></span>|
|<span data-ttu-id="86585-287">updateCompleteScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="86585-287">updateCompleteScreenDisabled</span></span>|<span data-ttu-id="86585-288">Booleano</span><span class="sxs-lookup"><span data-stu-id="86585-288">Boolean</span></span>|<span data-ttu-id="86585-289">Indica se a tela Weclome está desabilitada</span><span class="sxs-lookup"><span data-stu-id="86585-289">Indicates if Weclome screen is disabled</span></span>|



## <a name="response"></a><span data-ttu-id="86585-290">Resposta</span><span class="sxs-lookup"><span data-stu-id="86585-290">Response</span></span>
<span data-ttu-id="86585-291">Se tiver êxito, este método retornará um código de resposta e um objeto `200 OK` [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="86585-291">If successful, this method returns a `200 OK` response code and an updated [depIOSEnrollmentProfile](../resources/intune-enrollment-depiosenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="86585-292">Exemplo</span><span class="sxs-lookup"><span data-stu-id="86585-292">Example</span></span>

### <a name="request"></a><span data-ttu-id="86585-293">Solicitação</span><span class="sxs-lookup"><span data-stu-id="86585-293">Request</span></span>
<span data-ttu-id="86585-294">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="86585-294">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="86585-295">Resposta</span><span class="sxs-lookup"><span data-stu-id="86585-295">Response</span></span>
<span data-ttu-id="86585-p110">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="86585-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




