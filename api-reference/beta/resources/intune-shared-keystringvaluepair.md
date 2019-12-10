---
title: tipo de recurso keyStringValuePair
description: Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7c62ec2cf1fbe5a78534bdb5f6ff9b1e73e37c9f
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/10/2019
ms.locfileid: "39924518"
---
# <a name="keystringvaluepair-resource-type"></a><span data-ttu-id="bc6ff-103">tipo de recurso keyStringValuePair</span><span class="sxs-lookup"><span data-stu-id="bc6ff-103">keyStringValuePair resource type</span></span>

> <span data-ttu-id="bc6ff-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="bc6ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bc6ff-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="bc6ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bc6ff-106">Um par chave-valor com uma chave de cadeia de caracteres e um valor de cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="bc6ff-106">A key-value pair with a string key and a string value.</span></span>


<span data-ttu-id="bc6ff-107">Herda de [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ff-107">Inherits from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bc6ff-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bc6ff-108">Properties</span></span>
|<span data-ttu-id="bc6ff-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bc6ff-109">Property</span></span>|<span data-ttu-id="bc6ff-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="bc6ff-110">Type</span></span>|<span data-ttu-id="bc6ff-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="bc6ff-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc6ff-112">key</span><span class="sxs-lookup"><span data-stu-id="bc6ff-112">key</span></span>|<span data-ttu-id="bc6ff-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="bc6ff-113">String</span></span>|<span data-ttu-id="bc6ff-114">A chave de cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="bc6ff-114">The string key of the key-value pair.</span></span> <span data-ttu-id="bc6ff-115">Herdado de [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span><span class="sxs-lookup"><span data-stu-id="bc6ff-115">Inherited from [keyTypedValuePair](../resources/intune-shared-keytypedvaluepair.md)</span></span>|
|<span data-ttu-id="bc6ff-116">value</span><span class="sxs-lookup"><span data-stu-id="bc6ff-116">value</span></span>|<span data-ttu-id="bc6ff-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="bc6ff-117">String</span></span>|<span data-ttu-id="bc6ff-118">O valor da cadeia de caracteres do par chave-valor.</span><span class="sxs-lookup"><span data-stu-id="bc6ff-118">The string value of the key-value pair.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bc6ff-119">Relações</span><span class="sxs-lookup"><span data-stu-id="bc6ff-119">Relationships</span></span>
<span data-ttu-id="bc6ff-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="bc6ff-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bc6ff-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bc6ff-121">JSON Representation</span></span>
<span data-ttu-id="bc6ff-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bc6ff-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyStringValuePair"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyStringValuePair",
  "key": "String",
  "value": "String"
}
```



