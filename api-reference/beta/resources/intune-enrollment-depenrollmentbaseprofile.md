---
title: tipo de recurso de depEnrollmentBaseProfile
description: O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP). Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16baaef2413bbbc169ef8823dc9043245cdfad91
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27844356"
---
# <a name="depenrollmentbaseprofile-resource-type"></a><span data-ttu-id="437a3-104">tipo de recurso de depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="437a3-104">depEnrollmentBaseProfile resource type</span></span>

> <span data-ttu-id="437a3-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="437a3-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="437a3-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="437a3-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="437a3-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="437a3-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="437a3-108">O recurso de DepEnrollmentBaseProfile representa um perfil de inscrição do programa de inscrição de dispositivo da Apple (DEP).</span><span class="sxs-lookup"><span data-stu-id="437a3-108">The DepEnrollmentBaseProfile resource represents an Apple Device Enrollment Program (DEP) enrollment profile.</span></span> <span data-ttu-id="437a3-109">Esse tipo de perfil deve ser atribuído aos números de série do Apple DEP antes os dispositivos correspondentes podem registrar-se por meio do DEP.</span><span class="sxs-lookup"><span data-stu-id="437a3-109">This type of profile must be assigned to Apple DEP serial numbers before the corresponding devices can enroll via DEP.</span></span>

<span data-ttu-id="437a3-110">Herda de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-110">Inherits from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>

