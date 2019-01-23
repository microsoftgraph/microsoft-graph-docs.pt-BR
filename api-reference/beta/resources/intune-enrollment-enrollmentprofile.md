---
title: tipo de recurso de enrollmentProfile
description: O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados. As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7a7ce4aac1e22610d539419dd6a63d124616b83f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396837"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="568d9-104">tipo de recurso de enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="568d9-105">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="568d9-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="568d9-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="568d9-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="568d9-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="568d9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="568d9-108">O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados.</span><span class="sxs-lookup"><span data-stu-id="568d9-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="568d9-109">As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="568d9-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="568d9-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="568d9-110">Methods</span></span>
|<span data-ttu-id="568d9-111">Método</span><span class="sxs-lookup"><span data-stu-id="568d9-111">Method</span></span>|<span data-ttu-id="568d9-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="568d9-112">Return Type</span></span>|<span data-ttu-id="568d9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="568d9-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="568d9-114">Lista enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="568d9-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="568d9-115">coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="568d9-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="568d9-116">Lista as propriedades e os relacionamentos dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="568d9-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="568d9-117">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="568d9-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="568d9-119">Leia as propriedades e os relacionamentos do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="568d9-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="568d9-120">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="568d9-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="568d9-122">Crie um novo objeto de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="568d9-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="568d9-123">Excluir enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="568d9-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="568d9-124">None</span></span>|<span data-ttu-id="568d9-125">Exclui um [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="568d9-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="568d9-126">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="568d9-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="568d9-128">Atualize as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="568d9-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="568d9-129">ação de setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="568d9-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="568d9-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="568d9-130">None</span></span>|<span data-ttu-id="568d9-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="568d9-131">Not yet documented</span></span>|
|[<span data-ttu-id="568d9-132">função exportMobileConfig</span><span class="sxs-lookup"><span data-stu-id="568d9-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="568d9-133">String</span><span class="sxs-lookup"><span data-stu-id="568d9-133">String</span></span>|<span data-ttu-id="568d9-134">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="568d9-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="568d9-135">ação de updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="568d9-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="568d9-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="568d9-136">None</span></span>|<span data-ttu-id="568d9-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="568d9-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="568d9-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="568d9-138">Properties</span></span>
|<span data-ttu-id="568d9-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="568d9-139">Property</span></span>|<span data-ttu-id="568d9-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="568d9-140">Type</span></span>|<span data-ttu-id="568d9-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="568d9-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="568d9-142">id</span><span class="sxs-lookup"><span data-stu-id="568d9-142">id</span></span>|<span data-ttu-id="568d9-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="568d9-143">String</span></span>|<span data-ttu-id="568d9-144">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="568d9-144">The GUID for the object</span></span>|
|<span data-ttu-id="568d9-145">displayName</span><span class="sxs-lookup"><span data-stu-id="568d9-145">displayName</span></span>|<span data-ttu-id="568d9-146">String</span><span class="sxs-lookup"><span data-stu-id="568d9-146">String</span></span>|<span data-ttu-id="568d9-147">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="568d9-147">Name of the profile</span></span>|
|<span data-ttu-id="568d9-148">description</span><span class="sxs-lookup"><span data-stu-id="568d9-148">description</span></span>|<span data-ttu-id="568d9-149">String</span><span class="sxs-lookup"><span data-stu-id="568d9-149">String</span></span>|<span data-ttu-id="568d9-150">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="568d9-150">Description of the profile</span></span>|
|<span data-ttu-id="568d9-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="568d9-151">requiresUserAuthentication</span></span>|<span data-ttu-id="568d9-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="568d9-152">Boolean</span></span>|<span data-ttu-id="568d9-153">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="568d9-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="568d9-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="568d9-154">configurationEndpointUrl</span></span>|<span data-ttu-id="568d9-155">String</span><span class="sxs-lookup"><span data-stu-id="568d9-155">String</span></span>|<span data-ttu-id="568d9-156">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="568d9-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="568d9-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="568d9-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="568d9-158">Boolean</span><span class="sxs-lookup"><span data-stu-id="568d9-158">Boolean</span></span>|<span data-ttu-id="568d9-159">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="568d9-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="568d9-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="568d9-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="568d9-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="568d9-161">Boolean</span></span>|<span data-ttu-id="568d9-162">Indica que o Portal da empresa é necessária em dispositivos de inscritos do Assistente de instalação</span><span class="sxs-lookup"><span data-stu-id="568d9-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="568d9-163">Relações</span><span class="sxs-lookup"><span data-stu-id="568d9-163">Relationships</span></span>
<span data-ttu-id="568d9-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="568d9-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="568d9-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="568d9-165">JSON Representation</span></span>
<span data-ttu-id="568d9-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="568d9-166">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentProfile",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "requiresUserAuthentication": true,
  "configurationEndpointUrl": "String",
  "enableAuthenticationViaCompanyPortal": true,
  "requireCompanyPortalOnSetupAssistantEnrolledDevices": true
}
```




