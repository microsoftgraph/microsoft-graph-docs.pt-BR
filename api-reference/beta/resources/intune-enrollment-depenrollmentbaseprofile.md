---
title: tipo de recurso de depEnrollmentBaseProfile
description: O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f8b820959e5515a575e4f074a2762794a15e7f5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423752"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="190c7-104">tipo de recurso de depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="190c7-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="190c7-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="190c7-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="190c7-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="190c7-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="190c7-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="190c7-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="190c7-108">O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="190c7-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="190c7-109">Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.</span><span class="sxs-lookup"><span data-stu-id="190c7-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>


<span data-ttu-id="190c7-110">Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="190c7-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="190c7-111">Methods</span></span>
|<span data-ttu-id="190c7-112">Método</span><span class="sxs-lookup"><span data-stu-id="190c7-112">Method</span></span>|<span data-ttu-id="190c7-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="190c7-113">Return Type</span></span>|<span data-ttu-id="190c7-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="190c7-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="190c7-115">Lista depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="190c7-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="190c7-116">coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="190c7-117">Lista as propriedades e os relacionamentos dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="190c7-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="190c7-118">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="190c7-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="190c7-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="190c7-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="190c7-120">Leia as propriedades e os relacionamentos do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="190c7-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="190c7-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="190c7-121">Properties</span></span>
|<span data-ttu-id="190c7-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="190c7-122">Property</span></span>|<span data-ttu-id="190c7-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="190c7-123">Type</span></span>|<span data-ttu-id="190c7-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="190c7-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="190c7-125">id</span><span class="sxs-lookup"><span data-stu-id="190c7-125">id</span></span>|<span data-ttu-id="190c7-126">String</span><span class="sxs-lookup"><span data-stu-id="190c7-126">String</span></span>|<span data-ttu-id="190c7-127">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-128">displayName</span><span class="sxs-lookup"><span data-stu-id="190c7-128">displayName</span></span>|<span data-ttu-id="190c7-129">String</span><span class="sxs-lookup"><span data-stu-id="190c7-129">String</span></span>|<span data-ttu-id="190c7-130">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-131">description</span><span class="sxs-lookup"><span data-stu-id="190c7-131">description</span></span>|<span data-ttu-id="190c7-132">String</span><span class="sxs-lookup"><span data-stu-id="190c7-132">String</span></span>|<span data-ttu-id="190c7-133">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="190c7-134">requiresUserAuthentication</span></span>|<span data-ttu-id="190c7-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-135">Boolean</span></span>|<span data-ttu-id="190c7-136">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="190c7-137">configurationEndpointUrl</span></span>|<span data-ttu-id="190c7-138">String</span><span class="sxs-lookup"><span data-stu-id="190c7-138">String</span></span>|<span data-ttu-id="190c7-139">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="190c7-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="190c7-141">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-141">Boolean</span></span>|<span data-ttu-id="190c7-142">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="190c7-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="190c7-143">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="190c7-144">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="190c7-145">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-145">Boolean</span></span>|<span data-ttu-id="190c7-146">Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="190c7-146">Indicates that Company Portal is required on setup assistant enrolled devices Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="190c7-147">isDefault</span><span class="sxs-lookup"><span data-stu-id="190c7-147">isDefault</span></span>|<span data-ttu-id="190c7-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-148">Boolean</span></span>|<span data-ttu-id="190c7-149">Indica se esse é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="190c7-149">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="190c7-150">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="190c7-150">supervisedModeEnabled</span></span>|<span data-ttu-id="190c7-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-151">Boolean</span></span>|<span data-ttu-id="190c7-152">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="190c7-152">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="190c7-153">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="190c7-153">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="190c7-154">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="190c7-154">supportDepartment</span></span>|<span data-ttu-id="190c7-155">String</span><span class="sxs-lookup"><span data-stu-id="190c7-155">String</span></span>|<span data-ttu-id="190c7-156">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="190c7-156">Support department information</span></span>|
|<span data-ttu-id="190c7-157">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-157">passCodeDisabled</span></span>|<span data-ttu-id="190c7-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-158">Boolean</span></span>|<span data-ttu-id="190c7-159">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-159">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-160">isMandatory</span><span class="sxs-lookup"><span data-stu-id="190c7-160">isMandatory</span></span>|<span data-ttu-id="190c7-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-161">Boolean</span></span>|<span data-ttu-id="190c7-162">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="190c7-162">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="190c7-163">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-163">locationDisabled</span></span>|<span data-ttu-id="190c7-164">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-164">Boolean</span></span>|<span data-ttu-id="190c7-165">Indica se o painel de configuração do serviço local está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-165">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-166">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="190c7-166">supportPhoneNumber</span></span>|<span data-ttu-id="190c7-167">String</span><span class="sxs-lookup"><span data-stu-id="190c7-167">String</span></span>|<span data-ttu-id="190c7-168">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="190c7-168">Support phone number</span></span>|
|<span data-ttu-id="190c7-169">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-169">profileRemovalDisabled</span></span>|<span data-ttu-id="190c7-170">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-170">Boolean</span></span>|<span data-ttu-id="190c7-171">Indica se a opção de remoção do perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="190c7-171">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="190c7-172">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="190c7-172">restoreBlocked</span></span>|<span data-ttu-id="190c7-173">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-173">Boolean</span></span>|<span data-ttu-id="190c7-174">Indica se o painel de configuração de restauração será bloqueado</span><span class="sxs-lookup"><span data-stu-id="190c7-174">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="190c7-175">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-175">appleIdDisabled</span></span>|<span data-ttu-id="190c7-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-176">Boolean</span></span>|<span data-ttu-id="190c7-177">Indica se o painel de configuração de id do Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-177">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-178">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-178">termsAndConditionsDisabled</span></span>|<span data-ttu-id="190c7-179">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-179">Boolean</span></span>|<span data-ttu-id="190c7-180">Indica se o painel de configuração de 'Termos e condições' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-180">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-181">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-181">touchIdDisabled</span></span>|<span data-ttu-id="190c7-182">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-182">Boolean</span></span>|<span data-ttu-id="190c7-183">Indica se o painel de configuração de id de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-183">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-184">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-184">applePayDisabled</span></span>|<span data-ttu-id="190c7-185">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-185">Boolean</span></span>|<span data-ttu-id="190c7-186">Indica se o painel de configuração de pagamento do Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-186">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-187">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-187">zoomDisabled</span></span>|<span data-ttu-id="190c7-188">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-188">Boolean</span></span>|<span data-ttu-id="190c7-189">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-189">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-190">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-190">siriDisabled</span></span>|<span data-ttu-id="190c7-191">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-191">Boolean</span></span>|<span data-ttu-id="190c7-192">Indica se o painel de configuração de siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-192">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-193">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-193">diagnosticsDisabled</span></span>|<span data-ttu-id="190c7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-194">Boolean</span></span>|<span data-ttu-id="190c7-195">Indica se o painel de configuração de diagnósticos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="190c7-195">Indicates if diagnostics setup pane is disabled</span></span>|
|<span data-ttu-id="190c7-196">displayToneSetupDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-196">displayToneSetupDisabled</span></span>|<span data-ttu-id="190c7-197">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-197">Boolean</span></span>|<span data-ttu-id="190c7-198">Indica se a tela de instalação do displaytone está desabilitada</span><span class="sxs-lookup"><span data-stu-id="190c7-198">Indicates if displaytone setup screen is disabled</span></span>|
|<span data-ttu-id="190c7-199">privacyPaneDisabled</span><span class="sxs-lookup"><span data-stu-id="190c7-199">privacyPaneDisabled</span></span>|<span data-ttu-id="190c7-200">Boolean</span><span class="sxs-lookup"><span data-stu-id="190c7-200">Boolean</span></span>|<span data-ttu-id="190c7-201">Indica se a tela de privacidade está desabilitada</span><span class="sxs-lookup"><span data-stu-id="190c7-201">Indicates if privacy screen is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="190c7-202">Relações</span><span class="sxs-lookup"><span data-stu-id="190c7-202">Relationships</span></span>
<span data-ttu-id="190c7-203">Nenhum</span><span class="sxs-lookup"><span data-stu-id="190c7-203">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="190c7-204">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="190c7-204">JSON Representation</span></span>
<span data-ttu-id="190c7-205">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="190c7-205">Here is a JSON representation of the resource.</span></span>
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
  "privacyPaneDisabled": true
}
```




