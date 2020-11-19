---
title: tipo de recurso windows10XCertificateProfile
description: Tipo de perfil básico para certificados de autenticação (SCEP ou PFX de criação)
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 840b898599ec6fc97e6d1c6eba2d1f94cd84329f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301368"
---
# <a name="windows10xcertificateprofile-resource-type"></a><span data-ttu-id="dbb51-103">tipo de recurso windows10XCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="dbb51-103">windows10XCertificateProfile resource type</span></span>

<span data-ttu-id="dbb51-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dbb51-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dbb51-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="dbb51-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dbb51-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="dbb51-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dbb51-107">Tipo de perfil básico para certificados de autenticação (SCEP ou PFX de criação)</span><span class="sxs-lookup"><span data-stu-id="dbb51-107">Base Profile Type for Authentication Certificates (SCEP or PFX Create)</span></span>


<span data-ttu-id="dbb51-108">Herda de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-108">Inherits from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>

## <a name="methods"></a><span data-ttu-id="dbb51-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="dbb51-109">Methods</span></span>
|<span data-ttu-id="dbb51-110">Método</span><span class="sxs-lookup"><span data-stu-id="dbb51-110">Method</span></span>|<span data-ttu-id="dbb51-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="dbb51-111">Return Type</span></span>|<span data-ttu-id="dbb51-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb51-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="dbb51-113">Listar windows10XCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="dbb51-113">List windows10XCertificateProfiles</span></span>](../api/intune-rapolicy-windows10xcertificateprofile-list.md)|<span data-ttu-id="dbb51-114">coleção [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-114">[windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) collection</span></span>|<span data-ttu-id="dbb51-115">Listar Propriedades e relações dos objetos [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="dbb51-115">List properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) objects.</span></span>|
|[<span data-ttu-id="dbb51-116">Obter windows10XCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="dbb51-116">Get windows10XCertificateProfile</span></span>](../api/intune-rapolicy-windows10xcertificateprofile-get.md)|[<span data-ttu-id="dbb51-117">windows10XCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="dbb51-117">windows10XCertificateProfile</span></span>](../resources/intune-rapolicy-windows10xcertificateprofile.md)|<span data-ttu-id="dbb51-118">Leia as propriedades e as relações do objeto [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) .</span><span class="sxs-lookup"><span data-stu-id="dbb51-118">Read properties and relationships of the [windows10XCertificateProfile](../resources/intune-rapolicy-windows10xcertificateprofile.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="dbb51-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="dbb51-119">Properties</span></span>
|<span data-ttu-id="dbb51-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="dbb51-120">Property</span></span>|<span data-ttu-id="dbb51-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb51-121">Type</span></span>|<span data-ttu-id="dbb51-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb51-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb51-123">id</span><span class="sxs-lookup"><span data-stu-id="dbb51-123">id</span></span>|<span data-ttu-id="dbb51-124">String</span><span class="sxs-lookup"><span data-stu-id="dbb51-124">String</span></span>|<span data-ttu-id="dbb51-125">Identificador de perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-125">Profile identifier Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="dbb51-126">versão</span><span class="sxs-lookup"><span data-stu-id="dbb51-126">version</span></span>|<span data-ttu-id="dbb51-127">Int32</span><span class="sxs-lookup"><span data-stu-id="dbb51-127">Int32</span></span>|<span data-ttu-id="dbb51-128">Versão do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-128">Version of the profile Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="dbb51-129">displayName</span><span class="sxs-lookup"><span data-stu-id="dbb51-129">displayName</span></span>|<span data-ttu-id="dbb51-130">String</span><span class="sxs-lookup"><span data-stu-id="dbb51-130">String</span></span>|<span data-ttu-id="dbb51-131">Nome de exibição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-131">Profile display name Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="dbb51-132">description</span><span class="sxs-lookup"><span data-stu-id="dbb51-132">description</span></span>|<span data-ttu-id="dbb51-133">String</span><span class="sxs-lookup"><span data-stu-id="dbb51-133">String</span></span>|<span data-ttu-id="dbb51-134">Descrição do perfil herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-134">Profile description Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="dbb51-135">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="dbb51-135">creationDateTime</span></span>|<span data-ttu-id="dbb51-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbb51-136">DateTimeOffset</span></span>|<span data-ttu-id="dbb51-137">O perfil DateTime foi criado herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-137">DateTime profile was created Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="dbb51-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dbb51-138">lastModifiedDateTime</span></span>|<span data-ttu-id="dbb51-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dbb51-139">DateTimeOffset</span></span>|<span data-ttu-id="dbb51-140">O perfil DateTime foi modificado pela última vez de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-140">DateTime profile was last modified Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|
|<span data-ttu-id="dbb51-141">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dbb51-141">roleScopeTagIds</span></span>|<span data-ttu-id="dbb51-142">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="dbb51-142">String collection</span></span>|<span data-ttu-id="dbb51-143">Marcas de escopo herdadas de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-143">Scope Tags Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|

## <a name="relationships"></a><span data-ttu-id="dbb51-144">Relações</span><span class="sxs-lookup"><span data-stu-id="dbb51-144">Relationships</span></span>
|<span data-ttu-id="dbb51-145">Relação</span><span class="sxs-lookup"><span data-stu-id="dbb51-145">Relationship</span></span>|<span data-ttu-id="dbb51-146">Tipo</span><span class="sxs-lookup"><span data-stu-id="dbb51-146">Type</span></span>|<span data-ttu-id="dbb51-147">Descrição</span><span class="sxs-lookup"><span data-stu-id="dbb51-147">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dbb51-148">assignments</span><span class="sxs-lookup"><span data-stu-id="dbb51-148">assignments</span></span>|<span data-ttu-id="dbb51-149">coleção [deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-149">[deviceManagementResourceAccessProfileAssignment](../resources/intune-rapolicy-devicemanagementresourceaccessprofileassignment.md) collection</span></span>|<span data-ttu-id="dbb51-150">A lista de atribuições para o perfil de configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="dbb51-150">The list of assignments for the device configuration profile.</span></span> <span data-ttu-id="dbb51-151">Herdado de [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span><span class="sxs-lookup"><span data-stu-id="dbb51-151">Inherited from [deviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-devicemanagementresourceaccessprofilebase.md)</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dbb51-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="dbb51-152">JSON Representation</span></span>
<span data-ttu-id="dbb51-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="dbb51-153">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10XCertificateProfile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCertificateProfile",
  "id": "String (identifier)",
  "version": 1024,
  "displayName": "String",
  "description": "String",
  "creationDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ]
}
```




