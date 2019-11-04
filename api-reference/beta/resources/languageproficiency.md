---
title: tipo de recurso languageProficiency
description: tipo de recurso languageProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 4e2ea70eca4e830ef334e5bf61be724cb05f1cfc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939289"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="17da3-103">tipo de recurso languageProficiency</span><span class="sxs-lookup"><span data-stu-id="17da3-103">languageProficiency resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17da3-104">Representa informações detalhadas sobre os idiomas que um usuário adicionou ao [perfil](profile.md).</span><span class="sxs-lookup"><span data-stu-id="17da3-104">Represents detailed information about a languages a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="17da3-105">Herda de [Myfacet](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="17da3-105">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="17da3-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="17da3-106">Methods</span></span>

| <span data-ttu-id="17da3-107">Método</span><span class="sxs-lookup"><span data-stu-id="17da3-107">Method</span></span>                                                       | <span data-ttu-id="17da3-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="17da3-108">Return Type</span></span>                                   | <span data-ttu-id="17da3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="17da3-109">Description</span></span>                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="17da3-110">Obter languageProficiency</span><span class="sxs-lookup"><span data-stu-id="17da3-110">Get languageProficiency</span></span>](../api/languageproficiency-get.md) | [<span data-ttu-id="17da3-111">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="17da3-111">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="17da3-112">Leia as propriedades e os relacionamentos de um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="17da3-112">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="17da3-113">Atualizar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="17da3-113">Update languageProficiency</span></span>](../api/languageproficiency-update.md)               | [<span data-ttu-id="17da3-114">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="17da3-114">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="17da3-115">Atualizar um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="17da3-115">Update a **languageProficiency** object.</span></span>                               |
| [<span data-ttu-id="17da3-116">Excluir languageProficiency</span><span class="sxs-lookup"><span data-stu-id="17da3-116">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)               | <span data-ttu-id="17da3-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17da3-117">None</span></span>                                          | <span data-ttu-id="17da3-118">Excluir um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="17da3-118">Delete a **languageProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="17da3-119">Propriedades</span><span class="sxs-lookup"><span data-stu-id="17da3-119">Properties</span></span>

| <span data-ttu-id="17da3-120">Propriedade</span><span class="sxs-lookup"><span data-stu-id="17da3-120">Property</span></span>     | <span data-ttu-id="17da3-121">Tipo</span><span class="sxs-lookup"><span data-stu-id="17da3-121">Type</span></span>        | <span data-ttu-id="17da3-122">Descrição</span><span class="sxs-lookup"><span data-stu-id="17da3-122">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="17da3-123">displayName</span><span class="sxs-lookup"><span data-stu-id="17da3-123">displayName</span></span>   |<span data-ttu-id="17da3-124">String</span><span class="sxs-lookup"><span data-stu-id="17da3-124">String</span></span>       | <span data-ttu-id="17da3-125">Contém o nome de formato longo para o idioma.</span><span class="sxs-lookup"><span data-stu-id="17da3-125">Contains the long-form name for the language.</span></span>                                                                                                   |
|<span data-ttu-id="17da3-126">proficiência</span><span class="sxs-lookup"><span data-stu-id="17da3-126">proficiency</span></span>   |<span data-ttu-id="17da3-127">string</span><span class="sxs-lookup"><span data-stu-id="17da3-127">string</span></span>       | <span data-ttu-id="17da3-128">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="17da3-128">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="17da3-129">tag</span><span class="sxs-lookup"><span data-stu-id="17da3-129">tag</span></span>           |<span data-ttu-id="17da3-130">String</span><span class="sxs-lookup"><span data-stu-id="17da3-130">String</span></span>       | <span data-ttu-id="17da3-131">Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).</span><span class="sxs-lookup"><span data-stu-id="17da3-131">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                                  |

## <a name="relationships"></a><span data-ttu-id="17da3-132">Relações</span><span class="sxs-lookup"><span data-stu-id="17da3-132">Relationships</span></span>

<span data-ttu-id="17da3-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="17da3-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="17da3-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="17da3-134">JSON representation</span></span>

<span data-ttu-id="17da3-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="17da3-135">The following is a JSON representation of the resource.</span></span> 

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
