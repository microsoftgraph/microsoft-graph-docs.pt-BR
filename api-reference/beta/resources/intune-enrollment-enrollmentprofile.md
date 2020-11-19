---
title: tipo de recurso enrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4b7d2683baed89505280d8866132ce9e7846bbc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259813"
---
# <a name="enrollmentprofile-resource-type"></a><span data-ttu-id="bbbfd-104">tipo de recurso enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-104">enrollmentProfile resource type</span></span>

<span data-ttu-id="bbbfd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bbbfd-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bbbfd-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bbbfd-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bbbfd-108">O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="bbbfd-109">As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="bbbfd-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="bbbfd-110">Methods</span></span>
|<span data-ttu-id="bbbfd-111">Método</span><span class="sxs-lookup"><span data-stu-id="bbbfd-111">Method</span></span>|<span data-ttu-id="bbbfd-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bbbfd-112">Return Type</span></span>|<span data-ttu-id="bbbfd-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbfd-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bbbfd-114">Listar enrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="bbbfd-114">List enrollmentProfiles</span></span>](../api/intune-enrollment-enrollmentprofile-list.md)|<span data-ttu-id="bbbfd-115">coleção [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="bbbfd-115">[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) collection</span></span>|<span data-ttu-id="bbbfd-116">Listar Propriedades e relações dos objetos [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bbbfd-116">List properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="bbbfd-117">Obter enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-117">Get enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-get.md)|[<span data-ttu-id="bbbfd-118">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-118">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="bbbfd-119">Leia as propriedades e as relações do objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bbbfd-119">Read properties and relationships of the [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="bbbfd-120">Criar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-120">Create enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-create.md)|[<span data-ttu-id="bbbfd-121">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-121">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="bbbfd-122">Criar um novo objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bbbfd-122">Create a new [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="bbbfd-123">Excluir enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-123">Delete enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-delete.md)|<span data-ttu-id="bbbfd-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbbfd-124">None</span></span>|<span data-ttu-id="bbbfd-125">Exclui [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="bbbfd-125">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>|
|[<span data-ttu-id="bbbfd-126">Atualizar enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-126">Update enrollmentProfile</span></span>](../api/intune-enrollment-enrollmentprofile-update.md)|[<span data-ttu-id="bbbfd-127">enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-127">enrollmentProfile</span></span>](../resources/intune-enrollment-enrollmentprofile.md)|<span data-ttu-id="bbbfd-128">Atualiza as propriedades de um objeto [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="bbbfd-128">Update the properties of a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="bbbfd-129">Ação setDefaultProfile</span><span class="sxs-lookup"><span data-stu-id="bbbfd-129">setDefaultProfile action</span></span>](../api/intune-enrollment-enrollmentprofile-setdefaultprofile.md)|<span data-ttu-id="bbbfd-130">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bbbfd-130">None</span></span>|<span data-ttu-id="bbbfd-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bbbfd-131">Not yet documented</span></span>|
|[<span data-ttu-id="bbbfd-132">função função exportmobileconfig</span><span class="sxs-lookup"><span data-stu-id="bbbfd-132">exportMobileConfig function</span></span>](../api/intune-enrollment-enrollmentprofile-exportmobileconfig.md)|<span data-ttu-id="bbbfd-133">String</span><span class="sxs-lookup"><span data-stu-id="bbbfd-133">String</span></span>|<span data-ttu-id="bbbfd-134">Exporta a configuração móvel</span><span class="sxs-lookup"><span data-stu-id="bbbfd-134">Exports the mobile configuration</span></span>|
|[<span data-ttu-id="bbbfd-135">Ação updateDeviceProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="bbbfd-135">updateDeviceProfileAssignment action</span></span>](../api/intune-enrollment-enrollmentprofile-updatedeviceprofileassignment.md)|<span data-ttu-id="bbbfd-136">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="bbbfd-136">None</span></span>|<span data-ttu-id="bbbfd-137">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="bbbfd-137">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="bbbfd-138">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bbbfd-138">Properties</span></span>
|<span data-ttu-id="bbbfd-139">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bbbfd-139">Property</span></span>|<span data-ttu-id="bbbfd-140">Tipo</span><span class="sxs-lookup"><span data-stu-id="bbbfd-140">Type</span></span>|<span data-ttu-id="bbbfd-141">Descrição</span><span class="sxs-lookup"><span data-stu-id="bbbfd-141">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbbfd-142">id</span><span class="sxs-lookup"><span data-stu-id="bbbfd-142">id</span></span>|<span data-ttu-id="bbbfd-143">String</span><span class="sxs-lookup"><span data-stu-id="bbbfd-143">String</span></span>|<span data-ttu-id="bbbfd-144">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-144">The GUID for the object</span></span>|
|<span data-ttu-id="bbbfd-145">displayName</span><span class="sxs-lookup"><span data-stu-id="bbbfd-145">displayName</span></span>|<span data-ttu-id="bbbfd-146">String</span><span class="sxs-lookup"><span data-stu-id="bbbfd-146">String</span></span>|<span data-ttu-id="bbbfd-147">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="bbbfd-147">Name of the profile</span></span>|
|<span data-ttu-id="bbbfd-148">description</span><span class="sxs-lookup"><span data-stu-id="bbbfd-148">description</span></span>|<span data-ttu-id="bbbfd-149">String</span><span class="sxs-lookup"><span data-stu-id="bbbfd-149">String</span></span>|<span data-ttu-id="bbbfd-150">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="bbbfd-150">Description of the profile</span></span>|
|<span data-ttu-id="bbbfd-151">requiresUserAuthentication</span><span class="sxs-lookup"><span data-stu-id="bbbfd-151">requiresUserAuthentication</span></span>|<span data-ttu-id="bbbfd-152">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbbfd-152">Boolean</span></span>|<span data-ttu-id="bbbfd-153">Indica se o perfil requer autenticação do usuário</span><span class="sxs-lookup"><span data-stu-id="bbbfd-153">Indicates if the profile requires user authentication</span></span>|
|<span data-ttu-id="bbbfd-154">configurationEndpointUrl</span><span class="sxs-lookup"><span data-stu-id="bbbfd-154">configurationEndpointUrl</span></span>|<span data-ttu-id="bbbfd-155">String</span><span class="sxs-lookup"><span data-stu-id="bbbfd-155">String</span></span>|<span data-ttu-id="bbbfd-156">URL de ponto de extremidade de configuração a ser usada para registro</span><span class="sxs-lookup"><span data-stu-id="bbbfd-156">Configuration endpoint url to use for Enrollment</span></span>|
|<span data-ttu-id="bbbfd-157">Enableauthenticationviacompanyportal foi adicionada</span><span class="sxs-lookup"><span data-stu-id="bbbfd-157">enableAuthenticationViaCompanyPortal</span></span>|<span data-ttu-id="bbbfd-158">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbbfd-158">Boolean</span></span>|<span data-ttu-id="bbbfd-159">Indica a autenticação com o assistente de configuração da Apple em vez do portal da empresa.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-159">Indicates to authenticate with Apple Setup Assistant instead of Company Portal.</span></span>|
|<span data-ttu-id="bbbfd-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span><span class="sxs-lookup"><span data-stu-id="bbbfd-160">requireCompanyPortalOnSetupAssistantEnrolledDevices</span></span>|<span data-ttu-id="bbbfd-161">Booliano</span><span class="sxs-lookup"><span data-stu-id="bbbfd-161">Boolean</span></span>|<span data-ttu-id="bbbfd-162">Indica que o portal da empresa é necessário no assistente de configuração dispositivos registrados</span><span class="sxs-lookup"><span data-stu-id="bbbfd-162">Indicates that Company Portal is required on setup assistant enrolled devices</span></span>|

## <a name="relationships"></a><span data-ttu-id="bbbfd-163">Relações</span><span class="sxs-lookup"><span data-stu-id="bbbfd-163">Relationships</span></span>
<span data-ttu-id="bbbfd-164">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bbbfd-164">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbbfd-165">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bbbfd-165">JSON Representation</span></span>
<span data-ttu-id="bbbfd-166">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bbbfd-166">Here is a JSON representation of the resource.</span></span>
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




