---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b55c85abc632b149a4e397c007a4c7d4b79a6c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752831"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="e4fbd-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e4fbd-103">deviceManagement resource type</span></span>

<span data-ttu-id="e4fbd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e4fbd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e4fbd-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e4fbd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4fbd-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de aplicativos de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e4fbd-106">Singleton entity that acts as a container for all device app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="e4fbd-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e4fbd-107">Methods</span></span>
|<span data-ttu-id="e4fbd-108">Método</span><span class="sxs-lookup"><span data-stu-id="e4fbd-108">Method</span></span>|<span data-ttu-id="e4fbd-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e4fbd-109">Return Type</span></span>|<span data-ttu-id="e4fbd-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4fbd-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e4fbd-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e4fbd-111">Get deviceManagement</span></span>](../api/intune-auditing-devicemanagement-get.md)|[<span data-ttu-id="e4fbd-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e4fbd-112">deviceManagement</span></span>](../resources/intune-auditing-devicemanagement.md)|<span data-ttu-id="e4fbd-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-auditing-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e4fbd-113">Read properties and relationships of the [deviceManagement](../resources/intune-auditing-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="e4fbd-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e4fbd-114">Update deviceManagement</span></span>](../api/intune-auditing-devicemanagement-update.md)|[<span data-ttu-id="e4fbd-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="e4fbd-115">deviceManagement</span></span>](../resources/intune-auditing-devicemanagement.md)|<span data-ttu-id="e4fbd-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-auditing-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="e4fbd-116">Update the properties of a [deviceManagement](../resources/intune-auditing-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e4fbd-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e4fbd-117">Properties</span></span>
|<span data-ttu-id="e4fbd-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e4fbd-118">Property</span></span>|<span data-ttu-id="e4fbd-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4fbd-119">Type</span></span>|<span data-ttu-id="e4fbd-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4fbd-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4fbd-121">id</span><span class="sxs-lookup"><span data-stu-id="e4fbd-121">id</span></span>|<span data-ttu-id="e4fbd-122">String</span><span class="sxs-lookup"><span data-stu-id="e4fbd-122">String</span></span>|<span data-ttu-id="e4fbd-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e4fbd-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e4fbd-124">Relações</span><span class="sxs-lookup"><span data-stu-id="e4fbd-124">Relationships</span></span>
|<span data-ttu-id="e4fbd-125">Relação</span><span class="sxs-lookup"><span data-stu-id="e4fbd-125">Relationship</span></span>|<span data-ttu-id="e4fbd-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="e4fbd-126">Type</span></span>|<span data-ttu-id="e4fbd-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="e4fbd-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4fbd-128">auditEvents</span><span class="sxs-lookup"><span data-stu-id="e4fbd-128">auditEvents</span></span>|<span data-ttu-id="e4fbd-129">Conjunto [auditEvent](../resources/intune-auditing-auditevent.md)</span><span class="sxs-lookup"><span data-stu-id="e4fbd-129">[auditEvent](../resources/intune-auditing-auditevent.md) collection</span></span>|<span data-ttu-id="e4fbd-130">Eventos de auditoria</span><span class="sxs-lookup"><span data-stu-id="e4fbd-130">The Audit Events</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e4fbd-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e4fbd-131">JSON Representation</span></span>
<span data-ttu-id="e4fbd-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e4fbd-132">Here is a JSON representation of the resource.</span></span>
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




