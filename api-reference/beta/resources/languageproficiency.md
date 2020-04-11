---
title: tipo de recurso languageProficiency
description: tipo de recurso languageProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 48a9e26bde5d06b834c542cbb987a2faff9fc23c
ms.sourcegitcommit: 9a6ce4ddf75beead19b7c35a1949cf4d105b9b29
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2020
ms.locfileid: "43229392"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="e59e1-103">tipo de recurso languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e59e1-103">languageProficiency resource type</span></span>

<span data-ttu-id="e59e1-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e59e1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e59e1-105">Representa informações detalhadas sobre os idiomas que um usuário adicionou ao [perfil](profile.md).</span><span class="sxs-lookup"><span data-stu-id="e59e1-105">Represents detailed information about languages that a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="e59e1-106">Herda de [Myfacet](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="e59e1-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="e59e1-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="e59e1-107">Methods</span></span>

| <span data-ttu-id="e59e1-108">Método</span><span class="sxs-lookup"><span data-stu-id="e59e1-108">Method</span></span>                                                              | <span data-ttu-id="e59e1-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="e59e1-109">Return Type</span></span>                                   | <span data-ttu-id="e59e1-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59e1-110">Description</span></span>                                                                |
|:--------------------------------------------------------------------|:----------------------------------------------|:---------------------------------------------------------------------------|
| [<span data-ttu-id="e59e1-111">Obter languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e59e1-111">Get languageProficiency</span></span>](../api/languageproficiency-get.md)        | [<span data-ttu-id="e59e1-112">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e59e1-112">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="e59e1-113">Leia as propriedades e os relacionamentos de um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="e59e1-113">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="e59e1-114">Atualizar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e59e1-114">Update languageProficiency</span></span>](../api/languageproficiency-update.md)  | [<span data-ttu-id="e59e1-115">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e59e1-115">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="e59e1-116">Atualizar um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="e59e1-116">Update a **languageProficiency** object.</span></span>                                   |
| [<span data-ttu-id="e59e1-117">Excluir languageProficiency</span><span class="sxs-lookup"><span data-stu-id="e59e1-117">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)  | <span data-ttu-id="e59e1-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e59e1-118">None</span></span>                                          | <span data-ttu-id="e59e1-119">Excluir um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="e59e1-119">Delete a **languageProficiency** object.</span></span>                                   |

## <a name="properties"></a><span data-ttu-id="e59e1-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e59e1-120">Properties</span></span>

| <span data-ttu-id="e59e1-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e59e1-121">Property</span></span>     | <span data-ttu-id="e59e1-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="e59e1-122">Type</span></span>        | <span data-ttu-id="e59e1-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="e59e1-123">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="e59e1-124">displayName</span><span class="sxs-lookup"><span data-stu-id="e59e1-124">displayName</span></span>   |<span data-ttu-id="e59e1-125">String</span><span class="sxs-lookup"><span data-stu-id="e59e1-125">String</span></span>       | <span data-ttu-id="e59e1-126">Contém o nome de formato longo para o idioma.</span><span class="sxs-lookup"><span data-stu-id="e59e1-126">Contains the long-form name for the language.</span></span>                                                                                                               |
|<span data-ttu-id="e59e1-127">proficiência</span><span class="sxs-lookup"><span data-stu-id="e59e1-127">proficiency</span></span>   |<span data-ttu-id="e59e1-128">string</span><span class="sxs-lookup"><span data-stu-id="e59e1-128">string</span></span>       | <span data-ttu-id="e59e1-129">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="e59e1-129">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="e59e1-130">tag</span><span class="sxs-lookup"><span data-stu-id="e59e1-130">tag</span></span>           |<span data-ttu-id="e59e1-131">String</span><span class="sxs-lookup"><span data-stu-id="e59e1-131">String</span></span>       | <span data-ttu-id="e59e1-132">Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).</span><span class="sxs-lookup"><span data-stu-id="e59e1-132">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                              |

## <a name="relationships"></a><span data-ttu-id="e59e1-133">Relações</span><span class="sxs-lookup"><span data-stu-id="e59e1-133">Relationships</span></span>

<span data-ttu-id="e59e1-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e59e1-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e59e1-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e59e1-135">JSON representation</span></span>

<span data-ttu-id="e59e1-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e59e1-136">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.languageProficiency",
  "baseType": ""
}-->

```json
{
  "displayName": "String",
  "proficiency": "string",
  "tag": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "languageProficiency resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
