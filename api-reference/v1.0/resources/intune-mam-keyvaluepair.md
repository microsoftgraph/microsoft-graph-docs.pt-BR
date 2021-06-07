---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3deb1d366396bf97133b4984bda2b67609fcdee6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751661"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="9357e-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="9357e-103">keyValuePair resource type</span></span>

<span data-ttu-id="9357e-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9357e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9357e-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9357e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9357e-106">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="9357e-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="9357e-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9357e-107">Properties</span></span>
|<span data-ttu-id="9357e-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9357e-108">Property</span></span>|<span data-ttu-id="9357e-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="9357e-109">Type</span></span>|<span data-ttu-id="9357e-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="9357e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9357e-111">nome</span><span class="sxs-lookup"><span data-stu-id="9357e-111">name</span></span>|<span data-ttu-id="9357e-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9357e-112">String</span></span>|<span data-ttu-id="9357e-113">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="9357e-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="9357e-114">value</span><span class="sxs-lookup"><span data-stu-id="9357e-114">value</span></span>|<span data-ttu-id="9357e-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9357e-115">String</span></span>|<span data-ttu-id="9357e-116">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="9357e-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="9357e-117">Relações</span><span class="sxs-lookup"><span data-stu-id="9357e-117">Relationships</span></span>
<span data-ttu-id="9357e-118">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="9357e-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9357e-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9357e-119">JSON Representation</span></span>
<span data-ttu-id="9357e-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9357e-120">Here is a JSON representation of the resource.</span></span>
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




