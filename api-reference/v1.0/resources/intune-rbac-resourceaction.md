---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f1db2a1db2c76829ddd39438ed40cd1086fe4e17
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27932705"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="4cca7-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="4cca7-103">resourceAction resource type</span></span>

> <span data-ttu-id="4cca7-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4cca7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4cca7-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="4cca7-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="4cca7-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4cca7-106">Properties</span></span>
|<span data-ttu-id="4cca7-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4cca7-107">Property</span></span>|<span data-ttu-id="4cca7-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="4cca7-108">Type</span></span>|<span data-ttu-id="4cca7-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="4cca7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4cca7-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="4cca7-110">allowedResourceActions</span></span>|<span data-ttu-id="4cca7-111">String collection</span><span class="sxs-lookup"><span data-stu-id="4cca7-111">String collection</span></span>|<span data-ttu-id="4cca7-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="4cca7-112">Allowed Actions</span></span>|
|<span data-ttu-id="4cca7-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="4cca7-113">notAllowedResourceActions</span></span>|<span data-ttu-id="4cca7-114">String collection</span><span class="sxs-lookup"><span data-stu-id="4cca7-114">String collection</span></span>|<span data-ttu-id="4cca7-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="4cca7-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="4cca7-116">Relações</span><span class="sxs-lookup"><span data-stu-id="4cca7-116">Relationships</span></span>
<span data-ttu-id="4cca7-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4cca7-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4cca7-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4cca7-118">JSON Representation</span></span>
<span data-ttu-id="4cca7-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4cca7-119">Here is a JSON representation of the resource.</span></span>
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



