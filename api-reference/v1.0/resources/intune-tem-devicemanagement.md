---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 847ba54fd3cb755d6ade878112e15deffb5d8812
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757439"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="5171f-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5171f-103">deviceManagement resource type</span></span>

<span data-ttu-id="5171f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5171f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5171f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="5171f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5171f-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos.</span><span class="sxs-lookup"><span data-stu-id="5171f-106">Singleton entity that acts as a container for all device management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="5171f-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="5171f-107">Methods</span></span>
|<span data-ttu-id="5171f-108">Método</span><span class="sxs-lookup"><span data-stu-id="5171f-108">Method</span></span>|<span data-ttu-id="5171f-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5171f-109">Return Type</span></span>|<span data-ttu-id="5171f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="5171f-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5171f-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5171f-111">Get deviceManagement</span></span>](../api/intune-tem-devicemanagement-get.md)|[<span data-ttu-id="5171f-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5171f-112">deviceManagement</span></span>](../resources/intune-tem-devicemanagement.md)|<span data-ttu-id="5171f-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-tem-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5171f-113">Read properties and relationships of the [deviceManagement](../resources/intune-tem-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="5171f-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5171f-114">Update deviceManagement</span></span>](../api/intune-tem-devicemanagement-update.md)|[<span data-ttu-id="5171f-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="5171f-115">deviceManagement</span></span>](../resources/intune-tem-devicemanagement.md)|<span data-ttu-id="5171f-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-tem-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="5171f-116">Update the properties of a [deviceManagement](../resources/intune-tem-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5171f-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5171f-117">Properties</span></span>
|<span data-ttu-id="5171f-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5171f-118">Property</span></span>|<span data-ttu-id="5171f-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="5171f-119">Type</span></span>|<span data-ttu-id="5171f-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="5171f-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5171f-121">id</span><span class="sxs-lookup"><span data-stu-id="5171f-121">id</span></span>|<span data-ttu-id="5171f-122">String</span><span class="sxs-lookup"><span data-stu-id="5171f-122">String</span></span>|<span data-ttu-id="5171f-123">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="5171f-123">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="5171f-124">Relações</span><span class="sxs-lookup"><span data-stu-id="5171f-124">Relationships</span></span>
|<span data-ttu-id="5171f-125">Relação</span><span class="sxs-lookup"><span data-stu-id="5171f-125">Relationship</span></span>|<span data-ttu-id="5171f-126">Tipo</span><span class="sxs-lookup"><span data-stu-id="5171f-126">Type</span></span>|<span data-ttu-id="5171f-127">Descrição</span><span class="sxs-lookup"><span data-stu-id="5171f-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5171f-128">telecomExpenseManagementPartners</span><span class="sxs-lookup"><span data-stu-id="5171f-128">telecomExpenseManagementPartners</span></span>|<span data-ttu-id="5171f-129">Conjunto [telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md)</span><span class="sxs-lookup"><span data-stu-id="5171f-129">[telecomExpenseManagementPartner](../resources/intune-tem-telecomexpensemanagementpartner.md) collection</span></span>|<span data-ttu-id="5171f-130">Os parceiros de gerenciamento de despesas de telecomunicações.</span><span class="sxs-lookup"><span data-stu-id="5171f-130">The telecom expense management partners.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5171f-131">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5171f-131">JSON Representation</span></span>
<span data-ttu-id="5171f-132">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5171f-132">Here is a JSON representation of the resource.</span></span>
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




