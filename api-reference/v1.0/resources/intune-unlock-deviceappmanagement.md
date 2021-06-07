---
title: Tipo de recurso deviceAppManagement
description: Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos e aplicativos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 238c5fbd6b4179dd0be320b5cf8cac6fd27eb9b7
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751758"
---
# <a name="deviceappmanagement-resource-type"></a><span data-ttu-id="99690-103">Tipo de recurso deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="99690-103">deviceAppManagement resource type</span></span>

<span data-ttu-id="99690-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99690-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99690-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="99690-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99690-106">Entidade singleton que atua como um contêiner para todas as funcionalidades de gerenciamento de dispositivos e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="99690-106">Singleton entity that acts as a container for all device and app management functionality.</span></span>

## <a name="methods"></a><span data-ttu-id="99690-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="99690-107">Methods</span></span>
|<span data-ttu-id="99690-108">Método</span><span class="sxs-lookup"><span data-stu-id="99690-108">Method</span></span>|<span data-ttu-id="99690-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="99690-109">Return Type</span></span>|<span data-ttu-id="99690-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="99690-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="99690-111">Obter deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="99690-111">Get deviceAppManagement</span></span>](../api/intune-unlock-deviceappmanagement-get.md)|[<span data-ttu-id="99690-112">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="99690-112">deviceAppManagement</span></span>](../resources/intune-unlock-deviceappmanagement.md)|<span data-ttu-id="99690-113">Ler propriedades e relações de objetos de [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="99690-113">Read properties and relationships of the [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>|
|[<span data-ttu-id="99690-114">Atualizar deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="99690-114">Update deviceAppManagement</span></span>](../api/intune-unlock-deviceappmanagement-update.md)|[<span data-ttu-id="99690-115">deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="99690-115">deviceAppManagement</span></span>](../resources/intune-unlock-deviceappmanagement.md)|<span data-ttu-id="99690-116">Atualizar as propriedades de um objeto de [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md).</span><span class="sxs-lookup"><span data-stu-id="99690-116">Update the properties of a [deviceAppManagement](../resources/intune-unlock-deviceappmanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="99690-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="99690-117">Properties</span></span>
|<span data-ttu-id="99690-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="99690-118">Property</span></span>|<span data-ttu-id="99690-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="99690-119">Type</span></span>|<span data-ttu-id="99690-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="99690-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99690-121">id</span><span class="sxs-lookup"><span data-stu-id="99690-121">id</span></span>|<span data-ttu-id="99690-122">String</span><span class="sxs-lookup"><span data-stu-id="99690-122">String</span></span>|<span data-ttu-id="99690-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="99690-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99690-124">Relações</span><span class="sxs-lookup"><span data-stu-id="99690-124">Relationships</span></span>
<span data-ttu-id="99690-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="99690-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="99690-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="99690-126">JSON Representation</span></span>
<span data-ttu-id="99690-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="99690-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceAppManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "String (identifier)"
}
```




