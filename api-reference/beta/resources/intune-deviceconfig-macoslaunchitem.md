---
title: tipo de recurso macOSLaunchItem
description: Representa um aplicativo na lista de itens de lançamento do macOS
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: f8834b43e6d4f09e95701b700c3fa11224347291
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294302"
---
# <a name="macoslaunchitem-resource-type"></a><span data-ttu-id="04be7-103">tipo de recurso macOSLaunchItem</span><span class="sxs-lookup"><span data-stu-id="04be7-103">macOSLaunchItem resource type</span></span>

<span data-ttu-id="04be7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="04be7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="04be7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="04be7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="04be7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="04be7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04be7-107">Representa um aplicativo na lista de itens de lançamento do macOS</span><span class="sxs-lookup"><span data-stu-id="04be7-107">Represents an app in the list of macOS launch items</span></span>

## <a name="properties"></a><span data-ttu-id="04be7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="04be7-108">Properties</span></span>
|<span data-ttu-id="04be7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="04be7-109">Property</span></span>|<span data-ttu-id="04be7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="04be7-110">Type</span></span>|<span data-ttu-id="04be7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="04be7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04be7-112">caminho</span><span class="sxs-lookup"><span data-stu-id="04be7-112">path</span></span>|<span data-ttu-id="04be7-113">String</span><span class="sxs-lookup"><span data-stu-id="04be7-113">String</span></span>|<span data-ttu-id="04be7-114">Caminho para o item de lançamento.</span><span class="sxs-lookup"><span data-stu-id="04be7-114">Path to the launch item.</span></span>|
|<span data-ttu-id="04be7-115">ocult</span><span class="sxs-lookup"><span data-stu-id="04be7-115">hide</span></span>|<span data-ttu-id="04be7-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="04be7-116">Boolean</span></span>|<span data-ttu-id="04be7-117">Se o item será ou não ocultado da lista usuários e grupos.</span><span class="sxs-lookup"><span data-stu-id="04be7-117">Whether or not to hide the item from the Users and Groups List.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04be7-118">Relações</span><span class="sxs-lookup"><span data-stu-id="04be7-118">Relationships</span></span>
<span data-ttu-id="04be7-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="04be7-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="04be7-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="04be7-120">JSON Representation</span></span>
<span data-ttu-id="04be7-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="04be7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLaunchItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLaunchItem",
  "path": "String",
  "hide": true
}
```




