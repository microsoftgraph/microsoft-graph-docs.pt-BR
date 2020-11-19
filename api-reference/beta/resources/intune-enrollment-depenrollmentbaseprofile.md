---
title: tipo de recurso depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple. Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ed24aabc0f19ee6f9554a6d594c3095dcd4e3729
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49207432"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="f3cb4-104">tipo de recurso depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f3cb4-104">depEnrollmentBaseProfile resource type</span></span>

<span data-ttu-id="f3cb4-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f3cb4-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f3cb4-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3cb4-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3cb4-108">O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="f3cb4-109">Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="f3cb4-110">Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="f3cb4-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="f3cb4-111">Methods</span></span>
|<span data-ttu-id="f3cb4-112">Método</span><span class="sxs-lookup"><span data-stu-id="f3cb4-112">Method</span></span>|<span data-ttu-id="f3cb4-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f3cb4-113">Return Type</span></span>|<span data-ttu-id="f3cb4-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3cb4-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f3cb4-115">Listar depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="f3cb4-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="f3cb4-116">coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="f3cb4-117">Listar Propriedades e relações dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f3cb4-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="f3cb4-118">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f3cb4-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="f3cb4-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="f3cb4-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="f3cb4-120">Leia as propriedades e as relações do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="f3cb4-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f3cb4-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f3cb4-121">Properties</span></span>
|<span data-ttu-id="f3cb4-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f3cb4-122">Property</span></span>|<span data-ttu-id="f3cb4-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="f3cb4-123">Type</span></span>|<span data-ttu-id="f3cb4-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="f3cb4-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f3cb4-125">id</span><span class="sxs-lookup"><span data-stu-id="f3cb4-125">id</span></span>|<span data-ttu-id="f3cb4-126">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-126">String</span></span>|<span data-ttu-id="f3cb4-127">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-128">displayName</span><span class="sxs-lookup"><span data-stu-id="f3cb4-128">displayName</span></span>|<span data-ttu-id="f3cb4-129">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-129">String</span></span>|<span data-ttu-id="f3cb4-130">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-131">description</span><span class="sxs-lookup"><span data-stu-id="f3cb4-131">description</span></span>|<span data-ttu-id="f3cb4-132">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-132">String</span></span>|<span data-ttu-id="f3cb4-133">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="f3cb4-134">requiresUserAuthentication</span></span>|<span data-ttu-id="f3cb4-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-135">Boolean</span></span>|<span data-ttu-id="f3cb4-136">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="f3cb4-137">configurationEndpointUrl</span></span>|<span data-ttu-id="f3cb4-138">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-138">String</span></span>|<span data-ttu-id="f3cb4-139">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-140">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="f3cb4-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="f3cb4-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-141">Boolean</span></span>|<span data-ttu-id="f3cb4-142">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="f3cb4-143">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="f3cb4-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="f3cb4-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-145">Boolean</span></span>|<span data-ttu-id="f3cb4-146">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="f3cb4-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="f3cb4-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="f3cb4-147">isDefault</span></span>|<span data-ttu-id="f3cb4-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-148">Boolean</span></span>|<span data-ttu-id="f3cb4-149">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="f3cb4-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="f3cb4-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-150">supervisedModeEnabled</span></span>|<span data-ttu-id="f3cb4-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-151">Boolean</span></span>|<span data-ttu-id="f3cb4-152">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="f3cb4-153">Consulte https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-153">See https://docs.microsoft.com/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="f3cb4-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="f3cb4-154">supportDepartment</span></span>|<span data-ttu-id="f3cb4-155">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-155">String</span></span>|<span data-ttu-id="f3cb4-156">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="f3cb4-156">Support department information</span></span>|
|<span data-ttu-id="f3cb4-157">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="f3cb4-157">isMandatory</span></span>|<span data-ttu-id="f3cb4-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-158">Boolean</span></span>|<span data-ttu-id="f3cb4-159">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="f3cb4-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="f3cb4-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-160">locationDisabled</span></span>|<span data-ttu-id="f3cb4-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-161">Boolean</span></span>|<span data-ttu-id="f3cb4-162">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="f3cb4-163">supportPhoneNumber</span></span>|<span data-ttu-id="f3cb4-164">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-164">String</span></span>|<span data-ttu-id="f3cb4-165">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="f3cb4-165">Support phone number</span></span>|
|<span data-ttu-id="f3cb4-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-166">profileRemovalDisabled</span></span>|<span data-ttu-id="f3cb4-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-167">Boolean</span></span>|<span data-ttu-id="f3cb4-168">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f3cb4-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="f3cb4-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="f3cb4-169">restoreBlocked</span></span>|<span data-ttu-id="f3cb4-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-170">Boolean</span></span>|<span data-ttu-id="f3cb4-171">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="f3cb4-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-172">appleIdDisabled</span></span>|<span data-ttu-id="f3cb4-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-173">Boolean</span></span>|<span data-ttu-id="f3cb4-174">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="f3cb4-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-176">Boolean</span></span>|<span data-ttu-id="f3cb4-177">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-178">touchIdDisabled</span></span>|<span data-ttu-id="f3cb4-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-179">Boolean</span></span>|<span data-ttu-id="f3cb4-180">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-181">applePayDisabled</span></span>|<span data-ttu-id="f3cb4-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-182">Boolean</span></span>|<span data-ttu-id="f3cb4-183">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-184">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-184">siriDisabled</span></span>|<span data-ttu-id="f3cb4-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-185">Boolean</span></span>|<span data-ttu-id="f3cb4-186">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-186">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-187">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-187">diagnosticsDisabled</span></span>|<span data-ttu-id="f3cb4-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-188">Boolean</span></span>|<span data-ttu-id="f3cb4-189">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="f3cb4-189">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="f3cb4-190">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-190">displayToneSetupDisabled</span></span>|<span data-ttu-id="f3cb4-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-191">Boolean</span></span>|<span data-ttu-id="f3cb4-192">Indica se a tela de configuração do displaytone está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f3cb4-192">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="f3cb4-193">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-193">privacyPaneDisabled</span></span>|<span data-ttu-id="f3cb4-194">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-194">Boolean</span></span>|<span data-ttu-id="f3cb4-195">Indica se a tela de privacidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f3cb4-195">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="f3cb4-196">screenTimeScreenDisabled</span><span class="sxs-lookup"><span data-stu-id="f3cb4-196">screenTimeScreenDisabled</span></span>|<span data-ttu-id="f3cb4-197">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-197">Boolean</span></span>|<span data-ttu-id="f3cb4-198">Indica se a configuração de tempo limite da tela está desabilitada</span><span class="sxs-lookup"><span data-stu-id="f3cb4-198">Indicates if screen timeout setup is disabled</span></span>|
|<span data-ttu-id="f3cb4-199">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="f3cb4-199">deviceNameTemplate</span></span>|<span data-ttu-id="f3cb4-200">String</span><span class="sxs-lookup"><span data-stu-id="f3cb4-200">String</span></span>|<span data-ttu-id="f3cb4-201">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-201">Sets a literal or name pattern.</span></span>|
|<span data-ttu-id="f3cb4-202">configurationWebUrl</span><span class="sxs-lookup"><span data-stu-id="f3cb4-202">configurationWebUrl</span></span>|<span data-ttu-id="f3cb4-203">Booliano</span><span class="sxs-lookup"><span data-stu-id="f3cb4-203">Boolean</span></span>|<span data-ttu-id="f3cb4-204">URL para o logon do assistente de configuração</span><span class="sxs-lookup"><span data-stu-id="f3cb4-204">URL for setup assistant login</span></span>|

## <a name="relationships"></a><span data-ttu-id="f3cb4-205">Relações</span><span class="sxs-lookup"><span data-stu-id="f3cb4-205">Relationships</span></span>
<span data-ttu-id="f3cb4-206">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f3cb4-206">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f3cb4-207">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f3cb4-207">JSON Representation</span></span>
<span data-ttu-id="f3cb4-208">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f3cb4-208">Here is a JSON representation of the resource.</span></span>
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
  "isMandatory": true,
  "locationDisabled": true,
  "supportPhoneNumber": "String",
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
  "deviceNameTemplate": "String",
  "configurationWebUrl": true
}
```




