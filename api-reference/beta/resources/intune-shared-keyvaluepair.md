---
title: Tipo de recurso keyValuePair
description: Par chave-valor para armazenar configurações personalizadas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a8feecabeca3cfc916c0bd3ce1b87cab3a68809
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32525240"
---
# <a name="keyvaluepair-resource-type"></a><span data-ttu-id="47132-103">Tipo de recurso keyValuePair</span><span class="sxs-lookup"><span data-stu-id="47132-103">keyValuePair resource type</span></span>

> <span data-ttu-id="47132-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="47132-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47132-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="47132-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47132-106">Par chave-valor para armazenar configurações personalizadas</span><span class="sxs-lookup"><span data-stu-id="47132-106">Key value pair for storing custom settings</span></span>

## <a name="properties"></a><span data-ttu-id="47132-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="47132-107">Properties</span></span>
|<span data-ttu-id="47132-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="47132-108">Property</span></span>|<span data-ttu-id="47132-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="47132-109">Type</span></span>|<span data-ttu-id="47132-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="47132-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47132-111">name</span><span class="sxs-lookup"><span data-stu-id="47132-111">name</span></span>|<span data-ttu-id="47132-112">String</span><span class="sxs-lookup"><span data-stu-id="47132-112">String</span></span>|<span data-ttu-id="47132-113">Nome deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="47132-113">Name for this key-value pair</span></span>|
|<span data-ttu-id="47132-114">value</span><span class="sxs-lookup"><span data-stu-id="47132-114">value</span></span>|<span data-ttu-id="47132-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="47132-115">String</span></span>|<span data-ttu-id="47132-116">Valor deste par chave-valor</span><span class="sxs-lookup"><span data-stu-id="47132-116">Value for this key-value pair</span></span>|

## <a name="relationships"></a><span data-ttu-id="47132-117">Relações</span><span class="sxs-lookup"><span data-stu-id="47132-117">Relationships</span></span>
<span data-ttu-id="47132-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="47132-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="47132-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="47132-119">JSON Representation</span></span>
<span data-ttu-id="47132-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="47132-120">Here is a JSON representation of the resource.</span></span>
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




