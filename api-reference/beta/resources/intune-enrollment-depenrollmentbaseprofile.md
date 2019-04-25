---
title: tipo de recurso depEnrollmentBaseProfile
description: O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple. Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 69f0bb3647e5d12d0d441f06e7436626b0d29334
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573911"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="eb8d5-104">tipo de recurso depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="eb8d5-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="eb8d5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eb8d5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eb8d5-107">O recurso DepEnrollmentBaseProfile representa um perfil de registro de programa de registro de dispositivo (DEP) Apple.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-107">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="eb8d5-108">Esse tipo de perfil deve ser atribuído aos números de série da Apple DEP antes que os dispositivos correspondentes possam se inscrever via DEP.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-108">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="eb8d5-109">Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-109">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="eb8d5-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="eb8d5-110">Methods</span></span>
|<span data-ttu-id="eb8d5-111">Método</span><span class="sxs-lookup"><span data-stu-id="eb8d5-111">Method</span></span>|<span data-ttu-id="eb8d5-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="eb8d5-112">Return Type</span></span>|<span data-ttu-id="eb8d5-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb8d5-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="eb8d5-114">Listar depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="eb8d5-114">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="eb8d5-115">coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-115">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="eb8d5-116">Listar Propriedades e relações dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="eb8d5-116">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="eb8d5-117">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="eb8d5-117">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="eb8d5-118">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="eb8d5-118">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="eb8d5-119">Leia as propriedades e as relações do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="eb8d5-119">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="eb8d5-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="eb8d5-120">Properties</span></span>
|<span data-ttu-id="eb8d5-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="eb8d5-121">Property</span></span>|<span data-ttu-id="eb8d5-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="eb8d5-122">Type</span></span>|<span data-ttu-id="eb8d5-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="eb8d5-123">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eb8d5-124">id</span><span class="sxs-lookup"><span data-stu-id="eb8d5-124">id</span></span>|<span data-ttu-id="eb8d5-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="eb8d5-125">String</span></span>|<span data-ttu-id="eb8d5-126">O GUID do objeto herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-126">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-127">displayName</span><span class="sxs-lookup"><span data-stu-id="eb8d5-127">displayName</span></span>|<span data-ttu-id="eb8d5-128">String</span><span class="sxs-lookup"><span data-stu-id="eb8d5-128">String</span></span>|<span data-ttu-id="eb8d5-129">Nome do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-129">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-130">description</span><span class="sxs-lookup"><span data-stu-id="eb8d5-130">description</span></span>|<span data-ttu-id="eb8d5-131">String</span><span class="sxs-lookup"><span data-stu-id="eb8d5-131">String</span></span>|<span data-ttu-id="eb8d5-132">Descrição do perfil herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-132">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-133">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="eb8d5-133">requiresUserAuthentication</span></span>|<span data-ttu-id="eb8d5-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-134">Boolean</span></span>|<span data-ttu-id="eb8d5-135">Indica se o perfil requer autenticação de usuário herdada de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-135">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-136">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="eb8d5-136">configurationEndpointUrl</span></span>|<span data-ttu-id="eb8d5-137">String</span><span class="sxs-lookup"><span data-stu-id="eb8d5-137">String</span></span>|<span data-ttu-id="eb8d5-138">URL de ponto de extremidade de configuração a ser usada para registro herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-138">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-139">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="eb8d5-139">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="eb8d5-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-140">Boolean</span></span>|<span data-ttu-id="eb8d5-141">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-141">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="eb8d5-142">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-142">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="eb8d5-143">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="eb8d5-144">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-144">Boolean</span></span>|<span data-ttu-id="eb8d5-145">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados herdados de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="eb8d5-145">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="eb8d5-146">isDefault</span><span class="sxs-lookup"><span data-stu-id="eb8d5-146">isDefault</span></span>|<span data-ttu-id="eb8d5-147">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-147">Boolean</span></span>|<span data-ttu-id="eb8d5-148">Indica se este é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="eb8d5-148">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="eb8d5-149">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-149">supervisedModeEnabled</span></span>|<span data-ttu-id="eb8d5-150">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-150">Boolean</span></span>|<span data-ttu-id="eb8d5-151">Modo supervisionado, true para habilitar, caso contrário, false.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-151">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="eb8d5-152">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-152">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="eb8d5-153">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="eb8d5-153">supportDepartment</span></span>|<span data-ttu-id="eb8d5-154">String</span><span class="sxs-lookup"><span data-stu-id="eb8d5-154">String</span></span>|<span data-ttu-id="eb8d5-155">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="eb8d5-155">Support department information</span></span>|
|<span data-ttu-id="eb8d5-156">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-156">passCodeDisabled</span></span>|<span data-ttu-id="eb8d5-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-157">Boolean</span></span>|<span data-ttu-id="eb8d5-158">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-158">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-159">isMandatory</span><span class="sxs-lookup"><span data-stu-id="eb8d5-159">isMandatory</span></span>|<span data-ttu-id="eb8d5-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-160">Boolean</span></span>|<span data-ttu-id="eb8d5-161">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="eb8d5-161">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="eb8d5-162">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-162">locationDisabled</span></span>|<span data-ttu-id="eb8d5-163">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-163">Boolean</span></span>|<span data-ttu-id="eb8d5-164">Indica se o painel de instalação do serviço de localização está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-164">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-165">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="eb8d5-165">supportPhoneNumber</span></span>|<span data-ttu-id="eb8d5-166">String</span><span class="sxs-lookup"><span data-stu-id="eb8d5-166">String</span></span>|<span data-ttu-id="eb8d5-167">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="eb8d5-167">Support phone number</span></span>|
|<span data-ttu-id="eb8d5-168">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-168">profileRemovalDisabled</span></span>|<span data-ttu-id="eb8d5-169">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-169">Boolean</span></span>|<span data-ttu-id="eb8d5-170">Indica se a opção de remoção de perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="eb8d5-170">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="eb8d5-171">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="eb8d5-171">restoreBlocked</span></span>|<span data-ttu-id="eb8d5-172">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-172">Boolean</span></span>|<span data-ttu-id="eb8d5-173">Indica se o painel de configuração de restauração está bloqueado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-173">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="eb8d5-174">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-174">appleIdDisabled</span></span>|<span data-ttu-id="eb8d5-175">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-175">Boolean</span></span>|<span data-ttu-id="eb8d5-176">Indica se o painel de configuração de ID da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-176">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-177">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-177">termsAndConditionsDisabled</span></span>|<span data-ttu-id="eb8d5-178">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-178">Boolean</span></span>|<span data-ttu-id="eb8d5-179">Indica se o painel de configuração ' termos e condições ' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-179">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-180">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-180">touchIdDisabled</span></span>|<span data-ttu-id="eb8d5-181">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-181">Boolean</span></span>|<span data-ttu-id="eb8d5-182">Indica se o painel de configuração de ID de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-182">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-183">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-183">applePayDisabled</span></span>|<span data-ttu-id="eb8d5-184">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-184">Boolean</span></span>|<span data-ttu-id="eb8d5-185">Indica se o painel de configuração de pagamento da Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-185">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-186">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-186">zoomDisabled</span></span>|<span data-ttu-id="eb8d5-187">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-187">Boolean</span></span>|<span data-ttu-id="eb8d5-188">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-188">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-189">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-189">siriDisabled</span></span>|<span data-ttu-id="eb8d5-190">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-190">Boolean</span></span>|<span data-ttu-id="eb8d5-191">Indica se o painel de configuração do Siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-191">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-192">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-192">diagnosticsDisabled</span></span>|<span data-ttu-id="eb8d5-193">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-193">Boolean</span></span>|<span data-ttu-id="eb8d5-194">Indica se o painel de configuração de diagnóstico está desabilitado</span><span class="sxs-lookup"><span data-stu-id="eb8d5-194">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="eb8d5-195">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-195">displayToneSetupDisabled</span></span>|<span data-ttu-id="eb8d5-196">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-196">Boolean</span></span>|<span data-ttu-id="eb8d5-197">Indica se a tela de configuração do displaytone está desabilitada</span><span class="sxs-lookup"><span data-stu-id="eb8d5-197">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="eb8d5-198">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="eb8d5-198">privacyPaneDisabled</span></span>|<span data-ttu-id="eb8d5-199">Booliano</span><span class="sxs-lookup"><span data-stu-id="eb8d5-199">Boolean</span></span>|<span data-ttu-id="eb8d5-200">Indica se a tela de privacidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="eb8d5-200">Indicates if privacy screen is disabled</span></span>|
|<span data-ttu-id="eb8d5-201">deviceNameTemplate</span><span class="sxs-lookup"><span data-stu-id="eb8d5-201">deviceNameTemplate</span></span>|<span data-ttu-id="eb8d5-202">String</span><span class="sxs-lookup"><span data-stu-id="eb8d5-202">String</span></span>|<span data-ttu-id="eb8d5-203">Define um padrão literal ou de nome.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-203">Sets a literal or name pattern.</span></span>|

## <a name="relationships"></a><span data-ttu-id="eb8d5-204">Relações</span><span class="sxs-lookup"><span data-stu-id="eb8d5-204">Relationships</span></span>
<span data-ttu-id="eb8d5-205">Nenhum</span><span class="sxs-lookup"><span data-stu-id="eb8d5-205">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb8d5-206">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="eb8d5-206">JSON Representation</span></span>
<span data-ttu-id="eb8d5-207">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="eb8d5-207">Here is a JSON representation of the resource.</span></span>
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





