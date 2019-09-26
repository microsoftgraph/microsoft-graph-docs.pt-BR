---
title: tipo de recurso appleUserInitiatedEnrollmentProfile
description: O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas. As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ed568d5d8169623b5ff3e006d22cdfe5cecd4a47
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199664"
---
# <a name="appleuserinitiatedenrollmentprofile-resource-type"></a><span data-ttu-id="78f08-104">tipo de recurso appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-104">appleUserInitiatedEnrollmentProfile resource type</span></span>

> <span data-ttu-id="78f08-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="78f08-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="78f08-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="78f08-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="78f08-107">O recurso enrollmentProfile representa uma coleção de configurações que devem ser fornecidas como pré-registro para habilitar a inscrição de determinados dispositivos cujas identidades foram pré-configuradas.</span><span class="sxs-lookup"><span data-stu-id="78f08-107">The enrollmentProfile resource represents a collection of configurations which must be provided pre-enrollment to enable enrolling certain devices whose identities have been pre-staged.</span></span> <span data-ttu-id="78f08-108">As identidades de dispositivo pré-configuradas são atribuídas a esse tipo de perfil para aplicar as configurações do perfil no registro do dispositivo correspondente.</span><span class="sxs-lookup"><span data-stu-id="78f08-108">Pre-staged device identities are assigned to this type of profile to apply the profile's configurations at enrollment of the corresponding device.</span></span>

