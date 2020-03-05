---
title: tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 73536b8e1343d2c69296ca7c8149f4fad0e9a34b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42491327"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="964c9-103">tipo de recurso mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="964c9-103">mobileContainedApp resource type</span></span>

<span data-ttu-id="964c9-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="964c9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="964c9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="964c9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="964c9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="964c9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="964c9-107">Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="964c9-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="964c9-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="964c9-108">Methods</span></span>
|<span data-ttu-id="964c9-109">Método</span><span class="sxs-lookup"><span data-stu-id="964c9-109">Method</span></span>|<span data-ttu-id="964c9-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="964c9-110">Return Type</span></span>|<span data-ttu-id="964c9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="964c9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="964c9-112">Listar mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="964c9-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="964c9-113">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="964c9-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="964c9-114">Listar Propriedades e relações dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="964c9-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="964c9-115">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="964c9-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="964c9-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="964c9-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="964c9-117">Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="964c9-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="964c9-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="964c9-118">Properties</span></span>
|<span data-ttu-id="964c9-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="964c9-119">Property</span></span>|<span data-ttu-id="964c9-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="964c9-120">Type</span></span>|<span data-ttu-id="964c9-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="964c9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="964c9-122">id</span><span class="sxs-lookup"><span data-stu-id="964c9-122">id</span></span>|<span data-ttu-id="964c9-123">String</span><span class="sxs-lookup"><span data-stu-id="964c9-123">String</span></span>|<span data-ttu-id="964c9-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="964c9-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="964c9-125">Relações</span><span class="sxs-lookup"><span data-stu-id="964c9-125">Relationships</span></span>
<span data-ttu-id="964c9-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="964c9-126">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="964c9-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="964c9-127">JSON Representation</span></span>
<span data-ttu-id="964c9-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="964c9-128">Here is a JSON representation of the resource.</span></span>
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



