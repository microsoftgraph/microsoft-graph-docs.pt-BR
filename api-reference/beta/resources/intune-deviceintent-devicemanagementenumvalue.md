---
title: tipo de recurso deviceManagementEnumValue
description: Informações de definição para um valor de enumeração
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ade5c3c10354d8697ca40f553c0941751cd26c1a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36366620"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="06811-103">tipo de recurso deviceManagementEnumValue</span><span class="sxs-lookup"><span data-stu-id="06811-103">deviceManagementEnumValue resource type</span></span>

> <span data-ttu-id="06811-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="06811-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06811-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="06811-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06811-106">Informações de definição para um valor de enumeração</span><span class="sxs-lookup"><span data-stu-id="06811-106">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="06811-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="06811-107">Properties</span></span>
|<span data-ttu-id="06811-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="06811-108">Property</span></span>|<span data-ttu-id="06811-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="06811-109">Type</span></span>|<span data-ttu-id="06811-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="06811-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06811-111">valor</span><span class="sxs-lookup"><span data-stu-id="06811-111">value</span></span>|<span data-ttu-id="06811-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="06811-112">String</span></span>|<span data-ttu-id="06811-113">O texto de valor de enumeração bruto</span><span class="sxs-lookup"><span data-stu-id="06811-113">The raw enum value text</span></span>|
|<span data-ttu-id="06811-114">displayName</span><span class="sxs-lookup"><span data-stu-id="06811-114">displayName</span></span>|<span data-ttu-id="06811-115">String</span><span class="sxs-lookup"><span data-stu-id="06811-115">String</span></span>|<span data-ttu-id="06811-116">Nome para exibição desse valor de enumeração</span><span class="sxs-lookup"><span data-stu-id="06811-116">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="06811-117">Relações</span><span class="sxs-lookup"><span data-stu-id="06811-117">Relationships</span></span>
<span data-ttu-id="06811-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="06811-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06811-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="06811-119">JSON Representation</span></span>
<span data-ttu-id="06811-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="06811-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```



