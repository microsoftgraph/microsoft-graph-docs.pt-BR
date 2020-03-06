---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c63f390e31e83cfed64ee2a28bba4e4af0dfa756
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532731"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="7d561-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="7d561-103">auditProperty resource type</span></span>

<span data-ttu-id="7d561-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d561-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d561-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7d561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d561-106">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="7d561-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="7d561-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7d561-107">Properties</span></span>
|<span data-ttu-id="7d561-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7d561-108">Property</span></span>|<span data-ttu-id="7d561-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="7d561-109">Type</span></span>|<span data-ttu-id="7d561-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="7d561-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d561-111">displayName</span><span class="sxs-lookup"><span data-stu-id="7d561-111">displayName</span></span>|<span data-ttu-id="7d561-112">String</span><span class="sxs-lookup"><span data-stu-id="7d561-112">String</span></span>|<span data-ttu-id="7d561-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="7d561-113">Display name.</span></span>|
|<span data-ttu-id="7d561-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="7d561-114">oldValue</span></span>|<span data-ttu-id="7d561-115">String</span><span class="sxs-lookup"><span data-stu-id="7d561-115">String</span></span>|<span data-ttu-id="7d561-116">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="7d561-116">Old value.</span></span>|
|<span data-ttu-id="7d561-117">newValue</span><span class="sxs-lookup"><span data-stu-id="7d561-117">newValue</span></span>|<span data-ttu-id="7d561-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7d561-118">String</span></span>|<span data-ttu-id="7d561-119">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="7d561-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="7d561-120">Relações</span><span class="sxs-lookup"><span data-stu-id="7d561-120">Relationships</span></span>
<span data-ttu-id="7d561-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="7d561-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7d561-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7d561-122">JSON Representation</span></span>
<span data-ttu-id="7d561-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="7d561-123">Here is a JSON representation of the resource.</span></span>
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