## <a name="methods"></a><span data-ttu-id="78f08-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="78f08-109">Methods</span></span>
|<span data-ttu-id="78f08-110">Método</span><span class="sxs-lookup"><span data-stu-id="78f08-110">Method</span></span>|<span data-ttu-id="78f08-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="78f08-111">Return Type</span></span>|<span data-ttu-id="78f08-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f08-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="78f08-113">Listar appleUserInitiatedEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="78f08-113">List appleUserInitiatedEnrollmentProfiles</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-list.md)|<span data-ttu-id="78f08-114">coleção [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)</span><span class="sxs-lookup"><span data-stu-id="78f08-114">[appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) collection</span></span>|<span data-ttu-id="78f08-115">Listar Propriedades e relações dos objetos [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="78f08-115">List properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) objects.</span></span>|
|[<span data-ttu-id="78f08-116">Obter appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-116">Get appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-get.md)|[<span data-ttu-id="78f08-117">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-117">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="78f08-118">Leia as propriedades e as relações do objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="78f08-118">Read properties and relationships of the [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="78f08-119">Criar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-119">Create appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-create.md)|[<span data-ttu-id="78f08-120">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-120">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="78f08-121">Criar um novo objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="78f08-121">Create a new [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="78f08-122">Excluir appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-122">Delete appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-delete.md)|<span data-ttu-id="78f08-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78f08-123">None</span></span>|<span data-ttu-id="78f08-124">Exclui [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span><span class="sxs-lookup"><span data-stu-id="78f08-124">Deletes a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md).</span></span>|
|[<span data-ttu-id="78f08-125">Atualizar appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-125">Update appleUserInitiatedEnrollmentProfile</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-update.md)|[<span data-ttu-id="78f08-126">appleUserInitiatedEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="78f08-126">appleUserInitiatedEnrollmentProfile</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md)|<span data-ttu-id="78f08-127">Atualiza as propriedades de um objeto [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="78f08-127">Update the properties of a [appleUserInitiatedEnrollmentProfile](../resources/intune-enrollment-appleuserinitiatedenrollmentprofile.md) object.</span></span>|
|[<span data-ttu-id="78f08-128">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="78f08-128">setPriority action</span></span>](../api/intune-enrollment-appleuserinitiatedenrollmentprofile-setpriority.md)|<span data-ttu-id="78f08-129">Nenhum</span><span class="sxs-lookup"><span data-stu-id="78f08-129">None</span></span>|<span data-ttu-id="78f08-130">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="78f08-130">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="78f08-131">Propriedades</span><span class="sxs-lookup"><span data-stu-id="78f08-131">Properties</span></span>
|<span data-ttu-id="78f08-132">Propriedade</span><span class="sxs-lookup"><span data-stu-id="78f08-132">Property</span></span>|<span data-ttu-id="78f08-133">Tipo</span><span class="sxs-lookup"><span data-stu-id="78f08-133">Type</span></span>|<span data-ttu-id="78f08-134">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f08-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78f08-135">defaultenrollmentidtype</span><span class="sxs-lookup"><span data-stu-id="78f08-135">defaultEnrollmentType</span></span>|[<span data-ttu-id="78f08-136">appleUserInitiatedEnrollmentType</span><span class="sxs-lookup"><span data-stu-id="78f08-136">appleUserInitiatedEnrollmentType</span></span>](../resources/intune-enrollment-appleuserinitiatedenrollmenttype.md)|<span data-ttu-id="78f08-137">O tipo de registro de perfil padrão.</span><span class="sxs-lookup"><span data-stu-id="78f08-137">The default profile enrollment type.</span></span> <span data-ttu-id="78f08-138">Os valores possíveis são: `unknown`, `device`, `user`.</span><span class="sxs-lookup"><span data-stu-id="78f08-138">Possible values are: `unknown`, `device`, `user`.</span></span>|
|<span data-ttu-id="78f08-139">availableEnrollmentTypeOptions</span><span class="sxs-lookup"><span data-stu-id="78f08-139">availableEnrollmentTypeOptions</span></span>|<span data-ttu-id="78f08-140">coleção [appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md)</span><span class="sxs-lookup"><span data-stu-id="78f08-140">[appleOwnerTypeEnrollmentType](../resources/intune-enrollment-appleownertypeenrollmenttype.md) collection</span></span>|<span data-ttu-id="78f08-141">Lista de opções de tipo de registro disponíveis</span><span class="sxs-lookup"><span data-stu-id="78f08-141">List of available enrollment type options</span></span>|
|<span data-ttu-id="78f08-142">id</span><span class="sxs-lookup"><span data-stu-id="78f08-142">id</span></span>|<span data-ttu-id="78f08-143">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="78f08-143">String</span></span>|<span data-ttu-id="78f08-144">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="78f08-144">The GUID for the object</span></span>|
|<span data-ttu-id="78f08-145">displayName</span><span class="sxs-lookup"><span data-stu-id="78f08-145">displayName</span></span>|<span data-ttu-id="78f08-146">String</span><span class="sxs-lookup"><span data-stu-id="78f08-146">String</span></span>|<span data-ttu-id="78f08-147">Nome do perfil</span><span class="sxs-lookup"><span data-stu-id="78f08-147">Name of the profile</span></span>|
|<span data-ttu-id="78f08-148">descrição</span><span class="sxs-lookup"><span data-stu-id="78f08-148">description</span></span>|<span data-ttu-id="78f08-149">String</span><span class="sxs-lookup"><span data-stu-id="78f08-149">String</span></span>|<span data-ttu-id="78f08-150">Descrição do perfil</span><span class="sxs-lookup"><span data-stu-id="78f08-150">Description of the profile</span></span>|
|<span data-ttu-id="78f08-151">prioridade</span><span class="sxs-lookup"><span data-stu-id="78f08-151">priority</span></span>|<span data-ttu-id="78f08-152">Int32</span><span class="sxs-lookup"><span data-stu-id="78f08-152">Int32</span></span>|<span data-ttu-id="78f08-153">Prioridade, 0 é a maior</span><span class="sxs-lookup"><span data-stu-id="78f08-153">Priority, 0 is highest</span></span>|
|<span data-ttu-id="78f08-154">platform</span><span class="sxs-lookup"><span data-stu-id="78f08-154">platform</span></span>|[<span data-ttu-id="78f08-155">devicePlatformType</span><span class="sxs-lookup"><span data-stu-id="78f08-155">devicePlatformType</span></span>](../resources/intune-shared-deviceplatformtype.md)|<span data-ttu-id="78f08-156">A plataforma do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="78f08-156">The platform of the Device.</span></span> <span data-ttu-id="78f08-157">Os valores possíveis são: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="78f08-157">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="78f08-158">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="78f08-158">createdDateTime</span></span>|<span data-ttu-id="78f08-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f08-159">DateTimeOffset</span></span>|<span data-ttu-id="78f08-160">Hora de criação do perfil</span><span class="sxs-lookup"><span data-stu-id="78f08-160">Profile creation time</span></span>|
|<span data-ttu-id="78f08-161">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="78f08-161">lastModifiedDateTime</span></span>|<span data-ttu-id="78f08-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="78f08-162">DateTimeOffset</span></span>|<span data-ttu-id="78f08-163">Hora da última modificação do perfil</span><span class="sxs-lookup"><span data-stu-id="78f08-163">Profile last modified time</span></span>|

## <a name="relationships"></a><span data-ttu-id="78f08-164">Relações</span><span class="sxs-lookup"><span data-stu-id="78f08-164">Relationships</span></span>
|<span data-ttu-id="78f08-165">Relação</span><span class="sxs-lookup"><span data-stu-id="78f08-165">Relationship</span></span>|<span data-ttu-id="78f08-166">Tipo</span><span class="sxs-lookup"><span data-stu-id="78f08-166">Type</span></span>|<span data-ttu-id="78f08-167">Descrição</span><span class="sxs-lookup"><span data-stu-id="78f08-167">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78f08-168">assignments</span><span class="sxs-lookup"><span data-stu-id="78f08-168">assignments</span></span>|<span data-ttu-id="78f08-169">coleção [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="78f08-169">[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) collection</span></span>|<span data-ttu-id="78f08-170">A lista de atribuições para este perfil.</span><span class="sxs-lookup"><span data-stu-id="78f08-170">The list of assignments for this profile.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="78f08-171">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="78f08-171">JSON Representation</span></span>
<span data-ttu-id="78f08-172">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="78f08-172">Here is a JSON representation of the resource.</span></span>
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



