---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76e65eb3d4d49644d8f6350ad838b53c5990eee5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752836"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="18d02-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="18d02-103">deviceManagement resource type</span></span>

<span data-ttu-id="18d02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="18d02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="18d02-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="18d02-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18d02-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="18d02-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="18d02-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="18d02-107">Methods</span></span>
|<span data-ttu-id="18d02-108">Método</span><span class="sxs-lookup"><span data-stu-id="18d02-108">Method</span></span>|<span data-ttu-id="18d02-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="18d02-109">Return Type</span></span>|<span data-ttu-id="18d02-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d02-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="18d02-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="18d02-111">Get deviceManagement</span></span>](../api/intune-reporting-devicemanagement-get.md)|[<span data-ttu-id="18d02-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="18d02-112">deviceManagement</span></span>](../resources/intune-reporting-devicemanagement.md)|<span data-ttu-id="18d02-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-reporting-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="18d02-113">Read properties and relationships of the [deviceManagement](../resources/intune-reporting-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="18d02-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="18d02-114">Update deviceManagement</span></span>](../api/intune-reporting-devicemanagement-update.md)|[<span data-ttu-id="18d02-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="18d02-115">deviceManagement</span></span>](../resources/intune-reporting-devicemanagement.md)|<span data-ttu-id="18d02-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-reporting-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="18d02-116">Update the properties of a [deviceManagement](../resources/intune-reporting-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="18d02-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="18d02-117">Properties</span></span>
|<span data-ttu-id="18d02-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="18d02-118">Property</span></span>|<span data-ttu-id="18d02-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d02-119">Type</span></span>|<span data-ttu-id="18d02-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d02-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d02-121">id</span><span class="sxs-lookup"><span data-stu-id="18d02-121">id</span></span>|<span data-ttu-id="18d02-122">String</span><span class="sxs-lookup"><span data-stu-id="18d02-122">String</span></span>|<span data-ttu-id="18d02-123">Identificador exclusivo dessa entidade</span><span class="sxs-lookup"><span data-stu-id="18d02-123">Unique identifier for this entity</span></span>|

## <a name="relationships"></a><span data-ttu-id="18d02-124">Relações</span><span class="sxs-lookup"><span data-stu-id="18d02-124">Relationships</span></span>
|<span data-ttu-id="18d02-125">Relação</span><span class="sxs-lookup"><span data-stu-id="18d02-125">Relationship</span></span>|<span data-ttu-id="18d02-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="18d02-126">Type</span></span>|<span data-ttu-id="18d02-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="18d02-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18d02-128">reports</span><span class="sxs-lookup"><span data-stu-id="18d02-128">reports</span></span>|[<span data-ttu-id="18d02-129">deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="18d02-129">deviceManagementReports</span></span>](../resources/intune-reporting-devicemanagementreports.md)|<span data-ttu-id="18d02-130">Singleton de relatórios</span><span class="sxs-lookup"><span data-stu-id="18d02-130">Reports singleton</span></span>|

## <a name="json-representation"></a><span data-ttu-id="18d02-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="18d02-131">JSON Representation</span></span>
<span data-ttu-id="18d02-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="18d02-132">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```




