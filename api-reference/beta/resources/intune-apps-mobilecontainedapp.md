---
title: tipo de recurso de mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5a9b36193aeda51679018bc534974c3678326a19
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963812"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="0a501-103">tipo de recurso de mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="0a501-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="0a501-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="0a501-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0a501-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="0a501-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a501-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="0a501-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0a501-107">Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.</span><span class="sxs-lookup"><span data-stu-id="0a501-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>
## <a name="methods"></a><span data-ttu-id="0a501-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="0a501-108">Methods</span></span>
|<span data-ttu-id="0a501-109">Método</span><span class="sxs-lookup"><span data-stu-id="0a501-109">Method</span></span>|<span data-ttu-id="0a501-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="0a501-110">Return Type</span></span>|<span data-ttu-id="0a501-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a501-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0a501-112">Lista mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="0a501-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="0a501-113">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0a501-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="0a501-114">Lista as propriedades e os relacionamentos dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0a501-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="0a501-115">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="0a501-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="0a501-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="0a501-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="0a501-117">Leia as propriedades e os relacionamentos do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="0a501-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0a501-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0a501-118">Properties</span></span>
|<span data-ttu-id="0a501-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0a501-119">Property</span></span>|<span data-ttu-id="0a501-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="0a501-120">Type</span></span>|<span data-ttu-id="0a501-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="0a501-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0a501-122">id</span><span class="sxs-lookup"><span data-stu-id="0a501-122">id</span></span>|<span data-ttu-id="0a501-123">String</span><span class="sxs-lookup"><span data-stu-id="0a501-123">String</span></span>|<span data-ttu-id="0a501-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="0a501-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0a501-125">Relações</span><span class="sxs-lookup"><span data-stu-id="0a501-125">Relationships</span></span>
<span data-ttu-id="0a501-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0a501-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0a501-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0a501-127">JSON Representation</span></span>
<span data-ttu-id="0a501-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0a501-128">Here is a JSON representation of the resource.</span></span>
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





