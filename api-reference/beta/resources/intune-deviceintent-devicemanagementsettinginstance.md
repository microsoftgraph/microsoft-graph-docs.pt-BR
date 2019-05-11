---
title: tipo de recurso deviceManagementSettingInstance
description: Tipo base para uma instância de configuração
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b780fad1df833a1a5d431835364493ac5afc3c6b
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943330"
---
# <a name="devicemanagementsettinginstance-resource-type"></a><span data-ttu-id="50406-103">tipo de recurso deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="50406-103">deviceManagementSettingInstance resource type</span></span>

> <span data-ttu-id="50406-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="50406-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="50406-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="50406-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="50406-106">Tipo base para uma instância de configuração</span><span class="sxs-lookup"><span data-stu-id="50406-106">Base type for a setting instance</span></span>

## <a name="methods"></a><span data-ttu-id="50406-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="50406-107">Methods</span></span>
|<span data-ttu-id="50406-108">Método</span><span class="sxs-lookup"><span data-stu-id="50406-108">Method</span></span>|<span data-ttu-id="50406-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="50406-109">Return Type</span></span>|<span data-ttu-id="50406-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="50406-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="50406-111">Listar deviceManagementSettingInstances</span><span class="sxs-lookup"><span data-stu-id="50406-111">List deviceManagementSettingInstances</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|<span data-ttu-id="50406-112">coleção [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)</span><span class="sxs-lookup"><span data-stu-id="50406-112">[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) collection</span></span>|<span data-ttu-id="50406-113">Listar Propriedades e relações dos objetos [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="50406-113">List properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) objects.</span></span>|
|[<span data-ttu-id="50406-114">Obter deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="50406-114">Get deviceManagementSettingInstance</span></span>](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[<span data-ttu-id="50406-115">deviceManagementSettingInstance</span><span class="sxs-lookup"><span data-stu-id="50406-115">deviceManagementSettingInstance</span></span>](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|<span data-ttu-id="50406-116">Leia as propriedades e as relações do objeto [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) .</span><span class="sxs-lookup"><span data-stu-id="50406-116">Read properties and relationships of the [deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="50406-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="50406-117">Properties</span></span>
|<span data-ttu-id="50406-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="50406-118">Property</span></span>|<span data-ttu-id="50406-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="50406-119">Type</span></span>|<span data-ttu-id="50406-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="50406-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="50406-121">id</span><span class="sxs-lookup"><span data-stu-id="50406-121">id</span></span>|<span data-ttu-id="50406-122">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50406-122">String</span></span>|<span data-ttu-id="50406-123">A ID de instância da configuração</span><span class="sxs-lookup"><span data-stu-id="50406-123">The setting instance ID</span></span>|
|<span data-ttu-id="50406-124">DefinitionId</span><span class="sxs-lookup"><span data-stu-id="50406-124">definitionId</span></span>|<span data-ttu-id="50406-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50406-125">String</span></span>|<span data-ttu-id="50406-126">A ID da definição de configuração dessa instância</span><span class="sxs-lookup"><span data-stu-id="50406-126">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="50406-127">valueJson</span><span class="sxs-lookup"><span data-stu-id="50406-127">valueJson</span></span>|<span data-ttu-id="50406-128">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="50406-128">String</span></span>|<span data-ttu-id="50406-129">Representação JSON do valor</span><span class="sxs-lookup"><span data-stu-id="50406-129">JSON representation of the value</span></span>|

## <a name="relationships"></a><span data-ttu-id="50406-130">Relações</span><span class="sxs-lookup"><span data-stu-id="50406-130">Relationships</span></span>
<span data-ttu-id="50406-131">Nenhum</span><span class="sxs-lookup"><span data-stu-id="50406-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="50406-132">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="50406-132">JSON Representation</span></span>
<span data-ttu-id="50406-133">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="50406-133">Here is a JSON representation of the resource.</span></span>
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




