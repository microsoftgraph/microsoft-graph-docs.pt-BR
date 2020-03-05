---
title: Tipo de recurso deviceEnrollmentConfiguration
description: A classe base da configuração de registro do dispositivo
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: bd21f5dea3bab467abf1b19754ada88a4fbb531a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523713"
---
# <a name="deviceenrollmentconfiguration-resource-type"></a><span data-ttu-id="255f5-103">Tipo de recurso deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="255f5-103">deviceEnrollmentConfiguration resource type</span></span>

<span data-ttu-id="255f5-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="255f5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="255f5-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="255f5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="255f5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="255f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="255f5-107">A classe base da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-107">The Base Class of Device Enrollment Configuration</span></span>

## <a name="methods"></a><span data-ttu-id="255f5-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="255f5-108">Methods</span></span>
|<span data-ttu-id="255f5-109">Método</span><span class="sxs-lookup"><span data-stu-id="255f5-109">Method</span></span>|<span data-ttu-id="255f5-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="255f5-110">Return Type</span></span>|<span data-ttu-id="255f5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="255f5-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="255f5-112">Listar deviceEnrollmentConfigurations</span><span class="sxs-lookup"><span data-stu-id="255f5-112">List deviceEnrollmentConfigurations</span></span>](../api/intune-shared-deviceenrollmentconfiguration-list.md)|<span data-ttu-id="255f5-113">Conjunto [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="255f5-113">[deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) collection</span></span>|<span data-ttu-id="255f5-114">Listar propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="255f5-114">List properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="255f5-115">Obter deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="255f5-115">Get deviceEnrollmentConfiguration</span></span>](../api/intune-shared-deviceenrollmentconfiguration-get.md)|[<span data-ttu-id="255f5-116">deviceEnrollmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="255f5-116">deviceEnrollmentConfiguration</span></span>](../resources/intune-shared-deviceenrollmentconfiguration.md)|<span data-ttu-id="255f5-117">Ler propriedades e relações de objetos de [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="255f5-117">Read properties and relationships of the [deviceEnrollmentConfiguration](../resources/intune-shared-deviceenrollmentconfiguration.md) object.</span></span>|
|<span data-ttu-id="255f5-118">**Integração**</span><span class="sxs-lookup"><span data-stu-id="255f5-118">**Onboarding**</span></span>|
|[<span data-ttu-id="255f5-119">Ação setPriority</span><span class="sxs-lookup"><span data-stu-id="255f5-119">setPriority action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-setpriority.md)|<span data-ttu-id="255f5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="255f5-120">None</span></span>|<span data-ttu-id="255f5-121">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="255f5-121">Not yet documented</span></span>|
|[<span data-ttu-id="255f5-122">atribuir ação</span><span class="sxs-lookup"><span data-stu-id="255f5-122">assign action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-assign.md)|<span data-ttu-id="255f5-123">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="255f5-123">None</span></span>|<span data-ttu-id="255f5-124">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="255f5-124">Not yet documented</span></span>|
|<span data-ttu-id="255f5-125">**Conjunto de políticas**</span><span class="sxs-lookup"><span data-stu-id="255f5-125">**Policy Set**</span></span>|
|[<span data-ttu-id="255f5-126">ação hasPayloadLinks</span><span class="sxs-lookup"><span data-stu-id="255f5-126">hasPayloadLinks action</span></span>](../api/intune-shared-deviceenrollmentconfiguration-haspayloadlinks.md)|<span data-ttu-id="255f5-127">coleção [hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md)</span><span class="sxs-lookup"><span data-stu-id="255f5-127">[hasPayloadLinkResultItem](../resources/intune-policyset-haspayloadlinkresultitem.md) collection</span></span>|<span data-ttu-id="255f5-128">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="255f5-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="255f5-129">Propriedades</span><span class="sxs-lookup"><span data-stu-id="255f5-129">Properties</span></span>
|<span data-ttu-id="255f5-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="255f5-130">Property</span></span>|<span data-ttu-id="255f5-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="255f5-131">Type</span></span>|<span data-ttu-id="255f5-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="255f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="255f5-133">id</span><span class="sxs-lookup"><span data-stu-id="255f5-133">id</span></span>|<span data-ttu-id="255f5-134">String</span><span class="sxs-lookup"><span data-stu-id="255f5-134">String</span></span>|<span data-ttu-id="255f5-135">Identificador exclusivo para a conta</span><span class="sxs-lookup"><span data-stu-id="255f5-135">Unique Identifier for the account</span></span>|
|<span data-ttu-id="255f5-136">displayName</span><span class="sxs-lookup"><span data-stu-id="255f5-136">displayName</span></span>|<span data-ttu-id="255f5-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="255f5-137">String</span></span>|<span data-ttu-id="255f5-138">O nome de exibição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-138">The display name of the device enrollment configuration</span></span>|
|<span data-ttu-id="255f5-139">description</span><span class="sxs-lookup"><span data-stu-id="255f5-139">description</span></span>|<span data-ttu-id="255f5-140">String</span><span class="sxs-lookup"><span data-stu-id="255f5-140">String</span></span>|<span data-ttu-id="255f5-141">A descrição da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-141">The description of the device enrollment configuration</span></span>|
|<span data-ttu-id="255f5-142">prioridade</span><span class="sxs-lookup"><span data-stu-id="255f5-142">priority</span></span>|<span data-ttu-id="255f5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="255f5-143">Int32</span></span>|<span data-ttu-id="255f5-144">A prioridade é usada quando um usuário existe em vários grupos que são atribuídos à configuração de registro.</span><span class="sxs-lookup"><span data-stu-id="255f5-144">Priority is used when a user exists in multiple groups that are assigned enrollment configuration.</span></span> <span data-ttu-id="255f5-145">Os usuários estão sujeitos somente à configuração com o menor valor de prioridade.</span><span class="sxs-lookup"><span data-stu-id="255f5-145">Users are subject only to the configuration with the lowest priority value.</span></span>|
|<span data-ttu-id="255f5-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="255f5-146">createdDateTime</span></span>|<span data-ttu-id="255f5-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="255f5-147">DateTimeOffset</span></span>|<span data-ttu-id="255f5-148">Data e hora de criação em UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-148">Created date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="255f5-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="255f5-149">lastModifiedDateTime</span></span>|<span data-ttu-id="255f5-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="255f5-150">DateTimeOffset</span></span>|<span data-ttu-id="255f5-151">Data e hora da última modificação em UTC da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-151">Last modified date time in UTC of the device enrollment configuration</span></span>|
|<span data-ttu-id="255f5-152">versão</span><span class="sxs-lookup"><span data-stu-id="255f5-152">version</span></span>|<span data-ttu-id="255f5-153">Int32</span><span class="sxs-lookup"><span data-stu-id="255f5-153">Int32</span></span>|<span data-ttu-id="255f5-154">A versão da configuração de registro do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-154">The version of the device enrollment configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="255f5-155">Relações</span><span class="sxs-lookup"><span data-stu-id="255f5-155">Relationships</span></span>
|<span data-ttu-id="255f5-156">Relação</span><span class="sxs-lookup"><span data-stu-id="255f5-156">Relationship</span></span>|<span data-ttu-id="255f5-157">Tipo</span><span class="sxs-lookup"><span data-stu-id="255f5-157">Type</span></span>|<span data-ttu-id="255f5-158">Descrição</span><span class="sxs-lookup"><span data-stu-id="255f5-158">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="255f5-159">**Integração**</span><span class="sxs-lookup"><span data-stu-id="255f5-159">**Onboarding**</span></span>|
|<span data-ttu-id="255f5-160">atribuições</span><span class="sxs-lookup"><span data-stu-id="255f5-160">assignments</span></span>|<span data-ttu-id="255f5-161">Conjunto [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md)</span><span class="sxs-lookup"><span data-stu-id="255f5-161">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="255f5-162">A lista de atribuições de grupo para o perfil de configuração do dispositivo</span><span class="sxs-lookup"><span data-stu-id="255f5-162">The list of group assignments for the device configuration profile</span></span>|

## <a name="json-representation"></a><span data-ttu-id="255f5-163">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="255f5-163">JSON Representation</span></span>
<span data-ttu-id="255f5-164">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="255f5-164">Here is a JSON representation of the resource.</span></span>
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



