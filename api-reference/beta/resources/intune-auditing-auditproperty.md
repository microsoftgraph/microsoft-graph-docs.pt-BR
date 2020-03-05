---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 67a70ff1cafab25372931597392c21eb77dd6c7b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42489395"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="62f6e-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="62f6e-103">auditProperty resource type</span></span>

<span data-ttu-id="62f6e-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="62f6e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62f6e-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="62f6e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62f6e-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="62f6e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62f6e-107">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="62f6e-107">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="62f6e-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="62f6e-108">Properties</span></span>
|<span data-ttu-id="62f6e-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="62f6e-109">Property</span></span>|<span data-ttu-id="62f6e-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="62f6e-110">Type</span></span>|<span data-ttu-id="62f6e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="62f6e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62f6e-112">displayName</span><span class="sxs-lookup"><span data-stu-id="62f6e-112">displayName</span></span>|<span data-ttu-id="62f6e-113">String</span><span class="sxs-lookup"><span data-stu-id="62f6e-113">String</span></span>|<span data-ttu-id="62f6e-114">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="62f6e-114">Display name.</span></span>|
|<span data-ttu-id="62f6e-115">oldValue</span><span class="sxs-lookup"><span data-stu-id="62f6e-115">oldValue</span></span>|<span data-ttu-id="62f6e-116">String</span><span class="sxs-lookup"><span data-stu-id="62f6e-116">String</span></span>|<span data-ttu-id="62f6e-117">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="62f6e-117">Old value.</span></span>|
|<span data-ttu-id="62f6e-118">newValue</span><span class="sxs-lookup"><span data-stu-id="62f6e-118">newValue</span></span>|<span data-ttu-id="62f6e-119">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="62f6e-119">String</span></span>|<span data-ttu-id="62f6e-120">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="62f6e-120">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="62f6e-121">Relações</span><span class="sxs-lookup"><span data-stu-id="62f6e-121">Relationships</span></span>
<span data-ttu-id="62f6e-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="62f6e-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="62f6e-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="62f6e-123">JSON Representation</span></span>
<span data-ttu-id="62f6e-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="62f6e-124">Here is a JSON representation of the resource.</span></span>
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



