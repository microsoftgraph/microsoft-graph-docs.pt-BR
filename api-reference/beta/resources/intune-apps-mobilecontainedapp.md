---
title: tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 25078817c1add941a256ceb5f9f92cfd6b4426d7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49274163"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="9b483-103">tipo de recurso mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9b483-103">mobileContainedApp resource type</span></span>

<span data-ttu-id="9b483-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b483-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b483-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b483-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b483-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b483-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b483-107">Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="9b483-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="9b483-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="9b483-108">Methods</span></span>
|<span data-ttu-id="9b483-109">Método</span><span class="sxs-lookup"><span data-stu-id="9b483-109">Method</span></span>|<span data-ttu-id="9b483-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9b483-110">Return Type</span></span>|<span data-ttu-id="9b483-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b483-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9b483-112">Listar mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="9b483-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="9b483-113">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9b483-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="9b483-114">Listar Propriedades e relações dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9b483-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="9b483-115">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9b483-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="9b483-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9b483-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="9b483-117">Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9b483-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b483-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b483-118">Properties</span></span>
|<span data-ttu-id="9b483-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b483-119">Property</span></span>|<span data-ttu-id="9b483-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b483-120">Type</span></span>|<span data-ttu-id="9b483-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b483-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b483-122">id</span><span class="sxs-lookup"><span data-stu-id="9b483-122">id</span></span>|<span data-ttu-id="9b483-123">String</span><span class="sxs-lookup"><span data-stu-id="9b483-123">String</span></span>|<span data-ttu-id="9b483-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9b483-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b483-125">Relações</span><span class="sxs-lookup"><span data-stu-id="9b483-125">Relationships</span></span>
<span data-ttu-id="9b483-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b483-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b483-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b483-127">JSON Representation</span></span>
<span data-ttu-id="9b483-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b483-128">Here is a JSON representation of the resource.</span></span>
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




