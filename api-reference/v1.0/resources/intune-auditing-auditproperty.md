---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e91f3771be981f6ff410e8774f6a8ac9fbc121dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870914"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="55c7b-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="55c7b-103">auditProperty resource type</span></span>

> <span data-ttu-id="55c7b-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="55c7b-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="55c7b-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="55c7b-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="55c7b-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="55c7b-106">Properties</span></span>
|<span data-ttu-id="55c7b-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="55c7b-107">Property</span></span>|<span data-ttu-id="55c7b-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="55c7b-108">Type</span></span>|<span data-ttu-id="55c7b-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="55c7b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55c7b-110">displayName</span><span class="sxs-lookup"><span data-stu-id="55c7b-110">displayName</span></span>|<span data-ttu-id="55c7b-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55c7b-111">String</span></span>|<span data-ttu-id="55c7b-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="55c7b-112">Display name.</span></span>|
|<span data-ttu-id="55c7b-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="55c7b-113">oldValue</span></span>|<span data-ttu-id="55c7b-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55c7b-114">String</span></span>|<span data-ttu-id="55c7b-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="55c7b-115">Old value.</span></span>|
|<span data-ttu-id="55c7b-116">newValue</span><span class="sxs-lookup"><span data-stu-id="55c7b-116">newValue</span></span>|<span data-ttu-id="55c7b-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="55c7b-117">String</span></span>|<span data-ttu-id="55c7b-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="55c7b-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55c7b-119">Relações</span><span class="sxs-lookup"><span data-stu-id="55c7b-119">Relationships</span></span>
<span data-ttu-id="55c7b-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="55c7b-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="55c7b-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="55c7b-121">JSON Representation</span></span>
<span data-ttu-id="55c7b-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="55c7b-122">Here is a JSON representation of the resource.</span></span>
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



