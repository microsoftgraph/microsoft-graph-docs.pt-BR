---
title: Tipo de recurso resourceAction
description: Ainda não documentado
ms.openlocfilehash: 4cbfc149207f2f7589bd7e05075326641d4e8b67
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27003521"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="62468-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="62468-103">resourceAction resource type</span></span>

> <span data-ttu-id="62468-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="62468-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="62468-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="62468-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="62468-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62468-106">Properties</span></span>
|<span data-ttu-id="62468-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62468-107">Property</span></span>|<span data-ttu-id="62468-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="62468-108">Type</span></span>|<span data-ttu-id="62468-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="62468-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62468-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="62468-110">allowedResourceActions</span></span>|<span data-ttu-id="62468-111">String collection</span><span class="sxs-lookup"><span data-stu-id="62468-111">String collection</span></span>|<span data-ttu-id="62468-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="62468-112">Allowed Actions</span></span>|
|<span data-ttu-id="62468-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="62468-113">notAllowedResourceActions</span></span>|<span data-ttu-id="62468-114">String collection</span><span class="sxs-lookup"><span data-stu-id="62468-114">String collection</span></span>|<span data-ttu-id="62468-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="62468-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="62468-116">Relações</span><span class="sxs-lookup"><span data-stu-id="62468-116">Relationships</span></span>
<span data-ttu-id="62468-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62468-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="62468-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62468-118">JSON Representation</span></span>
<span data-ttu-id="62468-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62468-119">Here is a JSON representation of the resource.</span></span>
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



