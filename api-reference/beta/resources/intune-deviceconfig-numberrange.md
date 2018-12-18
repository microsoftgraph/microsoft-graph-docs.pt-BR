---
title: tipo de recurso de numberRange
description: Definição do intervalo de número.
author: tfitzmac
ms.openlocfilehash: 7b9703524e1562a7367a3c5b9bf0212e29620429
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314655"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="a660a-103">tipo de recurso de numberRange</span><span class="sxs-lookup"><span data-stu-id="a660a-103">numberRange resource type</span></span>

> <span data-ttu-id="a660a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a660a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a660a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a660a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a660a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a660a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a660a-107">Definição do intervalo de número.</span><span class="sxs-lookup"><span data-stu-id="a660a-107">Number Range definition.</span></span>
## <a name="properties"></a><span data-ttu-id="a660a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a660a-108">Properties</span></span>
|<span data-ttu-id="a660a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a660a-109">Property</span></span>|<span data-ttu-id="a660a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a660a-110">Type</span></span>|<span data-ttu-id="a660a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a660a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a660a-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="a660a-112">lowerNumber</span></span>|<span data-ttu-id="a660a-113">Int32</span><span class="sxs-lookup"><span data-stu-id="a660a-113">Int32</span></span>|<span data-ttu-id="a660a-114">Número menor.</span><span class="sxs-lookup"><span data-stu-id="a660a-114">Lower number.</span></span>|
|<span data-ttu-id="a660a-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="a660a-115">upperNumber</span></span>|<span data-ttu-id="a660a-116">Int32</span><span class="sxs-lookup"><span data-stu-id="a660a-116">Int32</span></span>|<span data-ttu-id="a660a-117">Número de superior.</span><span class="sxs-lookup"><span data-stu-id="a660a-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a660a-118">Relações</span><span class="sxs-lookup"><span data-stu-id="a660a-118">Relationships</span></span>
<span data-ttu-id="a660a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a660a-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a660a-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a660a-120">JSON Representation</span></span>
<span data-ttu-id="a660a-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a660a-121">Here is a JSON representation of the resource.</span></span>
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





