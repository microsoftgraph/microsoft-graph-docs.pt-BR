---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 666879bd6a4554be85c52c54c1d9ef3f1a406886
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295555"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="9a952-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="9a952-103">auditProperty resource type</span></span>

<span data-ttu-id="9a952-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a952-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a952-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9a952-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a952-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9a952-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a952-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="9a952-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="9a952-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="9a952-108">Properties</span></span>
|<span data-ttu-id="9a952-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="9a952-109">Property</span></span>|<span data-ttu-id="9a952-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="9a952-110">Type</span></span>|<span data-ttu-id="9a952-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="9a952-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a952-112">displayName</span><span class="sxs-lookup"><span data-stu-id="9a952-112">displayName</span></span>|<span data-ttu-id="9a952-113">String</span><span class="sxs-lookup"><span data-stu-id="9a952-113">String</span></span>|<span data-ttu-id="9a952-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="9a952-114">Display name.</span></span>|
|<span data-ttu-id="9a952-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="9a952-115">oldValue</span></span>|<span data-ttu-id="9a952-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a952-116">String</span></span>|<span data-ttu-id="9a952-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="9a952-117">Old value.</span></span>|
|<span data-ttu-id="9a952-118">newValue</span><span class="sxs-lookup"><span data-stu-id="9a952-118">newValue</span></span>|<span data-ttu-id="9a952-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="9a952-119">String</span></span>|<span data-ttu-id="9a952-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="9a952-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9a952-121">Relações</span><span class="sxs-lookup"><span data-stu-id="9a952-121">Relationships</span></span>
<span data-ttu-id="9a952-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="9a952-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="9a952-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="9a952-123">JSON Representation</span></span>
<span data-ttu-id="9a952-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="9a952-124">Here is a JSON representation of the resource.</span></span>
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




