---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5624105adff6d86fc52f713a90cb203bcf022044
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48705642"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="3f1c0-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="3f1c0-103">deviceManagementSettingInstance resource type</span></span>

<span data-ttu-id="3f1c0-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f1c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3f1c0-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="3f1c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3f1c0-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3f1c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f1c0-107">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="3f1c0-107">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="3f1c0-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="3f1c0-108">Methods</span></span>
|<span data-ttu-id="3f1c0-109">Método</span><span class="sxs-lookup"><span data-stu-id="3f1c0-109">Method</span></span>|<span data-ttu-id="3f1c0-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="3f1c0-110">Return Type</span></span>|<span data-ttu-id="3f1c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f1c0-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="3f1c0-112">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="3f1c0-112">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="3f1c0-113">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="3f1c0-113">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="3f1c0-114">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="3f1c0-114">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="3f1c0-115">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="3f1c0-115">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="3f1c0-116">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="3f1c0-116">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="3f1c0-117">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="3f1c0-117">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f1c0-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3f1c0-118">Properties</span></span>
|<span data-ttu-id="3f1c0-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3f1c0-119">Property</span></span>|<span data-ttu-id="3f1c0-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="3f1c0-120">Type</span></span>|<span data-ttu-id="3f1c0-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="3f1c0-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f1c0-122">id</span><span class="sxs-lookup"><span data-stu-id="3f1c0-122">id</span></span>|<span data-ttu-id="3f1c0-123">String</span><span class="sxs-lookup"><span data-stu-id="3f1c0-123">String</span></span>|<span data-ttu-id="3f1c0-124">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="3f1c0-124">The setting instance ID</span></span>|
|<span data-ttu-id="3f1c0-125">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="3f1c0-125">definitionId</span></span>|<span data-ttu-id="3f1c0-126">String</span><span class="sxs-lookup"><span data-stu-id="3f1c0-126">String</span></span>|<span data-ttu-id="3f1c0-127">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="3f1c0-127">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="3f1c0-128">valueJson</span><span class="sxs-lookup"><span data-stu-id="3f1c0-128">valueJson</span></span>|<span data-ttu-id="3f1c0-129">String</span><span class="sxs-lookup"><span data-stu-id="3f1c0-129">String</span></span>|<span data-ttu-id="3f1c0-130">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="3f1c0-130">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f1c0-131">Relações</span><span class="sxs-lookup"><span data-stu-id="3f1c0-131">Relationships</span></span>
<span data-ttu-id="3f1c0-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3f1c0-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f1c0-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3f1c0-133">JSON Representation</span></span>
<span data-ttu-id="3f1c0-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3f1c0-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```





