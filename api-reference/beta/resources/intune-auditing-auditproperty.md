---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: dd5a43f1837ed3acf8927af5bac4e46d864f3fec
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43472113"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="9b9ea-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="9b9ea-103">auditProperty resource type</span></span>

<span data-ttu-id="9b9ea-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b9ea-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9b9ea-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9b9ea-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9b9ea-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="9b9ea-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9b9ea-108">Properties</span></span>
|<span data-ttu-id="9b9ea-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9b9ea-109">Property</span></span>|<span data-ttu-id="9b9ea-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9b9ea-110">Type</span></span>|<span data-ttu-id="9b9ea-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9b9ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9b9ea-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9b9ea-112">displayName</span></span>|<span data-ttu-id="9b9ea-113">String</span><span class="sxs-lookup"><span data-stu-id="9b9ea-113">String</span></span>|<span data-ttu-id="9b9ea-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-114">Display name.</span></span>|
|<span data-ttu-id="9b9ea-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="9b9ea-115">oldValue</span></span>|<span data-ttu-id="9b9ea-116">String</span><span class="sxs-lookup"><span data-stu-id="9b9ea-116">String</span></span>|<span data-ttu-id="9b9ea-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-117">Old value.</span></span>|
|<span data-ttu-id="9b9ea-118">newValue</span><span class="sxs-lookup"><span data-stu-id="9b9ea-118">newValue</span></span>|<span data-ttu-id="9b9ea-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9b9ea-119">String</span></span>|<span data-ttu-id="9b9ea-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b9ea-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9b9ea-121">Relationships</span></span>
<span data-ttu-id="9b9ea-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9b9ea-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9b9ea-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9b9ea-123">JSON Representation</span></span>
<span data-ttu-id="9b9ea-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9b9ea-124">Here is a JSON representation of the resource.</span></span>
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



