---
title: tipo de recurso enrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8ccd3bfaea1d76c77bea62bfb3ebefaad827570e
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35999175"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="6b9a8-104">tipo de recurso enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="6b9a8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b9a8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b9a8-107">O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="6b9a8-108">As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="6b9a8-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="6b9a8-109">Methods</span></span>
|<span data-ttu-id="6b9a8-110">Método</span><span class="sxs-lookup"><span data-stu-id="6b9a8-110">Method</span></span>|<span data-ttu-id="6b9a8-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="6b9a8-111">Return Type</span></span>|<span data-ttu-id="6b9a8-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b9a8-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6b9a8-113">Listar enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="6b9a8-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="6b9a8-114">coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="6b9a8-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="6b9a8-115">Listar Propriedades e relações dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6b9a8-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="6b9a8-116">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="6b9a8-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="6b9a8-118">Leia as propriedades e as relações do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6b9a8-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="6b9a8-119">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="6b9a8-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="6b9a8-121">Criar um novo objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6b9a8-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="6b9a8-122">Excluir enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="6b9a8-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b9a8-123">None</span></span>|<span data-ttu-id="6b9a8-124">Exclui [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="6b9a8-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="6b9a8-125">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="6b9a8-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="6b9a8-127">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="6b9a8-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="6b9a8-128">Ação setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="6b9a8-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="6b9a8-129">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6b9a8-129">None</span></span>|<span data-ttu-id="6b9a8-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6b9a8-130">Not yet documented</span></span>|
|[<span data-ttu-id="6b9a8-131">função função exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="6b9a8-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="6b9a8-132">String</span><span class="sxs-lookup"><span data-stu-id="6b9a8-132">String</span></span>|<span data-ttu-id="6b9a8-133">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="6b9a8-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="6b9a8-134">Ação updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="6b9a8-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="6b9a8-135">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="6b9a8-135">None</span></span>|<span data-ttu-id="6b9a8-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6b9a8-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="6b9a8-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6b9a8-137">Properties</span></span>
|<span data-ttu-id="6b9a8-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6b9a8-138">Property</span></span>|<span data-ttu-id="6b9a8-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="6b9a8-139">Type</span></span>|<span data-ttu-id="6b9a8-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="6b9a8-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b9a8-141">id</span><span class="sxs-lookup"><span data-stu-id="6b9a8-141">id</span></span>|<span data-ttu-id="6b9a8-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6b9a8-142">String</span></span>|<span data-ttu-id="6b9a8-143">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-143">The GUID for the object</span></span>|
|<span data-ttu-id="6b9a8-144">displayName</span><span class="sxs-lookup"><span data-stu-id="6b9a8-144">displayName</span></span>|<span data-ttu-id="6b9a8-145">String</span><span class="sxs-lookup"><span data-stu-id="6b9a8-145">String</span></span>|<span data-ttu-id="6b9a8-146">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="6b9a8-146">Name of the profile</span></span>|
|<span data-ttu-id="6b9a8-147">descrição</span><span class="sxs-lookup"><span data-stu-id="6b9a8-147">description</span></span>|<span data-ttu-id="6b9a8-148">String</span><span class="sxs-lookup"><span data-stu-id="6b9a8-148">String</span></span>|<span data-ttu-id="6b9a8-149">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="6b9a8-149">Description of the profile</span></span>|
|<span data-ttu-id="6b9a8-150">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="6b9a8-150">requiresUserAuthentication</span></span>|<span data-ttu-id="6b9a8-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b9a8-151">Boolean</span></span>|<span data-ttu-id="6b9a8-152">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="6b9a8-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="6b9a8-153">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="6b9a8-153">configurationEndpointUrl</span></span>|<span data-ttu-id="6b9a8-154">String</span><span class="sxs-lookup"><span data-stu-id="6b9a8-154">String</span></span>|<span data-ttu-id="6b9a8-155">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="6b9a8-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="6b9a8-156">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="6b9a8-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="6b9a8-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b9a8-157">Boolean</span></span>|<span data-ttu-id="6b9a8-158">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="6b9a8-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="6b9a8-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="6b9a8-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="6b9a8-160">Boolean</span></span>|<span data-ttu-id="6b9a8-161">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="6b9a8-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="6b9a8-162">Relações</span><span class="sxs-lookup"><span data-stu-id="6b9a8-162">Relationships</span></span>
<span data-ttu-id="6b9a8-163">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6b9a8-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6b9a8-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6b9a8-164">JSON Representation</span></span>
<span data-ttu-id="6b9a8-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6b9a8-165">Here is a JSON representation of the resource.</span></span>
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





