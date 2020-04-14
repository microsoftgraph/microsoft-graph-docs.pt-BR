---
title: Tipo de recurso deviceEnrollmentConfiguration
description: A classe base da configuração de registro do dispositivo
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 95d806f2fef3723f89f43cf6b8cf721c224439a6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43356479"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="53319-103">Tipo de recurso deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="53319-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="53319-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53319-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53319-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="53319-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="53319-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="53319-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53319-107">A classe base da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="53319-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="53319-108">Methods</span></span>
|<span data-ttu-id="53319-109">Método</span><span class="sxs-lookup"><span data-stu-id="53319-109">Method</span></span>|<span data-ttu-id="53319-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="53319-110">Return Type</span></span>|<span data-ttu-id="53319-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="53319-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="53319-112">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="53319-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="53319-113">Conjunto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="53319-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="53319-114">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53319-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="53319-115">Obter deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="53319-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="53319-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="53319-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="53319-117">Ler propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="53319-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="53319-118">**Integração**</span><span class="sxs-lookup"><span data-stu-id="53319-118">**Onboarding**</span></span>|
|[<span data-ttu-id="53319-119">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="53319-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="53319-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="53319-120">None</span></span>|<span data-ttu-id="53319-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="53319-121">Not yet documented</span></span>|
|[<span data-ttu-id="53319-122">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="53319-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="53319-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="53319-123">None</span></span>|<span data-ttu-id="53319-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="53319-124">Not yet documented</span></span>|
|<span data-ttu-id="53319-125">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="53319-125">**Policy Set**</span></span>|
|[<span data-ttu-id="53319-126">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="53319-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="53319-127">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="53319-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="53319-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="53319-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="53319-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="53319-129">Properties</span></span>
|<span data-ttu-id="53319-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="53319-130">Property</span></span>|<span data-ttu-id="53319-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="53319-131">Type</span></span>|<span data-ttu-id="53319-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="53319-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53319-133">id</span><span class="sxs-lookup"><span data-stu-id="53319-133">id</span></span>|<span data-ttu-id="53319-134">String</span><span class="sxs-lookup"><span data-stu-id="53319-134">String</span></span>|<span data-ttu-id="53319-135">Identificador exclusivo para a conta</span><span class="sxs-lookup"><span data-stu-id="53319-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="53319-136">displayName</span><span class="sxs-lookup"><span data-stu-id="53319-136">displayName</span></span>|<span data-ttu-id="53319-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="53319-137">String</span></span>|<span data-ttu-id="53319-138">O nome de exibição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="53319-139">description</span><span class="sxs-lookup"><span data-stu-id="53319-139">description</span></span>|<span data-ttu-id="53319-140">String</span><span class="sxs-lookup"><span data-stu-id="53319-140">String</span></span>|<span data-ttu-id="53319-141">A descrição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="53319-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="53319-142">priority</span></span>|<span data-ttu-id="53319-143">Int32</span><span class="sxs-lookup"><span data-stu-id="53319-143">Int32</span></span>|<span data-ttu-id="53319-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="53319-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="53319-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="53319-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="53319-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="53319-146">createdDateTime</span></span>|<span data-ttu-id="53319-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53319-147">DateTimeOffset</span></span>|<span data-ttu-id="53319-148">Data e hora de criação em UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="53319-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="53319-149">lastModifiedDateTime</span></span>|<span data-ttu-id="53319-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="53319-150">DateTimeOffset</span></span>|<span data-ttu-id="53319-151">Data e hora da última modificação em UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="53319-152">versão</span><span class="sxs-lookup"><span data-stu-id="53319-152">version</span></span>|<span data-ttu-id="53319-153">Int32</span><span class="sxs-lookup"><span data-stu-id="53319-153">Int32</span></span>|<span data-ttu-id="53319-154">A versão da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="53319-155">Relações</span><span class="sxs-lookup"><span data-stu-id="53319-155">Relationships</span></span>
|<span data-ttu-id="53319-156">Relação</span><span class="sxs-lookup"><span data-stu-id="53319-156">Relationship</span></span>|<span data-ttu-id="53319-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="53319-157">Type</span></span>|<span data-ttu-id="53319-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="53319-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53319-159">**Integração**</span><span class="sxs-lookup"><span data-stu-id="53319-159">**Onboarding**</span></span>|
|<span data-ttu-id="53319-160">atribuições</span><span class="sxs-lookup"><span data-stu-id="53319-160">assignments</span></span>|<span data-ttu-id="53319-161">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="53319-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="53319-162">A lista de atribuições de grupo para o perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="53319-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="53319-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="53319-163">JSON Representation</span></span>
<span data-ttu-id="53319-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="53319-164">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceEnrollmentConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "priority": 1024,
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "version": 1024
}
```



