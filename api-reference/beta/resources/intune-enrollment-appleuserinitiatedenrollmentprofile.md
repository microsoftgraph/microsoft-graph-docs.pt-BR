---
title: tipo de recurso appleUserInitiatedEnrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7f6f7d28d1c5684793891bc8bee08300f67ebeec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419477"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="d58b9-104">tipo de recurso appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

<span data-ttu-id="d58b9-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d58b9-105">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d58b9-106">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d58b9-106">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d58b9-107">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d58b9-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d58b9-108">O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="d58b9-108">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="d58b9-109">As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="d58b9-109">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="d58b9-110">Métodos</span><span class="sxs-lookup"><span data-stu-id="d58b9-110">Methods</span></span>
|<span data-ttu-id="d58b9-111">Método</span><span class="sxs-lookup"><span data-stu-id="d58b9-111">Method</span></span>|<span data-ttu-id="d58b9-112">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="d58b9-112">Return Type</span></span>|<span data-ttu-id="d58b9-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="d58b9-113">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d58b9-114">Listar appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="d58b9-114">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="d58b9-115">coleção [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="d58b9-115">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="d58b9-116">Listar Propriedades e relações dos objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d58b9-116">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="d58b9-117">Obter appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-117">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="d58b9-118">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-118">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="d58b9-119">Leia as propriedades e as relações do objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d58b9-119">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d58b9-120">Criar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-120">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="d58b9-121">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-121">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="d58b9-122">Criar um novo objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d58b9-122">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d58b9-123">Excluir appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-123">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="d58b9-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d58b9-124">None</span></span>|<span data-ttu-id="d58b9-125">Exclui [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="d58b9-125">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="d58b9-126">Atualizar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-126">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="d58b9-127">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="d58b9-127">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="d58b9-128">Atualiza as propriedades de um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="d58b9-128">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="d58b9-129">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="d58b9-129">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="d58b9-130">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d58b9-130">None</span></span>|<span data-ttu-id="d58b9-131">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d58b9-131">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d58b9-132">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d58b9-132">Properties</span></span>
|<span data-ttu-id="d58b9-133">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d58b9-133">Property</span></span>|<span data-ttu-id="d58b9-134">Tipo</span><span class="sxs-lookup"><span data-stu-id="d58b9-134">Type</span></span>|<span data-ttu-id="d58b9-135">Descrição</span><span class="sxs-lookup"><span data-stu-id="d58b9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d58b9-136">defaultenrollmentidtype</span><span class="sxs-lookup"><span data-stu-id="d58b9-136">defaultEnrollmentType</span></span>|[<span data-ttu-id="d58b9-137">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="d58b9-137">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="d58b9-138">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="d58b9-138">The default profile enrollment type.</span></span> <span data-ttu-id="d58b9-139">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="d58b9-139">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="d58b9-140">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="d58b9-140">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="d58b9-141">coleção [appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="d58b9-141">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="d58b9-142">Lista de opções de tipo de registro disponíveis</span><span class="sxs-lookup"><span data-stu-id="d58b9-142">List of available enrollment type options</span></span>|
|<span data-ttu-id="d58b9-143">id</span><span class="sxs-lookup"><span data-stu-id="d58b9-143">id</span></span>|<span data-ttu-id="d58b9-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d58b9-144">String</span></span>|<span data-ttu-id="d58b9-145">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="d58b9-145">The GUID for the object</span></span>|
|<span data-ttu-id="d58b9-146">displayName</span><span class="sxs-lookup"><span data-stu-id="d58b9-146">displayName</span></span>|<span data-ttu-id="d58b9-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d58b9-147">String</span></span>|<span data-ttu-id="d58b9-148">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="d58b9-148">Name of the profile</span></span>|
|<span data-ttu-id="d58b9-149">description</span><span class="sxs-lookup"><span data-stu-id="d58b9-149">description</span></span>|<span data-ttu-id="d58b9-150">String</span><span class="sxs-lookup"><span data-stu-id="d58b9-150">String</span></span>|<span data-ttu-id="d58b9-151">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="d58b9-151">Description of the profile</span></span>|
|<span data-ttu-id="d58b9-152">prioridade</span><span class="sxs-lookup"><span data-stu-id="d58b9-152">priority</span></span>|<span data-ttu-id="d58b9-153">Int32</span><span class="sxs-lookup"><span data-stu-id="d58b9-153">Int32</span></span>|<span data-ttu-id="d58b9-154">Prioridade, 0 é a maior</span><span class="sxs-lookup"><span data-stu-id="d58b9-154">Priority, 0 is highest</span></span>|
|<span data-ttu-id="d58b9-155">platform</span><span class="sxs-lookup"><span data-stu-id="d58b9-155">platform</span></span>|[<span data-ttu-id="d58b9-156">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="d58b9-156">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="d58b9-157">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="d58b9-157">The platform of the Device.</span></span> <span data-ttu-id="d58b9-158">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="d58b9-158">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="d58b9-159">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d58b9-159">createdDateTime</span></span>|<span data-ttu-id="d58b9-160">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d58b9-160">DateTimeOffset</span></span>|<span data-ttu-id="d58b9-161">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="d58b9-161">Profile creation time</span></span>|
|<span data-ttu-id="d58b9-162">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d58b9-162">lastModifiedDateTime</span></span>|<span data-ttu-id="d58b9-163">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d58b9-163">DateTimeOffset</span></span>|<span data-ttu-id="d58b9-164">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="d58b9-164">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="d58b9-165">Relações</span><span class="sxs-lookup"><span data-stu-id="d58b9-165">Relationships</span></span>
|<span data-ttu-id="d58b9-166">Relação</span><span class="sxs-lookup"><span data-stu-id="d58b9-166">Relationship</span></span>|<span data-ttu-id="d58b9-167">Tipo</span><span class="sxs-lookup"><span data-stu-id="d58b9-167">Type</span></span>|<span data-ttu-id="d58b9-168">Descrição</span><span class="sxs-lookup"><span data-stu-id="d58b9-168">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d58b9-169">assignments</span><span class="sxs-lookup"><span data-stu-id="d58b9-169">assignments</span></span>|<span data-ttu-id="d58b9-170">coleção [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d58b9-170">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="d58b9-171">A lista de atribuições para este perfil.</span><span class="sxs-lookup"><span data-stu-id="d58b9-171">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d58b9-172">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d58b9-172">JSON Representation</span></span>
<span data-ttu-id="d58b9-173">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d58b9-173">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appleUserInitiatedEnrollmentProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appleUserInitiatedEnrollmentProfile",
  "defaultEnrollmentType": "String",
  "availableEnrollmentTypeOptions": [
    {
      "@odata.type": "microsoft.graph.appleOwnerTypeEnrollmentType",
      "ownerType": "String",
      "enrollmentType": "String"
    }
  ],
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "platform": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



