---
title: tipo de recurso mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05874102e62e86e5b64fb20c892c2e96c66acfc9
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32552845"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="9d825-103">tipo de recurso mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9d825-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="9d825-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9d825-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d825-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9d825-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d825-106">Uma classe abstrata que representa um aplicativo contido em um mobileApp que atua como um pacote.</span><span class="sxs-lookup"><span data-stu-id="9d825-106">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>

## <a name="methods"></a><span data-ttu-id="9d825-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="9d825-107">Methods</span></span>
|<span data-ttu-id="9d825-108">Método</span><span class="sxs-lookup"><span data-stu-id="9d825-108">Method</span></span>|<span data-ttu-id="9d825-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="9d825-109">Return Type</span></span>|<span data-ttu-id="9d825-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d825-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="9d825-111">Listar mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="9d825-111">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="9d825-112">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9d825-112">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="9d825-113">Listar Propriedades e relações dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9d825-113">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="9d825-114">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9d825-114">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="9d825-115">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="9d825-115">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="9d825-116">Leia as propriedades e as relações do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="9d825-116">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="9d825-117">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9d825-117">Properties</span></span>
|<span data-ttu-id="9d825-118">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9d825-118">Property</span></span>|<span data-ttu-id="9d825-119">Tipo</span><span class="sxs-lookup"><span data-stu-id="9d825-119">Type</span></span>|<span data-ttu-id="9d825-120">Descrição</span><span class="sxs-lookup"><span data-stu-id="9d825-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d825-121">id</span><span class="sxs-lookup"><span data-stu-id="9d825-121">id</span></span>|<span data-ttu-id="9d825-122">String</span><span class="sxs-lookup"><span data-stu-id="9d825-122">String</span></span>|<span data-ttu-id="9d825-123">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="9d825-123">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9d825-124">Relações</span><span class="sxs-lookup"><span data-stu-id="9d825-124">Relationships</span></span>
<span data-ttu-id="9d825-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9d825-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9d825-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9d825-126">JSON Representation</span></span>
<span data-ttu-id="9d825-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9d825-127">Here is a JSON representation of the resource.</span></span>
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





