---
title: Tipo de recurso resourceAction
description: Ainda não documentado
author: tfitzmac
ms.openlocfilehash: b64c1fb0ef49c2d7c47c88137bcca8ef89f6ad67
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343915"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="d493b-103">Tipo de recurso resourceAction</span><span class="sxs-lookup"><span data-stu-id="d493b-103">resourceAction resource type</span></span>

> <span data-ttu-id="d493b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="d493b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d493b-105">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="d493b-105">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="d493b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d493b-106">Properties</span></span>
|<span data-ttu-id="d493b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d493b-107">Property</span></span>|<span data-ttu-id="d493b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="d493b-108">Type</span></span>|<span data-ttu-id="d493b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="d493b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d493b-110">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d493b-110">allowedResourceActions</span></span>|<span data-ttu-id="d493b-111">String collection</span><span class="sxs-lookup"><span data-stu-id="d493b-111">String collection</span></span>|<span data-ttu-id="d493b-112">Ações permitidas</span><span class="sxs-lookup"><span data-stu-id="d493b-112">Allowed Actions</span></span>|
|<span data-ttu-id="d493b-113">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="d493b-113">notAllowedResourceActions</span></span>|<span data-ttu-id="d493b-114">String collection</span><span class="sxs-lookup"><span data-stu-id="d493b-114">String collection</span></span>|<span data-ttu-id="d493b-115">Ações não permitidas</span><span class="sxs-lookup"><span data-stu-id="d493b-115">Not Allowed Actions</span></span>|

## <a name="relationships"></a><span data-ttu-id="d493b-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d493b-116">Relationships</span></span>
<span data-ttu-id="d493b-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d493b-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d493b-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d493b-118">JSON Representation</span></span>
<span data-ttu-id="d493b-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d493b-119">Here is a JSON representation of the resource.</span></span>
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



