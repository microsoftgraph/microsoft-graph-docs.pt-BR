---
title: tipo de recurso depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple. Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0b3845b693dcc3030e8e24062d496b4c1fb19bcd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524763"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="ce6be-104">tipo de recurso depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="ce6be-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="ce6be-105">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="ce6be-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ce6be-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ce6be-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ce6be-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ce6be-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ce6be-108">O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple.</span><span class="sxs-lookup"><span data-stu-id="ce6be-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="ce6be-109">Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.</span><span class="sxs-lookup"><span data-stu-id="ce6be-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="ce6be-110">Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="ce6be-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="ce6be-111">Methods</span></span>
|<span data-ttu-id="ce6be-112">Método</span><span class="sxs-lookup"><span data-stu-id="ce6be-112">Method</span></span>|<span data-ttu-id="ce6be-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="ce6be-113">Return Type</span></span>|<span data-ttu-id="ce6be-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce6be-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="ce6be-115">Listar depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="ce6be-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="ce6be-116">coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="ce6be-117">Listar Propriedades e relações dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ce6be-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="ce6be-118">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="ce6be-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="ce6be-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="ce6be-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="ce6be-120">Leia as propriedades e as relações do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="ce6be-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="ce6be-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ce6be-121">Properties</span></span>
|<span data-ttu-id="ce6be-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ce6be-122">Property</span></span>|<span data-ttu-id="ce6be-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="ce6be-123">Type</span></span>|<span data-ttu-id="ce6be-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="ce6be-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ce6be-125">id</span><span class="sxs-lookup"><span data-stu-id="ce6be-125">id</span></span>|<span data-ttu-id="ce6be-126">String</span><span class="sxs-lookup"><span data-stu-id="ce6be-126">String</span></span>|<span data-ttu-id="ce6be-127">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-128">displayName</span><span class="sxs-lookup"><span data-stu-id="ce6be-128">displayName</span></span>|<span data-ttu-id="ce6be-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ce6be-129">String</span></span>|<span data-ttu-id="ce6be-130">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-131">description</span><span class="sxs-lookup"><span data-stu-id="ce6be-131">description</span></span>|<span data-ttu-id="ce6be-132">String</span><span class="sxs-lookup"><span data-stu-id="ce6be-132">String</span></span>|<span data-ttu-id="ce6be-133">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="ce6be-134">requiresUserAuthentication</span></span>|<span data-ttu-id="ce6be-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-135">Boolean</span></span>|<span data-ttu-id="ce6be-136">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="ce6be-137">configurationEndpointUrl</span></span>|<span data-ttu-id="ce6be-138">String</span><span class="sxs-lookup"><span data-stu-id="ce6be-138">String</span></span>|<span data-ttu-id="ce6be-139">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-140">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="ce6be-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="ce6be-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-141">Boolean</span></span>|<span data-ttu-id="ce6be-142">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="ce6be-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="ce6be-143">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="ce6be-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="ce6be-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-145">Boolean</span></span>|<span data-ttu-id="ce6be-146">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="ce6be-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="ce6be-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="ce6be-147">isDefault</span></span>|<span data-ttu-id="ce6be-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="ce6be-148">Boolean</span></span>|<span data-ttu-id="ce6be-149">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="ce6be-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="ce6be-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-150">supervisedModeEnabled</span></span>|<span data-ttu-id="ce6be-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-151">Boolean</span></span>|<span data-ttu-id="ce6be-152">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="ce6be-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="ce6be-153">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="ce6be-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="ce6be-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="ce6be-154">supportDepartment</span></span>|<span data-ttu-id="ce6be-155">String</span><span class="sxs-lookup"><span data-stu-id="ce6be-155">String</span></span>|<span data-ttu-id="ce6be-156">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="ce6be-156">Support department information</span></span>|
|<span data-ttu-id="ce6be-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-157">passCodeDisabled</span></span>|<span data-ttu-id="ce6be-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-158">Boolean</span></span>|<span data-ttu-id="ce6be-159">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-160">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="ce6be-160">isMandatory</span></span>|<span data-ttu-id="ce6be-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-161">Boolean</span></span>|<span data-ttu-id="ce6be-162">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="ce6be-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="ce6be-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-163">locationDisabled</span></span>|<span data-ttu-id="ce6be-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-164">Boolean</span></span>|<span data-ttu-id="ce6be-165">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="ce6be-166">supportPhoneNumber</span></span>|<span data-ttu-id="ce6be-167">String</span><span class="sxs-lookup"><span data-stu-id="ce6be-167">String</span></span>|<span data-ttu-id="ce6be-168">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="ce6be-168">Support phone number</span></span>|
|<span data-ttu-id="ce6be-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-169">profileRemovalDisabled</span></span>|<span data-ttu-id="ce6be-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-170">Boolean</span></span>|<span data-ttu-id="ce6be-171">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ce6be-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="ce6be-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="ce6be-172">restoreBlocked</span></span>|<span data-ttu-id="ce6be-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-173">Boolean</span></span>|<span data-ttu-id="ce6be-174">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="ce6be-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="ce6be-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-175">appleIdDisabled</span></span>|<span data-ttu-id="ce6be-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-176">Boolean</span></span>|<span data-ttu-id="ce6be-177">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="ce6be-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-179">Boolean</span></span>|<span data-ttu-id="ce6be-180">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-181">touchIdDisabled</span></span>|<span data-ttu-id="ce6be-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-182">Boolean</span></span>|<span data-ttu-id="ce6be-183">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-184">applePayDisabled</span></span>|<span data-ttu-id="ce6be-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-185">Boolean</span></span>|<span data-ttu-id="ce6be-186">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-187">zoomDisabled</span></span>|<span data-ttu-id="ce6be-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-188">Boolean</span></span>|<span data-ttu-id="ce6be-189">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-190">siriDisabled</span></span>|<span data-ttu-id="ce6be-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-191">Boolean</span></span>|<span data-ttu-id="ce6be-192">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-193">diagnosticsDisabled</span></span>|<span data-ttu-id="ce6be-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-194">Boolean</span></span>|<span data-ttu-id="ce6be-195">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="ce6be-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="ce6be-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="ce6be-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-197">Boolean</span></span>|<span data-ttu-id="ce6be-198">Indica se a tela de configuração do displaytone está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ce6be-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="ce6be-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-199">privacyPaneDisabled</span></span>|<span data-ttu-id="ce6be-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-200">Boolean</span></span>|<span data-ttu-id="ce6be-201">Indica se a tela de privacidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ce6be-201">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="ce6be-202">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="ce6be-202">screenTimeScreenDisabled</span></span>|<span data-ttu-id="ce6be-203">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-203">Boolean</span></span>|<span data-ttu-id="ce6be-204">Indica se a configuração de tempo limite da tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="ce6be-204">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="ce6be-205">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="ce6be-205">deviceNameTemplate</span></span>|<span data-ttu-id="ce6be-206">String</span><span class="sxs-lookup"><span data-stu-id="ce6be-206">String</span></span>|<span data-ttu-id="ce6be-207">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="ce6be-207">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="ce6be-208">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="ce6be-208">configurationWebUrl</span></span>|<span data-ttu-id="ce6be-209">Boolean</span><span class="sxs-lookup"><span data-stu-id="ce6be-209">Boolean</span></span>|<span data-ttu-id="ce6be-210">URL para o logon do assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="ce6be-210">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="ce6be-211">Relações</span><span class="sxs-lookup"><span data-stu-id="ce6be-211">Relationships</span></span>
<span data-ttu-id="ce6be-212">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ce6be-212">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ce6be-213">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ce6be-213">JSON Representation</span></span>
<span data-ttu-id="ce6be-214">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ce6be-214">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.depEnrollmentBaseProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.depEnrollmentBaseProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true,
  "isDefault": true,
  "supervisedModeEnabled": true,
  "supportDepartment": "String",
  "passCodeDisabled": true,
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```



