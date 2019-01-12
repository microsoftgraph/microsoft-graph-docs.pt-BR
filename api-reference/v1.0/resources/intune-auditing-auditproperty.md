---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 290aae8c245fd09c17fc766cedd7c2e253626943
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912026"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="9247f-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="9247f-103">auditProperty resource type</span></span>

> <span data-ttu-id="9247f-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="9247f-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9247f-105">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9247f-105">A class containing the properties for Audit Property.</span></span>
## <a name="properties"></a><span data-ttu-id="9247f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9247f-106">Properties</span></span>
|<span data-ttu-id="9247f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9247f-107">Property</span></span>|<span data-ttu-id="9247f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="9247f-108">Type</span></span>|<span data-ttu-id="9247f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="9247f-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9247f-110">displayName</span><span class="sxs-lookup"><span data-stu-id="9247f-110">displayName</span></span>|<span data-ttu-id="9247f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9247f-111">String</span></span>|<span data-ttu-id="9247f-112">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9247f-112">Display name.</span></span>|
|<span data-ttu-id="9247f-113">oldValue</span><span class="sxs-lookup"><span data-stu-id="9247f-113">oldValue</span></span>|<span data-ttu-id="9247f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9247f-114">String</span></span>|<span data-ttu-id="9247f-115">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="9247f-115">Old value.</span></span>|
|<span data-ttu-id="9247f-116">newValue</span><span class="sxs-lookup"><span data-stu-id="9247f-116">newValue</span></span>|<span data-ttu-id="9247f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9247f-117">String</span></span>|<span data-ttu-id="9247f-118">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="9247f-118">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9247f-119">Relações</span><span class="sxs-lookup"><span data-stu-id="9247f-119">Relationships</span></span>
<span data-ttu-id="9247f-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9247f-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9247f-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9247f-121">JSON Representation</span></span>
<span data-ttu-id="9247f-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9247f-122">Here is a JSON representation of the resource.</span></span>
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



