---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e179c1c7318934c538cef06c3284308c54199059
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706062"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="67655-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="67655-103">auditProperty resource type</span></span>

<span data-ttu-id="67655-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67655-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="67655-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67655-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67655-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67655-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67655-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="67655-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="67655-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67655-108">Properties</span></span>
|<span data-ttu-id="67655-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67655-109">Property</span></span>|<span data-ttu-id="67655-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="67655-110">Type</span></span>|<span data-ttu-id="67655-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67655-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67655-112">displayName</span><span class="sxs-lookup"><span data-stu-id="67655-112">displayName</span></span>|<span data-ttu-id="67655-113">String</span><span class="sxs-lookup"><span data-stu-id="67655-113">String</span></span>|<span data-ttu-id="67655-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="67655-114">Display name.</span></span>|
|<span data-ttu-id="67655-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="67655-115">oldValue</span></span>|<span data-ttu-id="67655-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67655-116">String</span></span>|<span data-ttu-id="67655-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="67655-117">Old value.</span></span>|
|<span data-ttu-id="67655-118">newValue</span><span class="sxs-lookup"><span data-stu-id="67655-118">newValue</span></span>|<span data-ttu-id="67655-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67655-119">String</span></span>|<span data-ttu-id="67655-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="67655-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="67655-121">Relações</span><span class="sxs-lookup"><span data-stu-id="67655-121">Relationships</span></span>
<span data-ttu-id="67655-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67655-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67655-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67655-123">JSON Representation</span></span>
<span data-ttu-id="67655-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67655-124">Here is a JSON representation of the resource.</span></span>
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





