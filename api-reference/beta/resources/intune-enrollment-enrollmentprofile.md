---
title: tipo de recurso de enrollmentProfile
description: O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados. As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
ms.openlocfilehash: 884fee5c6851e79d96cd036294e5e5485d6df66a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27036796"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="cee79-104">tipo de recurso de enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="cee79-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="cee79-105">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cee79-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="cee79-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cee79-107">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="cee79-107">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cee79-108">O recurso de enrollmentProfile representa uma coleção de configurações que devem ser fornecidas a inscrição prévia para habilitar inscrevendo determinados dispositivos cujas identidades foram pré-configurados.</span><span class="sxs-lookup"><span data-stu-id="cee79-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="cee79-109">As identidades de dispositivo pré-configurados são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="cee79-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>
## <a name="methods"></a><span data-ttu-id="cee79-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="cee79-110">Methods</span></span>
|<span data-ttu-id="cee79-111">Método</span><span class="sxs-lookup"><span data-stu-id="cee79-111">Method</span></span>|<span data-ttu-id="cee79-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="cee79-112">Return Type</span></span>|<span data-ttu-id="cee79-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="cee79-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="cee79-114">Lista enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="cee79-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="cee79-115">coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="cee79-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="cee79-116">Lista as propriedades e os relacionamentos dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cee79-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="cee79-117">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="cee79-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="cee79-119">Leia as propriedades e os relacionamentos do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cee79-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="cee79-120">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="cee79-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="cee79-122">Crie um novo objeto de [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cee79-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="cee79-123">Excluir enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="cee79-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cee79-124">None</span></span>|<span data-ttu-id="cee79-125">Exclui um [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="cee79-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="cee79-126">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="cee79-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="cee79-128">Atualize as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="cee79-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="cee79-129">ação de setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="cee79-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="cee79-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cee79-130">None</span></span>|<span data-ttu-id="cee79-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cee79-131">Not yet documented</span></span>|
|[<span data-ttu-id="cee79-132">função exportMobileConfig</span><span class="sxs-lookup"><span data-stu-id="cee79-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="cee79-133">String</span><span class="sxs-lookup"><span data-stu-id="cee79-133">String</span></span>|<span data-ttu-id="cee79-134">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="cee79-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="cee79-135">ação de updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="cee79-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="cee79-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cee79-136">None</span></span>|<span data-ttu-id="cee79-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="cee79-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="cee79-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cee79-138">Properties</span></span>
|<span data-ttu-id="cee79-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cee79-139">Property</span></span>|<span data-ttu-id="cee79-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="cee79-140">Type</span></span>|<span data-ttu-id="cee79-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="cee79-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cee79-142">id</span><span class="sxs-lookup"><span data-stu-id="cee79-142">id</span></span>|<span data-ttu-id="cee79-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="cee79-143">String</span></span>|<span data-ttu-id="cee79-144">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="cee79-144">The GUID for the object</span></span>|
|<span data-ttu-id="cee79-145">displayName</span><span class="sxs-lookup"><span data-stu-id="cee79-145">displayName</span></span>|<span data-ttu-id="cee79-146">String</span><span class="sxs-lookup"><span data-stu-id="cee79-146">String</span></span>|<span data-ttu-id="cee79-147">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="cee79-147">Name of the profile</span></span>|
|<span data-ttu-id="cee79-148">description</span><span class="sxs-lookup"><span data-stu-id="cee79-148">description</span></span>|<span data-ttu-id="cee79-149">String</span><span class="sxs-lookup"><span data-stu-id="cee79-149">String</span></span>|<span data-ttu-id="cee79-150">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="cee79-150">Description of the profile</span></span>|
|<span data-ttu-id="cee79-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="cee79-151">requiresUserAuthentication</span></span>|<span data-ttu-id="cee79-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="cee79-152">Boolean</span></span>|<span data-ttu-id="cee79-153">Indica se o perfil exige autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="cee79-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="cee79-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="cee79-154">configurationEndpointUrl</span></span>|<span data-ttu-id="cee79-155">String</span><span class="sxs-lookup"><span data-stu-id="cee79-155">String</span></span>|<span data-ttu-id="cee79-156">Url de ponto de extremidade de configuração a ser usado para registro</span><span class="sxs-lookup"><span data-stu-id="cee79-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="cee79-157">enableAuthenticationViaCompanyPortal</span><span class="sxs-lookup"><span data-stu-id="cee79-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="cee79-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="cee79-158">Boolean</span></span>|<span data-ttu-id="cee79-159">Indica para autenticar com o Assistente de configuração do Apple em vez do Portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="cee79-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cee79-160">Relações</span><span class="sxs-lookup"><span data-stu-id="cee79-160">Relationships</span></span>
<span data-ttu-id="cee79-161">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cee79-161">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="cee79-162">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cee79-162">JSON Representation</span></span>
<span data-ttu-id="cee79-163">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cee79-163">Here is a JSON representation of the resource.</span></span>
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





