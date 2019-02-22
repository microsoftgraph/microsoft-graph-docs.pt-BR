---
title: tipo de recurso enrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3d8947864611ac2c0d26256a5d739d41b86c383f
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30151174"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="283e6-104">tipo de recurso enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-104">enrollmentProfile resource type</span></span>

> <span data-ttu-id="283e6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="283e6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="283e6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="283e6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="283e6-107">O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="283e6-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="283e6-108">As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="283e6-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="283e6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="283e6-109">Methods</span></span>
|<span data-ttu-id="283e6-110">Método</span><span class="sxs-lookup"><span data-stu-id="283e6-110">Method</span></span>|<span data-ttu-id="283e6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="283e6-111">Return Type</span></span>|<span data-ttu-id="283e6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="283e6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="283e6-113">Listar enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="283e6-113">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="283e6-114">coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="283e6-114">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="283e6-115">Listar Propriedades e relações dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="283e6-115">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="283e6-116">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-116">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="283e6-117">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-117">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="283e6-118">Leia as propriedades e as relações do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="283e6-118">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="283e6-119">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-119">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="283e6-120">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-120">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="283e6-121">Criar um novo objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="283e6-121">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="283e6-122">Excluir enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-122">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="283e6-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="283e6-123">None</span></span>|<span data-ttu-id="283e6-124">Exclui [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="283e6-124">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="283e6-125">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-125">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="283e6-126">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-126">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="283e6-127">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="283e6-127">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="283e6-128">Ação setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="283e6-128">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="283e6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="283e6-129">None</span></span>|<span data-ttu-id="283e6-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="283e6-130">Not yet documented</span></span>|
|[<span data-ttu-id="283e6-131">função função exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="283e6-131">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="283e6-132">String</span><span class="sxs-lookup"><span data-stu-id="283e6-132">String</span></span>|<span data-ttu-id="283e6-133">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="283e6-133">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="283e6-134">Ação updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="283e6-134">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="283e6-135">Nenhum</span><span class="sxs-lookup"><span data-stu-id="283e6-135">None</span></span>|<span data-ttu-id="283e6-136">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="283e6-136">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="283e6-137">Propriedades</span><span class="sxs-lookup"><span data-stu-id="283e6-137">Properties</span></span>
|<span data-ttu-id="283e6-138">Propriedade</span><span class="sxs-lookup"><span data-stu-id="283e6-138">Property</span></span>|<span data-ttu-id="283e6-139">Tipo</span><span class="sxs-lookup"><span data-stu-id="283e6-139">Type</span></span>|<span data-ttu-id="283e6-140">Descrição</span><span class="sxs-lookup"><span data-stu-id="283e6-140">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="283e6-141">id</span><span class="sxs-lookup"><span data-stu-id="283e6-141">id</span></span>|<span data-ttu-id="283e6-142">String</span><span class="sxs-lookup"><span data-stu-id="283e6-142">String</span></span>|<span data-ttu-id="283e6-143">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="283e6-143">The GUID for the object</span></span>|
|<span data-ttu-id="283e6-144">displayName</span><span class="sxs-lookup"><span data-stu-id="283e6-144">displayName</span></span>|<span data-ttu-id="283e6-145">String</span><span class="sxs-lookup"><span data-stu-id="283e6-145">String</span></span>|<span data-ttu-id="283e6-146">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="283e6-146">Name of the profile</span></span>|
|<span data-ttu-id="283e6-147">description</span><span class="sxs-lookup"><span data-stu-id="283e6-147">description</span></span>|<span data-ttu-id="283e6-148">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="283e6-148">String</span></span>|<span data-ttu-id="283e6-149">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="283e6-149">Description of the profile</span></span>|
|<span data-ttu-id="283e6-150">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="283e6-150">requiresUserAuthentication</span></span>|<span data-ttu-id="283e6-151">Booliano</span><span class="sxs-lookup"><span data-stu-id="283e6-151">Boolean</span></span>|<span data-ttu-id="283e6-152">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="283e6-152">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="283e6-153">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="283e6-153">configurationEndpointUrl</span></span>|<span data-ttu-id="283e6-154">String</span><span class="sxs-lookup"><span data-stu-id="283e6-154">String</span></span>|<span data-ttu-id="283e6-155">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="283e6-155">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="283e6-156">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="283e6-156">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="283e6-157">Booliano</span><span class="sxs-lookup"><span data-stu-id="283e6-157">Boolean</span></span>|<span data-ttu-id="283e6-158">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="283e6-158">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="283e6-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="283e6-159">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="283e6-160">Booliano</span><span class="sxs-lookup"><span data-stu-id="283e6-160">Boolean</span></span>|<span data-ttu-id="283e6-161">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="283e6-161">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="283e6-162">Relações</span><span class="sxs-lookup"><span data-stu-id="283e6-162">Relationships</span></span>
<span data-ttu-id="283e6-163">Nenhum</span><span class="sxs-lookup"><span data-stu-id="283e6-163">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="283e6-164">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="283e6-164">JSON Representation</span></span>
<span data-ttu-id="283e6-165">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="283e6-165">Here is a JSON representation of the resource.</span></span>
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




