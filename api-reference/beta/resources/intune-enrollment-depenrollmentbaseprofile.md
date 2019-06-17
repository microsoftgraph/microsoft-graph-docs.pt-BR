---
title: tipo de recurso depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple. Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b92a86a3faa3da1af203e3688b7de7318a76dca4
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978910"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="200b3-104">tipo de recurso depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="200b3-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="200b3-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="200b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="200b3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="200b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="200b3-107">O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple.</span><span class="sxs-lookup"><span data-stu-id="200b3-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="200b3-108">Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.</span><span class="sxs-lookup"><span data-stu-id="200b3-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="200b3-109">Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="200b3-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="200b3-110">Methods</span></span>
|<span data-ttu-id="200b3-111">Método</span><span class="sxs-lookup"><span data-stu-id="200b3-111">Method</span></span>|<span data-ttu-id="200b3-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="200b3-112">Return Type</span></span>|<span data-ttu-id="200b3-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="200b3-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="200b3-114">Listar depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="200b3-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="200b3-115">coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="200b3-116">Listar Propriedades e relações dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="200b3-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="200b3-117">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="200b3-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="200b3-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="200b3-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="200b3-119">Leia as propriedades e as relações do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="200b3-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="200b3-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="200b3-120">Properties</span></span>
|<span data-ttu-id="200b3-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="200b3-121">Property</span></span>|<span data-ttu-id="200b3-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="200b3-122">Type</span></span>|<span data-ttu-id="200b3-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="200b3-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="200b3-124">id</span><span class="sxs-lookup"><span data-stu-id="200b3-124">id</span></span>|<span data-ttu-id="200b3-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="200b3-125">String</span></span>|<span data-ttu-id="200b3-126">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-127">displayName</span><span class="sxs-lookup"><span data-stu-id="200b3-127">displayName</span></span>|<span data-ttu-id="200b3-128">String</span><span class="sxs-lookup"><span data-stu-id="200b3-128">String</span></span>|<span data-ttu-id="200b3-129">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-130">descrição</span><span class="sxs-lookup"><span data-stu-id="200b3-130">description</span></span>|<span data-ttu-id="200b3-131">String</span><span class="sxs-lookup"><span data-stu-id="200b3-131">String</span></span>|<span data-ttu-id="200b3-132">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="200b3-133">requiresUserAuthentication</span></span>|<span data-ttu-id="200b3-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-134">Boolean</span></span>|<span data-ttu-id="200b3-135">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-136">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="200b3-136">configurationEndpointUrl</span></span>|<span data-ttu-id="200b3-137">String</span><span class="sxs-lookup"><span data-stu-id="200b3-137">String</span></span>|<span data-ttu-id="200b3-138">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-139">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="200b3-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="200b3-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-140">Boolean</span></span>|<span data-ttu-id="200b3-141">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="200b3-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="200b3-142">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="200b3-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="200b3-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-144">Boolean</span></span>|<span data-ttu-id="200b3-145">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="200b3-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="200b3-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="200b3-146">isDefault</span></span>|<span data-ttu-id="200b3-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-147">Boolean</span></span>|<span data-ttu-id="200b3-148">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="200b3-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="200b3-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="200b3-149">supervisedModeEnabled</span></span>|<span data-ttu-id="200b3-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-150">Boolean</span></span>|<span data-ttu-id="200b3-151">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="200b3-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="200b3-152">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="200b3-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="200b3-153">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="200b3-153">supportDepartment</span></span>|<span data-ttu-id="200b3-154">String</span><span class="sxs-lookup"><span data-stu-id="200b3-154">String</span></span>|<span data-ttu-id="200b3-155">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="200b3-155">Support department information</span></span>|
|<span data-ttu-id="200b3-156">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-156">passCodeDisabled</span></span>|<span data-ttu-id="200b3-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-157">Boolean</span></span>|<span data-ttu-id="200b3-158">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-159">IsMandatory</span><span class="sxs-lookup"><span data-stu-id="200b3-159">isMandatory</span></span>|<span data-ttu-id="200b3-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-160">Boolean</span></span>|<span data-ttu-id="200b3-161">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="200b3-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="200b3-162">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-162">locationDisabled</span></span>|<span data-ttu-id="200b3-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-163">Boolean</span></span>|<span data-ttu-id="200b3-164">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="200b3-165">supportPhoneNumber</span></span>|<span data-ttu-id="200b3-166">String</span><span class="sxs-lookup"><span data-stu-id="200b3-166">String</span></span>|<span data-ttu-id="200b3-167">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="200b3-167">Support phone number</span></span>|
|<span data-ttu-id="200b3-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-168">profileRemovalDisabled</span></span>|<span data-ttu-id="200b3-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-169">Boolean</span></span>|<span data-ttu-id="200b3-170">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="200b3-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="200b3-171">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="200b3-171">restoreBlocked</span></span>|<span data-ttu-id="200b3-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-172">Boolean</span></span>|<span data-ttu-id="200b3-173">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="200b3-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="200b3-174">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-174">appleIdDisabled</span></span>|<span data-ttu-id="200b3-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-175">Boolean</span></span>|<span data-ttu-id="200b3-176">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="200b3-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-178">Boolean</span></span>|<span data-ttu-id="200b3-179">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-180">touchIdDisabled</span></span>|<span data-ttu-id="200b3-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-181">Boolean</span></span>|<span data-ttu-id="200b3-182">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-183">applePayDisabled</span></span>|<span data-ttu-id="200b3-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-184">Boolean</span></span>|<span data-ttu-id="200b3-185">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-186">zoomDisabled</span></span>|<span data-ttu-id="200b3-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-187">Boolean</span></span>|<span data-ttu-id="200b3-188">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-189">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-189">siriDisabled</span></span>|<span data-ttu-id="200b3-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-190">Boolean</span></span>|<span data-ttu-id="200b3-191">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-192">diagnosticsDisabled</span></span>|<span data-ttu-id="200b3-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-193">Boolean</span></span>|<span data-ttu-id="200b3-194">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="200b3-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="200b3-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="200b3-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-196">Boolean</span></span>|<span data-ttu-id="200b3-197">Indica se a tela de configuração do displaytone está desabilitada</span><span class="sxs-lookup"><span data-stu-id="200b3-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="200b3-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="200b3-198">privacyPaneDisabled</span></span>|<span data-ttu-id="200b3-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="200b3-199">Boolean</span></span>|<span data-ttu-id="200b3-200">Indica se a tela de privacidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="200b3-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="200b3-201">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="200b3-201">deviceNameTemplate</span></span>|<span data-ttu-id="200b3-202">String</span><span class="sxs-lookup"><span data-stu-id="200b3-202">String</span></span>|<span data-ttu-id="200b3-203">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="200b3-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="200b3-204">Relações</span><span class="sxs-lookup"><span data-stu-id="200b3-204">Relationships</span></span>
<span data-ttu-id="200b3-205">Nenhum</span><span class="sxs-lookup"><span data-stu-id="200b3-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="200b3-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="200b3-206">JSON Representation</span></span>
<span data-ttu-id="200b3-207">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="200b3-207">Here is a JSON representation of the resource.</span></span>
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
  "deviceNameTemplate": "String"
}
```





