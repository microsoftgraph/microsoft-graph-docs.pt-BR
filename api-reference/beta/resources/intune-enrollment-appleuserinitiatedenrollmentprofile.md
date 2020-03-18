---
title: tipo de recurso appleUserInitiatedEnrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b6bf6eefeb94156b85affa3df72665fbe4c3f7bb
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783568"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="15ee6-104">tipo de recurso appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

> <span data-ttu-id="15ee6-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="15ee6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15ee6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="15ee6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15ee6-107">O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="15ee6-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="15ee6-108">As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="15ee6-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="15ee6-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="15ee6-109">Methods</span></span>
|<span data-ttu-id="15ee6-110">Método</span><span class="sxs-lookup"><span data-stu-id="15ee6-110">Method</span></span>|<span data-ttu-id="15ee6-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="15ee6-111">Return Type</span></span>|<span data-ttu-id="15ee6-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ee6-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15ee6-113">Listar appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="15ee6-113">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="15ee6-114">coleção [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="15ee6-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="15ee6-115">Listar Propriedades e relações dos objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="15ee6-115">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="15ee6-116">Obter appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-116">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="15ee6-117">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-117">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="15ee6-118">Leia as propriedades e as relações do objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="15ee6-118">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="15ee6-119">Criar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-119">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="15ee6-120">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-120">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="15ee6-121">Criar um novo objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="15ee6-121">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="15ee6-122">Excluir appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-122">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="15ee6-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15ee6-123">None</span></span>|<span data-ttu-id="15ee6-124">Exclui [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="15ee6-124">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="15ee6-125">Atualizar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-125">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="15ee6-126">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="15ee6-126">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="15ee6-127">Atualiza as propriedades de um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="15ee6-127">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="15ee6-128">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="15ee6-128">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="15ee6-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15ee6-129">None</span></span>|<span data-ttu-id="15ee6-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="15ee6-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="15ee6-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15ee6-131">Properties</span></span>
|<span data-ttu-id="15ee6-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15ee6-132">Property</span></span>|<span data-ttu-id="15ee6-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ee6-133">Type</span></span>|<span data-ttu-id="15ee6-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ee6-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ee6-135">defaultenrollmentidtype</span><span class="sxs-lookup"><span data-stu-id="15ee6-135">defaultEnrollmentType</span></span>|[<span data-ttu-id="15ee6-136">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="15ee6-136">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="15ee6-137">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="15ee6-137">The default profile enrollment type.</span></span> <span data-ttu-id="15ee6-138">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="15ee6-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="15ee6-139">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="15ee6-139">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="15ee6-140">coleção [appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="15ee6-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="15ee6-141">Lista de opções de tipo de registro disponíveis</span><span class="sxs-lookup"><span data-stu-id="15ee6-141">List of available enrollment type options</span></span>|
|<span data-ttu-id="15ee6-142">id</span><span class="sxs-lookup"><span data-stu-id="15ee6-142">id</span></span>|<span data-ttu-id="15ee6-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15ee6-143">String</span></span>|<span data-ttu-id="15ee6-144">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="15ee6-144">The GUID for the object</span></span>|
|<span data-ttu-id="15ee6-145">displayName</span><span class="sxs-lookup"><span data-stu-id="15ee6-145">displayName</span></span>|<span data-ttu-id="15ee6-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15ee6-146">String</span></span>|<span data-ttu-id="15ee6-147">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="15ee6-147">Name of the profile</span></span>|
|<span data-ttu-id="15ee6-148">description</span><span class="sxs-lookup"><span data-stu-id="15ee6-148">description</span></span>|<span data-ttu-id="15ee6-149">String</span><span class="sxs-lookup"><span data-stu-id="15ee6-149">String</span></span>|<span data-ttu-id="15ee6-150">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="15ee6-150">Description of the profile</span></span>|
|<span data-ttu-id="15ee6-151">prioridade</span><span class="sxs-lookup"><span data-stu-id="15ee6-151">priority</span></span>|<span data-ttu-id="15ee6-152">Int32</span><span class="sxs-lookup"><span data-stu-id="15ee6-152">Int32</span></span>|<span data-ttu-id="15ee6-153">Prioridade, 0 é a maior</span><span class="sxs-lookup"><span data-stu-id="15ee6-153">Priority, 0 is highest</span></span>|
|<span data-ttu-id="15ee6-154">platform</span><span class="sxs-lookup"><span data-stu-id="15ee6-154">platform</span></span>|[<span data-ttu-id="15ee6-155">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="15ee6-155">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="15ee6-156">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="15ee6-156">The platform of the Device.</span></span> <span data-ttu-id="15ee6-157">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="15ee6-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="15ee6-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="15ee6-158">createdDateTime</span></span>|<span data-ttu-id="15ee6-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15ee6-159">DateTimeOffset</span></span>|<span data-ttu-id="15ee6-160">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="15ee6-160">Profile creation time</span></span>|
|<span data-ttu-id="15ee6-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="15ee6-161">lastModifiedDateTime</span></span>|<span data-ttu-id="15ee6-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15ee6-162">DateTimeOffset</span></span>|<span data-ttu-id="15ee6-163">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="15ee6-163">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="15ee6-164">Relações</span><span class="sxs-lookup"><span data-stu-id="15ee6-164">Relationships</span></span>
|<span data-ttu-id="15ee6-165">Relação</span><span class="sxs-lookup"><span data-stu-id="15ee6-165">Relationship</span></span>|<span data-ttu-id="15ee6-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="15ee6-166">Type</span></span>|<span data-ttu-id="15ee6-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="15ee6-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ee6-168">assignments</span><span class="sxs-lookup"><span data-stu-id="15ee6-168">assignments</span></span>|<span data-ttu-id="15ee6-169">coleção [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="15ee6-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="15ee6-170">A lista de atribuições para este perfil.</span><span class="sxs-lookup"><span data-stu-id="15ee6-170">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="15ee6-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15ee6-171">JSON Representation</span></span>
<span data-ttu-id="15ee6-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15ee6-172">Here is a JSON representation of the resource.</span></span>
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



