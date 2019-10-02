---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2849e6adfc0b43b9091764cd2706d5c572826774
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37356433"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="2c8ae-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="2c8ae-103">keyValuePair resource type</span></span>

> <span data-ttu-id="2c8ae-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2c8ae-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2c8ae-105">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="2c8ae-105">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="2c8ae-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2c8ae-106">Properties</span></span>
|<span data-ttu-id="2c8ae-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2c8ae-107">Property</span></span>|<span data-ttu-id="2c8ae-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="2c8ae-108">Type</span></span>|<span data-ttu-id="2c8ae-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="2c8ae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2c8ae-110">name</span><span class="sxs-lookup"><span data-stu-id="2c8ae-110">name</span></span>|<span data-ttu-id="2c8ae-111">String</span><span class="sxs-lookup"><span data-stu-id="2c8ae-111">String</span></span>|<span data-ttu-id="2c8ae-112">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="2c8ae-112">Name for this key-value pair</span></span>|
|<span data-ttu-id="2c8ae-113">value</span><span class="sxs-lookup"><span data-stu-id="2c8ae-113">value</span></span>|<span data-ttu-id="2c8ae-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2c8ae-114">String</span></span>|<span data-ttu-id="2c8ae-115">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="2c8ae-115">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="2c8ae-116">Relações</span><span class="sxs-lookup"><span data-stu-id="2c8ae-116">Relationships</span></span>
<span data-ttu-id="2c8ae-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2c8ae-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2c8ae-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2c8ae-118">JSON Representation</span></span>
<span data-ttu-id="2c8ae-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c8ae-119">Here is a JSON representation of the resource.</span></span>
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




