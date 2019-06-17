---
title: tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 435b23cd3d8767d381137879f6eca5cdd345a676
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991790"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="bc0ed-103">tipo de recurso mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="bc0ed-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="bc0ed-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc0ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc0ed-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc0ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc0ed-106">Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="bc0ed-106">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="bc0ed-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="bc0ed-107">Methods</span></span>
|<span data-ttu-id="bc0ed-108">Método</span><span class="sxs-lookup"><span data-stu-id="bc0ed-108">Method</span></span>|<span data-ttu-id="bc0ed-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="bc0ed-109">Return Type</span></span>|<span data-ttu-id="bc0ed-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0ed-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="bc0ed-111">Listar mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="bc0ed-111">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="bc0ed-112">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="bc0ed-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="bc0ed-113">Listar Propriedades e relações dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bc0ed-113">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="bc0ed-114">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="bc0ed-114">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="bc0ed-115">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="bc0ed-115">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="bc0ed-116">Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="bc0ed-116">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="bc0ed-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc0ed-117">Properties</span></span>
|<span data-ttu-id="bc0ed-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc0ed-118">Property</span></span>|<span data-ttu-id="bc0ed-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc0ed-119">Type</span></span>|<span data-ttu-id="bc0ed-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc0ed-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc0ed-121">id</span><span class="sxs-lookup"><span data-stu-id="bc0ed-121">id</span></span>|<span data-ttu-id="bc0ed-122">String</span><span class="sxs-lookup"><span data-stu-id="bc0ed-122">String</span></span>|<span data-ttu-id="bc0ed-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="bc0ed-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc0ed-124">Relações</span><span class="sxs-lookup"><span data-stu-id="bc0ed-124">Relationships</span></span>
<span data-ttu-id="bc0ed-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc0ed-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc0ed-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc0ed-126">JSON Representation</span></span>
<span data-ttu-id="bc0ed-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc0ed-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mobileContainedApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileContainedApp",
  "id": "String (identifier)"
}
```





