---
title: Tipo de recurso templateParameter
description: Representa um parâmetro usado em um modelo de gerenciamento.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f533bc375e2d7e4a1e4ef2f7f801f248c1801c4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402139"
---
# <a name="templateparameter-resource-type"></a><span data-ttu-id="af11e-103">Tipo de recurso templateParameter</span><span class="sxs-lookup"><span data-stu-id="af11e-103">templateParameter resource type</span></span>

<span data-ttu-id="af11e-104">Namespace: microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="af11e-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af11e-105">Representa um parâmetro usado em um modelo de gerenciamento.</span><span class="sxs-lookup"><span data-stu-id="af11e-105">Represents a parameter utilized in a management template.</span></span>

## <a name="properties"></a><span data-ttu-id="af11e-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="af11e-106">Properties</span></span>
|<span data-ttu-id="af11e-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="af11e-107">Property</span></span>|<span data-ttu-id="af11e-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="af11e-108">Type</span></span>|<span data-ttu-id="af11e-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="af11e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af11e-110">description</span><span class="sxs-lookup"><span data-stu-id="af11e-110">description</span></span>|<span data-ttu-id="af11e-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af11e-111">String</span></span>|<span data-ttu-id="af11e-112">A descrição do parâmetro template.</span><span class="sxs-lookup"><span data-stu-id="af11e-112">The description for the template parameter.</span></span> <span data-ttu-id="af11e-113">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af11e-113">Optional.</span></span> <span data-ttu-id="af11e-114">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11e-114">Read-only.</span></span>|
|<span data-ttu-id="af11e-115">displayName</span><span class="sxs-lookup"><span data-stu-id="af11e-115">displayName</span></span>|<span data-ttu-id="af11e-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af11e-116">String</span></span>|<span data-ttu-id="af11e-117">O nome de exibição do parâmetro template.</span><span class="sxs-lookup"><span data-stu-id="af11e-117">The display name for the template parameter.</span></span> <span data-ttu-id="af11e-118">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af11e-118">Required.</span></span> <span data-ttu-id="af11e-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11e-119">Read-only.</span></span>|
|<span data-ttu-id="af11e-120">jsonAllowedValues</span><span class="sxs-lookup"><span data-stu-id="af11e-120">jsonAllowedValues</span></span>|<span data-ttu-id="af11e-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af11e-121">String</span></span>|<span data-ttu-id="af11e-122">Os valores permitidos para o parâmetro template representados por uma cadeia de caracteres serializada de JSON.</span><span class="sxs-lookup"><span data-stu-id="af11e-122">The allowed values for the template parameter represented by a serialized string of JSON.</span></span> <span data-ttu-id="af11e-123">Opcional.</span><span class="sxs-lookup"><span data-stu-id="af11e-123">Optional.</span></span> <span data-ttu-id="af11e-124">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11e-124">Read-only.</span></span>|
|<span data-ttu-id="af11e-125">jsonDefaultValue</span><span class="sxs-lookup"><span data-stu-id="af11e-125">jsonDefaultValue</span></span>|<span data-ttu-id="af11e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="af11e-126">String</span></span>|<span data-ttu-id="af11e-127">O valor padrão para o parâmetro template representado por uma cadeia de caracteres serializada de JSON.</span><span class="sxs-lookup"><span data-stu-id="af11e-127">The default value for the template parameter represented by a serialized string of JSON.</span></span> <span data-ttu-id="af11e-128">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af11e-128">Required.</span></span> <span data-ttu-id="af11e-129">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11e-129">Read-only.</span></span>|
|<span data-ttu-id="af11e-130">valueType</span><span class="sxs-lookup"><span data-stu-id="af11e-130">valueType</span></span>|<span data-ttu-id="af11e-131">managementParameterValueType</span><span class="sxs-lookup"><span data-stu-id="af11e-131">managementParameterValueType</span></span>|<span data-ttu-id="af11e-132">O tipo de dados do parâmetro template..</span><span class="sxs-lookup"><span data-stu-id="af11e-132">The data type for the template parameter..</span></span> <span data-ttu-id="af11e-133">Os valores possíveis são: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="af11e-133">Possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span></span> <span data-ttu-id="af11e-134">Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="af11e-134">Required.</span></span> <span data-ttu-id="af11e-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="af11e-135">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="af11e-136">Relações</span><span class="sxs-lookup"><span data-stu-id="af11e-136">Relationships</span></span>
<span data-ttu-id="af11e-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="af11e-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af11e-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="af11e-138">JSON representation</span></span>
<span data-ttu-id="af11e-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="af11e-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateParameter",
  "displayName": "String",
  "description": "String",
  "valueType": "String",
  "jsonDefaultValue": "String",
  "jsonAllowedValues": "String"
}
```
