---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
ms.openlocfilehash: 2d7cd7f1fbbf9f813cf447ca53e0d4652eb0feda
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27312898"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="290af-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="290af-103">auditProperty resource type</span></span>

> <span data-ttu-id="290af-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="290af-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="290af-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="290af-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="290af-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="290af-106">Properties</span></span>
|<span data-ttu-id="290af-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="290af-107">Property</span></span>|<span data-ttu-id="290af-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="290af-108">Type</span></span>|<span data-ttu-id="290af-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="290af-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="290af-110">displayName</span><span class="sxs-lookup"><span data-stu-id="290af-110">displayName</span></span>|<span data-ttu-id="290af-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="290af-111">String</span></span>|<span data-ttu-id="290af-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="290af-112">Display name.</span></span>|
|<span data-ttu-id="290af-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="290af-113">oldValue</span></span>|<span data-ttu-id="290af-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="290af-114">String</span></span>|<span data-ttu-id="290af-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="290af-115">Old value.</span></span>|
|<span data-ttu-id="290af-116">newValue</span><span class="sxs-lookup"><span data-stu-id="290af-116">newValue</span></span>|<span data-ttu-id="290af-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="290af-117">String</span></span>|<span data-ttu-id="290af-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="290af-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="290af-119">Relações</span><span class="sxs-lookup"><span data-stu-id="290af-119">Relationships</span></span>
<span data-ttu-id="290af-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="290af-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="290af-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="290af-121">JSON Representation</span></span>
<span data-ttu-id="290af-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="290af-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.auditProperty"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditProperty",
  "displayName": "String",
  "oldValue": "String",
  "newValue": "String"
}
```



