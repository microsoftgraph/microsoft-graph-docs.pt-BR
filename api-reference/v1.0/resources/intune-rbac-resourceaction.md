---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 94a0ce30dc6e9607aa1531e7421af6b7a5500939
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870726"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="651d1-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="651d1-103">resourceAction resource type</span></span>

> <span data-ttu-id="651d1-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="651d1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="651d1-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="651d1-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="651d1-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="651d1-106">Properties</span></span>
|<span data-ttu-id="651d1-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="651d1-107">Property</span></span>|<span data-ttu-id="651d1-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="651d1-108">Type</span></span>|<span data-ttu-id="651d1-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="651d1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="651d1-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="651d1-110">allowedResourceActions</span></span>|<span data-ttu-id="651d1-111">String collection</span><span class="sxs-lookup"><span data-stu-id="651d1-111">String collection</span></span>|<span data-ttu-id="651d1-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="651d1-112">Allowed Actions</span></span>|
|<span data-ttu-id="651d1-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="651d1-113">notAllowedResourceActions</span></span>|<span data-ttu-id="651d1-114">String collection</span><span class="sxs-lookup"><span data-stu-id="651d1-114">String collection</span></span>|<span data-ttu-id="651d1-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="651d1-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="651d1-116">Relações</span><span class="sxs-lookup"><span data-stu-id="651d1-116">Relationships</span></span>
<span data-ttu-id="651d1-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="651d1-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="651d1-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="651d1-118">JSON Representation</span></span>
<span data-ttu-id="651d1-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="651d1-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```



