---
title: Tipo de recurso deviceManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos e aplicativos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2bfc2ddb9f3883f2157a451edc53ea4b33590371
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751751"
---
# <a name="devicemanagement-resource-type"></a><span data-ttu-id="75a57-103">Tipo de recurso deviceManagement</span><span class="sxs-lookup"><span data-stu-id="75a57-103">deviceManagement resource type</span></span>

<span data-ttu-id="75a57-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="75a57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="75a57-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="75a57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="75a57-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="75a57-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="75a57-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="75a57-107">Methods</span></span>
|<span data-ttu-id="75a57-108">Método</span><span class="sxs-lookup"><span data-stu-id="75a57-108">Method</span></span>|<span data-ttu-id="75a57-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="75a57-109">Return Type</span></span>|<span data-ttu-id="75a57-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a57-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="75a57-111">Obter deviceManagement</span><span class="sxs-lookup"><span data-stu-id="75a57-111">Get deviceManagement</span></span>](../api/intune-policyset-devicemanagement-get.md)|[<span data-ttu-id="75a57-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="75a57-112">deviceManagement</span></span>](../resources/intune-policyset-devicemanagement.md)|<span data-ttu-id="75a57-113">Leia as propriedades e as relações do objeto [deviceManagement](../resources/intune-policyset-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="75a57-113">Read properties and relationships of the [deviceManagement](../resources/intune-policyset-devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="75a57-114">Atualizar deviceManagement</span><span class="sxs-lookup"><span data-stu-id="75a57-114">Update deviceManagement</span></span>](../api/intune-policyset-devicemanagement-update.md)|[<span data-ttu-id="75a57-115">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="75a57-115">deviceManagement</span></span>](../resources/intune-policyset-devicemanagement.md)|<span data-ttu-id="75a57-116">Atualizar as propriedades de um objeto de [deviceManagement](../resources/intune-policyset-devicemanagement.md).</span><span class="sxs-lookup"><span data-stu-id="75a57-116">Update the properties of a [deviceManagement](../resources/intune-policyset-devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="75a57-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="75a57-117">Properties</span></span>
|<span data-ttu-id="75a57-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="75a57-118">Property</span></span>|<span data-ttu-id="75a57-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="75a57-119">Type</span></span>|<span data-ttu-id="75a57-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="75a57-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="75a57-121">id</span><span class="sxs-lookup"><span data-stu-id="75a57-121">id</span></span>|<span data-ttu-id="75a57-122">String</span><span class="sxs-lookup"><span data-stu-id="75a57-122">String</span></span>|<span data-ttu-id="75a57-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="75a57-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="75a57-124">Relações</span><span class="sxs-lookup"><span data-stu-id="75a57-124">Relationships</span></span>
<span data-ttu-id="75a57-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="75a57-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="75a57-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="75a57-126">JSON Representation</span></span>
<span data-ttu-id="75a57-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="75a57-127">Here is a JSON representation of the resource.</span></span>
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




