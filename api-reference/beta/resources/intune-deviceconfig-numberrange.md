---
title: tipo de recurso de numberRange
description: Definição do intervalo de número.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27393bdac6519078c2021e3484ae58ddf43216d9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416857"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="23558-103">tipo de recurso de numberRange</span><span class="sxs-lookup"><span data-stu-id="23558-103">numberRange resource type</span></span>

> <span data-ttu-id="23558-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="23558-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="23558-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="23558-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23558-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="23558-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23558-107">Definição do intervalo de número.</span><span class="sxs-lookup"><span data-stu-id="23558-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="23558-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="23558-108">Properties</span></span>
|<span data-ttu-id="23558-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="23558-109">Property</span></span>|<span data-ttu-id="23558-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="23558-110">Type</span></span>|<span data-ttu-id="23558-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="23558-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23558-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="23558-112">lowerNumber</span></span>|<span data-ttu-id="23558-113">Int32</span><span class="sxs-lookup"><span data-stu-id="23558-113">Int32</span></span>|<span data-ttu-id="23558-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="23558-114">Lower number.</span></span>|
|<span data-ttu-id="23558-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="23558-115">upperNumber</span></span>|<span data-ttu-id="23558-116">Int32</span><span class="sxs-lookup"><span data-stu-id="23558-116">Int32</span></span>|<span data-ttu-id="23558-117">Número de superior.</span><span class="sxs-lookup"><span data-stu-id="23558-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23558-118">Relações</span><span class="sxs-lookup"><span data-stu-id="23558-118">Relationships</span></span>
<span data-ttu-id="23558-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="23558-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="23558-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="23558-120">JSON Representation</span></span>
<span data-ttu-id="23558-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="23558-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




