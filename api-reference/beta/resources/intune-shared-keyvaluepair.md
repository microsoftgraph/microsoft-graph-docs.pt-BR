---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4b86c1cbfcee4519d93bdfa704bc5d283343342c
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49255823"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="1fe7c-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="1fe7c-103">keyValuePair resource type</span></span>

<span data-ttu-id="1fe7c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1fe7c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1fe7c-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1fe7c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1fe7c-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1fe7c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1fe7c-107">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="1fe7c-107">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="1fe7c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1fe7c-108">Properties</span></span>
|<span data-ttu-id="1fe7c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1fe7c-109">Property</span></span>|<span data-ttu-id="1fe7c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1fe7c-110">Type</span></span>|<span data-ttu-id="1fe7c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1fe7c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1fe7c-112">nome</span><span class="sxs-lookup"><span data-stu-id="1fe7c-112">name</span></span>|<span data-ttu-id="1fe7c-113">String</span><span class="sxs-lookup"><span data-stu-id="1fe7c-113">String</span></span>|<span data-ttu-id="1fe7c-114">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="1fe7c-114">Name for this key-value pair</span></span>|
|<span data-ttu-id="1fe7c-115">value</span><span class="sxs-lookup"><span data-stu-id="1fe7c-115">value</span></span>|<span data-ttu-id="1fe7c-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1fe7c-116">String</span></span>|<span data-ttu-id="1fe7c-117">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="1fe7c-117">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fe7c-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1fe7c-118">Relationships</span></span>
<span data-ttu-id="1fe7c-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1fe7c-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1fe7c-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1fe7c-120">JSON Representation</span></span>
<span data-ttu-id="1fe7c-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1fe7c-121">Here is a JSON representation of the resource.</span></span>
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