## <a name="methods"></a><span data-ttu-id="437a3-111">Métodos</span><span class="sxs-lookup"><span data-stu-id="437a3-111">Methods</span></span>
|<span data-ttu-id="437a3-112">Método</span><span class="sxs-lookup"><span data-stu-id="437a3-112">Method</span></span>|<span data-ttu-id="437a3-113">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="437a3-113">Return Type</span></span>|<span data-ttu-id="437a3-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="437a3-114">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="437a3-115">Lista depEnrollmentBaseProfiles</span><span class="sxs-lookup"><span data-stu-id="437a3-115">List depEnrollmentBaseProfiles</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-list.md)|<span data-ttu-id="437a3-116">coleção [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-116">[depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) collection</span></span>|<span data-ttu-id="437a3-117">Lista as propriedades e os relacionamentos dos objetos [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="437a3-117">List properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) objects.</span></span>|
|[<span data-ttu-id="437a3-118">Obter depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="437a3-118">Get depEnrollmentBaseProfile</span></span>](../api/intune-enrollment-depenrollmentbaseprofile-get.md)|[<span data-ttu-id="437a3-119">depEnrollmentBaseProfile</span><span class="sxs-lookup"><span data-stu-id="437a3-119">depEnrollmentBaseProfile</span></span>](../resources/intune-enrollment-depenrollmentbaseprofile.md)|<span data-ttu-id="437a3-120">Leia as propriedades e os relacionamentos do objeto [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="437a3-120">Read properties and relationships of the [depEnrollmentBaseProfile](../resources/intune-enrollment-depenrollmentbaseprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="437a3-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="437a3-121">Properties</span></span>
|<span data-ttu-id="437a3-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="437a3-122">Property</span></span>|<span data-ttu-id="437a3-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="437a3-123">Type</span></span>|<span data-ttu-id="437a3-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="437a3-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="437a3-125">id</span><span class="sxs-lookup"><span data-stu-id="437a3-125">id</span></span>|<span data-ttu-id="437a3-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="437a3-126">String</span></span>|<span data-ttu-id="437a3-127">O GUID do objeto Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-127">The GUID for the object Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="437a3-128">displayName</span><span class="sxs-lookup"><span data-stu-id="437a3-128">displayName</span></span>|<span data-ttu-id="437a3-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="437a3-129">String</span></span>|<span data-ttu-id="437a3-130">Nome do perfil Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-130">Name of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="437a3-131">description</span><span class="sxs-lookup"><span data-stu-id="437a3-131">description</span></span>|<span data-ttu-id="437a3-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="437a3-132">String</span></span>|<span data-ttu-id="437a3-133">Descrição do perfil de Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-133">Description of the profile Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="437a3-134">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="437a3-134">requiresUserAuthentication</span></span>|<span data-ttu-id="437a3-135">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-135">Boolean</span></span>|<span data-ttu-id="437a3-136">Indica se o perfil exige autenticação do usuário Inherited de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-136">Indicates if the profile requires user authentication Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="437a3-137">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="437a3-137">configurationEndpointUrl</span></span>|<span data-ttu-id="437a3-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="437a3-138">String</span></span>|<span data-ttu-id="437a3-139">Url de ponto de extremidade de configuração a ser usado para inscrição herdada do [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-139">Configuration endpoint url to use for Enrollment Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="437a3-140">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="437a3-140">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="437a3-141">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-141">Boolean</span></span>|<span data-ttu-id="437a3-142">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="437a3-142">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span> <span data-ttu-id="437a3-143">Herdado de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="437a3-143">Inherited from [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span></span>|
|<span data-ttu-id="437a3-144">isDefault</span><span class="sxs-lookup"><span data-stu-id="437a3-144">isDefault</span></span>|<span data-ttu-id="437a3-145">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-145">Boolean</span></span>|<span data-ttu-id="437a3-146">Indica se esse é o perfil padrão</span><span class="sxs-lookup"><span data-stu-id="437a3-146">Indicates if this is the default profile</span></span>|
|<span data-ttu-id="437a3-147">supervisedModeEnabled</span><span class="sxs-lookup"><span data-stu-id="437a3-147">supervisedModeEnabled</span></span>|<span data-ttu-id="437a3-148">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-148">Boolean</span></span>|<span data-ttu-id="437a3-149">Modo supervisionado, True para habilitar, false caso contrário.</span><span class="sxs-lookup"><span data-stu-id="437a3-149">Supervised mode, True to enable, false otherwise.</span></span> <span data-ttu-id="437a3-150">Consulte https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune para obter informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="437a3-150">See https://docs.microsoft.com/en-us/intune/deploy-use/enroll-devices-in-microsoft-intune for additional information.</span></span>|
|<span data-ttu-id="437a3-151">supportDepartment</span><span class="sxs-lookup"><span data-stu-id="437a3-151">supportDepartment</span></span>|<span data-ttu-id="437a3-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="437a3-152">String</span></span>|<span data-ttu-id="437a3-153">Informações do departamento de suporte</span><span class="sxs-lookup"><span data-stu-id="437a3-153">Support department information</span></span>|
|<span data-ttu-id="437a3-154">passCodeDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-154">passCodeDisabled</span></span>|<span data-ttu-id="437a3-155">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-155">Boolean</span></span>|<span data-ttu-id="437a3-156">Indica se o painel de configuração de senha está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-156">Indicates if Passcode setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-157">isMandatory</span><span class="sxs-lookup"><span data-stu-id="437a3-157">isMandatory</span></span>|<span data-ttu-id="437a3-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-158">Boolean</span></span>|<span data-ttu-id="437a3-159">Indica se o perfil é obrigatório</span><span class="sxs-lookup"><span data-stu-id="437a3-159">Indicates if the profile is mandatory</span></span>|
|<span data-ttu-id="437a3-160">locationDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-160">locationDisabled</span></span>|<span data-ttu-id="437a3-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-161">Boolean</span></span>|<span data-ttu-id="437a3-162">Indica se o painel de configuração do serviço local está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-162">Indicates if Location service setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-163">supportPhoneNumber</span><span class="sxs-lookup"><span data-stu-id="437a3-163">supportPhoneNumber</span></span>|<span data-ttu-id="437a3-164">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="437a3-164">String</span></span>|<span data-ttu-id="437a3-165">Número de telefone de suporte</span><span class="sxs-lookup"><span data-stu-id="437a3-165">Support phone number</span></span>|
|<span data-ttu-id="437a3-166">profileRemovalDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-166">profileRemovalDisabled</span></span>|<span data-ttu-id="437a3-167">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-167">Boolean</span></span>|<span data-ttu-id="437a3-168">Indica se a opção de remoção do perfil está desabilitada</span><span class="sxs-lookup"><span data-stu-id="437a3-168">Indicates if the profile removal option is disabled</span></span>|
|<span data-ttu-id="437a3-169">restoreBlocked</span><span class="sxs-lookup"><span data-stu-id="437a3-169">restoreBlocked</span></span>|<span data-ttu-id="437a3-170">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-170">Boolean</span></span>|<span data-ttu-id="437a3-171">Indica se o painel de configuração de restauração será bloqueado</span><span class="sxs-lookup"><span data-stu-id="437a3-171">Indicates if Restore setup pane is blocked</span></span>|
|<span data-ttu-id="437a3-172">appleIdDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-172">appleIdDisabled</span></span>|<span data-ttu-id="437a3-173">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-173">Boolean</span></span>|<span data-ttu-id="437a3-174">Indica se o painel de configuração de id do Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-174">Indicates if Apple id setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-175">termsAndConditionsDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-175">termsAndConditionsDisabled</span></span>|<span data-ttu-id="437a3-176">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-176">Boolean</span></span>|<span data-ttu-id="437a3-177">Indica se o painel de configuração de 'Termos e condições' está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-177">Indicates if 'Terms and Conditions' setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-178">touchIdDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-178">touchIdDisabled</span></span>|<span data-ttu-id="437a3-179">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-179">Boolean</span></span>|<span data-ttu-id="437a3-180">Indica se o painel de configuração de id de toque está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-180">Indicates if touch id setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-181">applePayDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-181">applePayDisabled</span></span>|<span data-ttu-id="437a3-182">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-182">Boolean</span></span>|<span data-ttu-id="437a3-183">Indica se o painel de configuração de pagamento do Apple está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-183">Indicates if Apple pay setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-184">zoomDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-184">zoomDisabled</span></span>|<span data-ttu-id="437a3-185">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-185">Boolean</span></span>|<span data-ttu-id="437a3-186">Indica se o painel de configuração de zoom está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-186">Indicates if zoom setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-187">siriDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-187">siriDisabled</span></span>|<span data-ttu-id="437a3-188">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-188">Boolean</span></span>|<span data-ttu-id="437a3-189">Indica se o painel de configuração de siri está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-189">Indicates if siri setup pane is disabled</span></span>|
|<span data-ttu-id="437a3-190">diagnosticsDisabled</span><span class="sxs-lookup"><span data-stu-id="437a3-190">diagnosticsDisabled</span></span>|<span data-ttu-id="437a3-191">Booliano</span><span class="sxs-lookup"><span data-stu-id="437a3-191">Boolean</span></span>|<span data-ttu-id="437a3-192">Indica se o painel de configuração de diagnósticos está desabilitado</span><span class="sxs-lookup"><span data-stu-id="437a3-192">Indicates if diagnostics setup pane is disabled</span></span>|

## <a name="relationships"></a><span data-ttu-id="437a3-193">Relações</span><span class="sxs-lookup"><span data-stu-id="437a3-193">Relationships</span></span>
<span data-ttu-id="437a3-194">Nenhum</span><span class="sxs-lookup"><span data-stu-id="437a3-194">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="437a3-195">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="437a3-195">JSON Representation</span></span>
<span data-ttu-id="437a3-196">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="437a3-196">Here is a JSON representation of the resource.</span></span>
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
  "diagnosticsDisabled": true
}
```





