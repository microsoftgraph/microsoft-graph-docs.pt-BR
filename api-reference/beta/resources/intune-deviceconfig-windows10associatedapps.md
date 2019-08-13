---
title: tipo de recurso windows10AssociatedApps
description: Definição de aplicativo associado ao Windows 10.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 438448d90dcbe5fa1922dfd3b51c28d3d5f80ecf
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337892"
---
# <a name="windows10associatedapps-resource-type"></a><span data-ttu-id="08cfb-103">tipo de recurso windows10AssociatedApps</span><span class="sxs-lookup"><span data-stu-id="08cfb-103">windows10AssociatedApps resource type</span></span>

> <span data-ttu-id="08cfb-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="08cfb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08cfb-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="08cfb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08cfb-106">Definição de aplicativo associado ao Windows 10.</span><span class="sxs-lookup"><span data-stu-id="08cfb-106">Windows 10 Associated Application definition.</span></span>

## <a name="properties"></a><span data-ttu-id="08cfb-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="08cfb-107">Properties</span></span>
|<span data-ttu-id="08cfb-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="08cfb-108">Property</span></span>|<span data-ttu-id="08cfb-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="08cfb-109">Type</span></span>|<span data-ttu-id="08cfb-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="08cfb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08cfb-111">appType</span><span class="sxs-lookup"><span data-stu-id="08cfb-111">appType</span></span>|[<span data-ttu-id="08cfb-112">windows10AppType</span><span class="sxs-lookup"><span data-stu-id="08cfb-112">windows10AppType</span></span>](../resources/intune-deviceconfig-windows10apptype.md)|<span data-ttu-id="08cfb-113">Tipo de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="08cfb-113">Application type.</span></span> <span data-ttu-id="08cfb-114">Os valores possíveis são: `desktop` e `universal`.</span><span class="sxs-lookup"><span data-stu-id="08cfb-114">Possible values are: `desktop`, `universal`.</span></span>|
|<span data-ttu-id="08cfb-115">identificador</span><span class="sxs-lookup"><span data-stu-id="08cfb-115">identifier</span></span>|<span data-ttu-id="08cfb-116">String</span><span class="sxs-lookup"><span data-stu-id="08cfb-116">String</span></span>|<span data-ttu-id="08cfb-117">Identificação.</span><span class="sxs-lookup"><span data-stu-id="08cfb-117">Identifier.</span></span>|

## <a name="relationships"></a><span data-ttu-id="08cfb-118">Relações</span><span class="sxs-lookup"><span data-stu-id="08cfb-118">Relationships</span></span>
<span data-ttu-id="08cfb-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="08cfb-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="08cfb-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="08cfb-120">JSON Representation</span></span>
<span data-ttu-id="08cfb-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="08cfb-121">Here is a JSON representation of the resource.</span></span>
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



