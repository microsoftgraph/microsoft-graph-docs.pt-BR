---
title: tipo de recurso de configuração
description: Representa uma configuração usada em uma linha de base.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 2545dc6aa11668359fa9dda636412d36f8d92de1
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402141"
---
# <a name="setting-resource-type"></a><span data-ttu-id="458d4-103">tipo de recurso de configuração</span><span class="sxs-lookup"><span data-stu-id="458d4-103">setting resource type</span></span>

<span data-ttu-id="458d4-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="458d4-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="458d4-105">Representa uma configuração usada em uma linha de base.</span><span class="sxs-lookup"><span data-stu-id="458d4-105">Represents a setting that is used within a baseline.</span></span>

## <a name="properties"></a><span data-ttu-id="458d4-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="458d4-106">Properties</span></span>
|<span data-ttu-id="458d4-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="458d4-107">Property</span></span>|<span data-ttu-id="458d4-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="458d4-108">Type</span></span>|<span data-ttu-id="458d4-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="458d4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="458d4-110">displayName</span><span class="sxs-lookup"><span data-stu-id="458d4-110">displayName</span></span>|<span data-ttu-id="458d4-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="458d4-111">String</span></span>|<span data-ttu-id="458d4-112">O nome de exibição da configuração.</span><span class="sxs-lookup"><span data-stu-id="458d4-112">The display name for the setting.</span></span> <span data-ttu-id="458d4-113">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458d4-113">Required.</span></span> <span data-ttu-id="458d4-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="458d4-114">Read-only.</span></span>|
|<span data-ttu-id="458d4-115">jsonValue</span><span class="sxs-lookup"><span data-stu-id="458d4-115">jsonValue</span></span>|<span data-ttu-id="458d4-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="458d4-116">String</span></span>|<span data-ttu-id="458d4-117">O valor da configuração serializada como cadeia de caracteres de JSON.</span><span class="sxs-lookup"><span data-stu-id="458d4-117">The value for the setting serialized as string of JSON.</span></span> <span data-ttu-id="458d4-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458d4-118">Required.</span></span> <span data-ttu-id="458d4-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="458d4-119">Read-only.</span></span>|
|<span data-ttu-id="458d4-120">overwriteAllowed</span><span class="sxs-lookup"><span data-stu-id="458d4-120">overwriteAllowed</span></span>|<span data-ttu-id="458d4-121">Boolean</span><span class="sxs-lookup"><span data-stu-id="458d4-121">Boolean</span></span>|<span data-ttu-id="458d4-122">Um sinalizador indicando se a configuração pode substituir as configurações existentes quando aplicada.</span><span class="sxs-lookup"><span data-stu-id="458d4-122">A flag indicating whether the setting can be override existing configurations when applied.</span></span> <span data-ttu-id="458d4-123">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458d4-123">Required.</span></span> <span data-ttu-id="458d4-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="458d4-124">Read-only.</span></span>|
|<span data-ttu-id="458d4-125">valueType</span><span class="sxs-lookup"><span data-stu-id="458d4-125">valueType</span></span>|<span data-ttu-id="458d4-126">managementParameterValueType</span><span class="sxs-lookup"><span data-stu-id="458d4-126">managementParameterValueType</span></span>|<span data-ttu-id="458d4-127">O tipo de dados da configuração.</span><span class="sxs-lookup"><span data-stu-id="458d4-127">The data type for the setting.</span></span> <span data-ttu-id="458d4-128">Os valores possíveis são: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="458d4-128">Possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span></span> <span data-ttu-id="458d4-129">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="458d4-129">Required.</span></span> <span data-ttu-id="458d4-130">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="458d4-130">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="458d4-131">Relações</span><span class="sxs-lookup"><span data-stu-id="458d4-131">Relationships</span></span>
<span data-ttu-id="458d4-132">Nenhum</span><span class="sxs-lookup"><span data-stu-id="458d4-132">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="458d4-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="458d4-133">JSON representation</span></span>
<span data-ttu-id="458d4-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="458d4-134">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.setting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.setting",
  "displayName": "String",
  "overwriteAllowed": "Boolean",
  "valueType": "String",
  "jsonValue": "String"
}
```
