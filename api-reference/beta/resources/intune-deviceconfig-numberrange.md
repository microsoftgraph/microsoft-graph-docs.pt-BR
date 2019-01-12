---
title: tipo de recurso de numberRange
description: Definição do intervalo de número.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9dc10caaa125144944cf3e6c52c65e58f9d57975
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977402"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="735f6-103">tipo de recurso de numberRange</span><span class="sxs-lookup"><span data-stu-id="735f6-103">numberRange resource type</span></span>

> <span data-ttu-id="735f6-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="735f6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="735f6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="735f6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="735f6-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="735f6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="735f6-107">Definição do intervalo de número.</span><span class="sxs-lookup"><span data-stu-id="735f6-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="735f6-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="735f6-108">Properties</span></span>
|<span data-ttu-id="735f6-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="735f6-109">Property</span></span>|<span data-ttu-id="735f6-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="735f6-110">Type</span></span>|<span data-ttu-id="735f6-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="735f6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="735f6-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="735f6-112">lowerNumber</span></span>|<span data-ttu-id="735f6-113">Int32</span><span class="sxs-lookup"><span data-stu-id="735f6-113">Int32</span></span>|<span data-ttu-id="735f6-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="735f6-114">Lower number.</span></span>|
|<span data-ttu-id="735f6-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="735f6-115">upperNumber</span></span>|<span data-ttu-id="735f6-116">Int32</span><span class="sxs-lookup"><span data-stu-id="735f6-116">Int32</span></span>|<span data-ttu-id="735f6-117">Número de superior.</span><span class="sxs-lookup"><span data-stu-id="735f6-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="735f6-118">Relações</span><span class="sxs-lookup"><span data-stu-id="735f6-118">Relationships</span></span>
<span data-ttu-id="735f6-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="735f6-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="735f6-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="735f6-120">JSON Representation</span></span>
<span data-ttu-id="735f6-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="735f6-121">Here is a JSON representation of the resource.</span></span>
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





