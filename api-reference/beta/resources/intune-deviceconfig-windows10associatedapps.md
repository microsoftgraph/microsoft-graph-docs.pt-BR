---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 44b754ba08e8fde1366fda67640582d8552bc4f3
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787204"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="0e528-103">tipo de recurso windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="0e528-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="0e528-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0e528-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e528-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0e528-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e528-106">Definição de aplicativo associado ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0e528-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="0e528-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0e528-107">Properties</span></span>
|<span data-ttu-id="0e528-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0e528-108">Property</span></span>|<span data-ttu-id="0e528-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="0e528-109">Type</span></span>|<span data-ttu-id="0e528-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="0e528-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e528-111">appType</span><span class="sxs-lookup"><span data-stu-id="0e528-111">appType</span></span>|[<span data-ttu-id="0e528-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="0e528-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="0e528-113">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="0e528-113">Application type.</span></span> <span data-ttu-id="0e528-114">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="0e528-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="0e528-115">identificador</span><span class="sxs-lookup"><span data-stu-id="0e528-115">identifier</span></span>|<span data-ttu-id="0e528-116">String</span><span class="sxs-lookup"><span data-stu-id="0e528-116">String</span></span>|<span data-ttu-id="0e528-117">Identificação.</span><span class="sxs-lookup"><span data-stu-id="0e528-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0e528-118">Relações</span><span class="sxs-lookup"><span data-stu-id="0e528-118">Relationships</span></span>
<span data-ttu-id="0e528-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0e528-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e528-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0e528-120">JSON Representation</span></span>
<span data-ttu-id="0e528-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0e528-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10AssociatedApps"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10AssociatedApps",
  "appType": "String",
  "identifier": "String"
}
```



