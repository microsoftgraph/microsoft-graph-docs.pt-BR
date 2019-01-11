---
title: tipo de recurso de mobileContainedApp
description: Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b81ee4ca194d1d01e3d834b3287f6b400e712a27
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27826282"
---
# <a name="mobilecontainedapp-resource-type"></a><span data-ttu-id="320ce-103">tipo de recurso de mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="320ce-103">mobileContainedApp resource type</span></span>

> <span data-ttu-id="320ce-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="320ce-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="320ce-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="320ce-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="320ce-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="320ce-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="320ce-107">Uma classe abstrata que representa um aplicativo contido em um mobileApp atuando como um pacote.</span><span class="sxs-lookup"><span data-stu-id="320ce-107">An abstract class that represents a contained app in a mobileApp acting as a package.</span></span>
## <a name="methods"></a><span data-ttu-id="320ce-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="320ce-108">Methods</span></span>
|<span data-ttu-id="320ce-109">Método</span><span class="sxs-lookup"><span data-stu-id="320ce-109">Method</span></span>|<span data-ttu-id="320ce-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="320ce-110">Return Type</span></span>|<span data-ttu-id="320ce-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="320ce-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="320ce-112">Lista mobileContainedApps</span><span class="sxs-lookup"><span data-stu-id="320ce-112">List mobileContainedApps</span></span>](../api/intune-apps-mobilecontainedapp-list.md)|<span data-ttu-id="320ce-113">coleção [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="320ce-113">[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) collection</span></span>|<span data-ttu-id="320ce-114">Lista as propriedades e os relacionamentos dos objetos [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="320ce-114">List properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) objects.</span></span>|
|[<span data-ttu-id="320ce-115">Obter mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="320ce-115">Get mobileContainedApp</span></span>](../api/intune-apps-mobilecontainedapp-get.md)|[<span data-ttu-id="320ce-116">mobileContainedApp</span><span class="sxs-lookup"><span data-stu-id="320ce-116">mobileContainedApp</span></span>](../resources/intune-apps-mobilecontainedapp.md)|<span data-ttu-id="320ce-117">Leia as propriedades e os relacionamentos do objeto [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) .</span><span class="sxs-lookup"><span data-stu-id="320ce-117">Read properties and relationships of the [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="320ce-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="320ce-118">Properties</span></span>
|<span data-ttu-id="320ce-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="320ce-119">Property</span></span>|<span data-ttu-id="320ce-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="320ce-120">Type</span></span>|<span data-ttu-id="320ce-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="320ce-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="320ce-122">id</span><span class="sxs-lookup"><span data-stu-id="320ce-122">id</span></span>|<span data-ttu-id="320ce-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="320ce-123">String</span></span>|<span data-ttu-id="320ce-124">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="320ce-124">Key of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="320ce-125">Relações</span><span class="sxs-lookup"><span data-stu-id="320ce-125">Relationships</span></span>
<span data-ttu-id="320ce-126">Nenhum</span><span class="sxs-lookup"><span data-stu-id="320ce-126">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="320ce-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="320ce-127">JSON Representation</span></span>
<span data-ttu-id="320ce-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="320ce-128">Here is a JSON representation of the resource.</span></span>
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





