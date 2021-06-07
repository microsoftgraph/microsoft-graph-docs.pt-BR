---
title: Tipo de recurso auditProperty
description: Uma classe que contém as propriedades para a Propriedade de auditoria.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 900e493ce77fd47a232626ad73999ce3482d4fe6
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52748870"
---
# <a name="auditproperty-resource-type"></a><span data-ttu-id="57f4b-103">Tipo de recurso auditProperty</span><span class="sxs-lookup"><span data-stu-id="57f4b-103">auditProperty resource type</span></span>

<span data-ttu-id="57f4b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="57f4b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="57f4b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="57f4b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="57f4b-106">Uma classe que contém as propriedades para a Propriedade de auditoria.</span><span class="sxs-lookup"><span data-stu-id="57f4b-106">A class containing the properties for Audit Property.</span></span>

## <a name="properties"></a><span data-ttu-id="57f4b-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="57f4b-107">Properties</span></span>
|<span data-ttu-id="57f4b-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="57f4b-108">Property</span></span>|<span data-ttu-id="57f4b-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="57f4b-109">Type</span></span>|<span data-ttu-id="57f4b-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="57f4b-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="57f4b-111">displayName</span><span class="sxs-lookup"><span data-stu-id="57f4b-111">displayName</span></span>|<span data-ttu-id="57f4b-112">String</span><span class="sxs-lookup"><span data-stu-id="57f4b-112">String</span></span>|<span data-ttu-id="57f4b-113">Nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="57f4b-113">Display name.</span></span>|
|<span data-ttu-id="57f4b-114">oldValue</span><span class="sxs-lookup"><span data-stu-id="57f4b-114">oldValue</span></span>|<span data-ttu-id="57f4b-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57f4b-115">String</span></span>|<span data-ttu-id="57f4b-116">Valor antigo.</span><span class="sxs-lookup"><span data-stu-id="57f4b-116">Old value.</span></span>|
|<span data-ttu-id="57f4b-117">newValue</span><span class="sxs-lookup"><span data-stu-id="57f4b-117">newValue</span></span>|<span data-ttu-id="57f4b-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="57f4b-118">String</span></span>|<span data-ttu-id="57f4b-119">Novo valor.</span><span class="sxs-lookup"><span data-stu-id="57f4b-119">New value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="57f4b-120">Relações</span><span class="sxs-lookup"><span data-stu-id="57f4b-120">Relationships</span></span>
<span data-ttu-id="57f4b-121">Nenhum</span><span class="sxs-lookup"><span data-stu-id="57f4b-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="57f4b-122">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="57f4b-122">JSON Representation</span></span>
<span data-ttu-id="57f4b-123">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="57f4b-123">Here is a JSON representation of the resource.</span></span>
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




