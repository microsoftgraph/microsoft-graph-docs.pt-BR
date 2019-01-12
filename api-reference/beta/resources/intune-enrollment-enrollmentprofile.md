---
title: tipo de recurso de enrollmentProfile
description: O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados. As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
localization_priority: Normal
author: tfitzmac
ms.prod: intune
ms.openlocfilehash: b88745c060e71e32199a96b23f94fa0d3229d451
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935588"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="587da-104">tipo de recurso de enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="587da-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="587da-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="587da-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="587da-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="587da-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="587da-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="587da-108">O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados.</span><span class="sxs-lookup"><span data-stu-id="587da-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="587da-109">As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="587da-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="587da-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="587da-110">Methods</span></span>
|<span data-ttu-id="587da-111">Método</span><span class="sxs-lookup"><span data-stu-id="587da-111">Method</span></span>|<span data-ttu-id="587da-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="587da-112">Return Type</span></span>|<span data-ttu-id="587da-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="587da-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="587da-114">Lista enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="587da-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="587da-115">coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="587da-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="587da-116">Lista as propriedades e os relacionamentos dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="587da-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="587da-117">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="587da-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="587da-119">Leia as propriedades e os relacionamentos do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="587da-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="587da-120">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="587da-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="587da-122">Crie um novo objeto de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="587da-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="587da-123">Excluir enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="587da-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="587da-124">None</span></span>|<span data-ttu-id="587da-125">Exclui um [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="587da-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="587da-126">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="587da-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="587da-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="587da-128">Atualize as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="587da-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="587da-129">ação de setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="587da-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="587da-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="587da-130">None</span></span>|<span data-ttu-id="587da-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="587da-131">Not yet documented</span></span>|
|[<span data-ttu-id="587da-132">função exportMobileConfig</span><span class="sxs-lookup"><span data-stu-id="587da-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="587da-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="587da-133">String</span></span>|<span data-ttu-id="587da-134">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="587da-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="587da-135">ação de updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="587da-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="587da-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="587da-136">None</span></span>|<span data-ttu-id="587da-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="587da-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="587da-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="587da-138">Properties</span></span>
|<span data-ttu-id="587da-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="587da-139">Property</span></span>|<span data-ttu-id="587da-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="587da-140">Type</span></span>|<span data-ttu-id="587da-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="587da-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="587da-142">id</span><span class="sxs-lookup"><span data-stu-id="587da-142">id</span></span>|<span data-ttu-id="587da-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="587da-143">String</span></span>|<span data-ttu-id="587da-144">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="587da-144">The GUID for the object</span></span>|
|<span data-ttu-id="587da-145">displayName</span><span class="sxs-lookup"><span data-stu-id="587da-145">displayName</span></span>|<span data-ttu-id="587da-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="587da-146">String</span></span>|<span data-ttu-id="587da-147">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="587da-147">Name of the profile</span></span>|
|<span data-ttu-id="587da-148">description</span><span class="sxs-lookup"><span data-stu-id="587da-148">description</span></span>|<span data-ttu-id="587da-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="587da-149">String</span></span>|<span data-ttu-id="587da-150">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="587da-150">Description of the profile</span></span>|
|<span data-ttu-id="587da-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="587da-151">requiresUserAuthentication</span></span>|<span data-ttu-id="587da-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="587da-152">Boolean</span></span>|<span data-ttu-id="587da-153">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="587da-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="587da-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="587da-154">configurationEndpointUrl</span></span>|<span data-ttu-id="587da-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="587da-155">String</span></span>|<span data-ttu-id="587da-156">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="587da-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="587da-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="587da-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="587da-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="587da-158">Boolean</span></span>|<span data-ttu-id="587da-159">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="587da-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="587da-160">Relações</span><span class="sxs-lookup"><span data-stu-id="587da-160">Relationships</span></span>
<span data-ttu-id="587da-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="587da-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="587da-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="587da-162">JSON Representation</span></span>
<span data-ttu-id="587da-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="587da-163">Here is a JSON representation of the resource.</span></span>
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
  "enableAuthenticationViaCompanyPortal": true
}
```





