---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 28f380bc2aef749079676d4f97fd4bd6f3d7c671
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36364646"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="1fac5-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1fac5-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="1fac5-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1fac5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fac5-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fac5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fac5-106">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="1fac5-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="1fac5-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="1fac5-107">Methods</span></span>
|<span data-ttu-id="1fac5-108">Método</span><span class="sxs-lookup"><span data-stu-id="1fac5-108">Method</span></span>|<span data-ttu-id="1fac5-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="1fac5-109">Return Type</span></span>|<span data-ttu-id="1fac5-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fac5-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1fac5-111">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="1fac5-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="1fac5-112">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="1fac5-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="1fac5-113">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="1fac5-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="1fac5-114">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1fac5-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="1fac5-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="1fac5-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="1fac5-116">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="1fac5-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fac5-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fac5-117">Properties</span></span>
|<span data-ttu-id="1fac5-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fac5-118">Property</span></span>|<span data-ttu-id="1fac5-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fac5-119">Type</span></span>|<span data-ttu-id="1fac5-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fac5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fac5-121">id</span><span class="sxs-lookup"><span data-stu-id="1fac5-121">id</span></span>|<span data-ttu-id="1fac5-122">String</span><span class="sxs-lookup"><span data-stu-id="1fac5-122">String</span></span>|<span data-ttu-id="1fac5-123">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="1fac5-123">The setting instance ID</span></span>|
|<span data-ttu-id="1fac5-124">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="1fac5-124">definitionId</span></span>|<span data-ttu-id="1fac5-125">String</span><span class="sxs-lookup"><span data-stu-id="1fac5-125">String</span></span>|<span data-ttu-id="1fac5-126">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="1fac5-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="1fac5-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="1fac5-127">valueJson</span></span>|<span data-ttu-id="1fac5-128">String</span><span class="sxs-lookup"><span data-stu-id="1fac5-128">String</span></span>|<span data-ttu-id="1fac5-129">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="1fac5-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fac5-130">Relações</span><span class="sxs-lookup"><span data-stu-id="1fac5-130">Relationships</span></span>
<span data-ttu-id="1fac5-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fac5-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fac5-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fac5-132">JSON Representation</span></span>
<span data-ttu-id="1fac5-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fac5-133">Here is a JSON representation of the resource.</span></span>
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



