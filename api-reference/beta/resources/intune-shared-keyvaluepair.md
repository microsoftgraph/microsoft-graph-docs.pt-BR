---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: cd97b7cf0729ae9e1cad1c8440ec9727cc321a67
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42769126"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="f867e-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="f867e-103">keyValuePair resource type</span></span>

> <span data-ttu-id="f867e-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="f867e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f867e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="f867e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f867e-106">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="f867e-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="f867e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f867e-107">Properties</span></span>
|<span data-ttu-id="f867e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f867e-108">Property</span></span>|<span data-ttu-id="f867e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="f867e-109">Type</span></span>|<span data-ttu-id="f867e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="f867e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f867e-111">nome</span><span class="sxs-lookup"><span data-stu-id="f867e-111">name</span></span>|<span data-ttu-id="f867e-112">String</span><span class="sxs-lookup"><span data-stu-id="f867e-112">String</span></span>|<span data-ttu-id="f867e-113">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="f867e-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="f867e-114">value</span><span class="sxs-lookup"><span data-stu-id="f867e-114">value</span></span>|<span data-ttu-id="f867e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f867e-115">String</span></span>|<span data-ttu-id="f867e-116">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="f867e-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="f867e-117">Relações</span><span class="sxs-lookup"><span data-stu-id="f867e-117">Relationships</span></span>
<span data-ttu-id="f867e-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f867e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f867e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f867e-119">JSON Representation</span></span>
<span data-ttu-id="f867e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f867e-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValuePair",
  "name": "String",
  "value": "String"
}
```



