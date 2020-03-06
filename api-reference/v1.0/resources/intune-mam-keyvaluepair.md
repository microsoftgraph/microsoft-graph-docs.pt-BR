---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c0ced5c90f0e36906a534523836e7be3b99eb797
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533193"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="4c39f-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="4c39f-103">keyValuePair resource type</span></span>

<span data-ttu-id="4c39f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c39f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c39f-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4c39f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c39f-106">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="4c39f-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="4c39f-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c39f-107">Properties</span></span>
|<span data-ttu-id="4c39f-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c39f-108">Property</span></span>|<span data-ttu-id="4c39f-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c39f-109">Type</span></span>|<span data-ttu-id="4c39f-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c39f-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c39f-111">nome</span><span class="sxs-lookup"><span data-stu-id="4c39f-111">name</span></span>|<span data-ttu-id="4c39f-112">String</span><span class="sxs-lookup"><span data-stu-id="4c39f-112">String</span></span>|<span data-ttu-id="4c39f-113">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="4c39f-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="4c39f-114">value</span><span class="sxs-lookup"><span data-stu-id="4c39f-114">value</span></span>|<span data-ttu-id="4c39f-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4c39f-115">String</span></span>|<span data-ttu-id="4c39f-116">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="4c39f-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c39f-117">Relações</span><span class="sxs-lookup"><span data-stu-id="4c39f-117">Relationships</span></span>
<span data-ttu-id="4c39f-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c39f-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="4c39f-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c39f-119">JSON Representation</span></span>
<span data-ttu-id="4c39f-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c39f-120">Here is a JSON representation of the resource.</span></span>
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




