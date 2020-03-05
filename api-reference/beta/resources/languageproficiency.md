---
title: tipo de recurso languageProficiency
description: tipo de recurso languageProficiency
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0934ea66c15e090a4f9ba9bcaa62a6c7eb900cd5
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522992"
---
# <a name="languageproficiency-resource-type"></a><span data-ttu-id="a7403-103">tipo de recurso languageProficiency</span><span class="sxs-lookup"><span data-stu-id="a7403-103">languageProficiency resource type</span></span>

<span data-ttu-id="a7403-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="a7403-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7403-105">Representa informações detalhadas sobre os idiomas que um usuário adicionou ao [perfil](profile.md).</span><span class="sxs-lookup"><span data-stu-id="a7403-105">Represents detailed information about languages that a user has added to their [profile](profile.md).</span></span>

<span data-ttu-id="a7403-106">Herda de [Myfacet](itemFacet.md).</span><span class="sxs-lookup"><span data-stu-id="a7403-106">Inherits from [itemFacet](itemFacet.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a7403-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a7403-107">Methods</span></span>

| <span data-ttu-id="a7403-108">Método</span><span class="sxs-lookup"><span data-stu-id="a7403-108">Method</span></span>                                                       | <span data-ttu-id="a7403-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a7403-109">Return Type</span></span>                                   | <span data-ttu-id="a7403-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7403-110">Description</span></span>                                                      | 
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="a7403-111">Obter languageProficiency</span><span class="sxs-lookup"><span data-stu-id="a7403-111">Get languageProficiency</span></span>](../api/languageproficiency-get.md) | [<span data-ttu-id="a7403-112">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="a7403-112">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="a7403-113">Leia as propriedades e os relacionamentos de um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="a7403-113">Read the properties and relationships of a **languageProficiency** object.</span></span> |
| [<span data-ttu-id="a7403-114">Atualizar languageProficiency</span><span class="sxs-lookup"><span data-stu-id="a7403-114">Update languageProficiency</span></span>](../api/languageproficiency-update.md)               | [<span data-ttu-id="a7403-115">languageProficiency</span><span class="sxs-lookup"><span data-stu-id="a7403-115">languageProficiency</span></span>](languageproficiency.md) | <span data-ttu-id="a7403-116">Atualizar um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="a7403-116">Update a **languageProficiency** object.</span></span>                               |
| [<span data-ttu-id="a7403-117">Excluir languageProficiency</span><span class="sxs-lookup"><span data-stu-id="a7403-117">Delete languageProficiency</span></span>](../api/languageproficiency-delete.md)               | <span data-ttu-id="a7403-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7403-118">None</span></span>                                          | <span data-ttu-id="a7403-119">Excluir um objeto **languageProficiency** .</span><span class="sxs-lookup"><span data-stu-id="a7403-119">Delete a **languageProficiency** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="a7403-120">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a7403-120">Properties</span></span>

| <span data-ttu-id="a7403-121">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7403-121">Property</span></span>     | <span data-ttu-id="a7403-122">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7403-122">Type</span></span>        | <span data-ttu-id="a7403-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7403-123">Description</span></span>                                                                                                                                                 |
|:-------------|:------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="a7403-124">displayName</span><span class="sxs-lookup"><span data-stu-id="a7403-124">displayName</span></span>   |<span data-ttu-id="a7403-125">String</span><span class="sxs-lookup"><span data-stu-id="a7403-125">String</span></span>       | <span data-ttu-id="a7403-126">Contém o nome de formato longo para o idioma.</span><span class="sxs-lookup"><span data-stu-id="a7403-126">Contains the long-form name for the language.</span></span>                                                                                                   |
|<span data-ttu-id="a7403-127">proficiência</span><span class="sxs-lookup"><span data-stu-id="a7403-127">proficiency</span></span>   |<span data-ttu-id="a7403-128">string</span><span class="sxs-lookup"><span data-stu-id="a7403-128">string</span></span>       | <span data-ttu-id="a7403-129">Os valores possíveis são: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="a7403-129">Possible values are: `elementary`, `conversational`, `limitedWorking`, `professionalWorking`, `fullProfessional`, `nativeOrBilingual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="a7403-130">tag</span><span class="sxs-lookup"><span data-stu-id="a7403-130">tag</span></span>           |<span data-ttu-id="a7403-131">String</span><span class="sxs-lookup"><span data-stu-id="a7403-131">String</span></span>       | <span data-ttu-id="a7403-132">Contém o nome BCP47 de quatro caracteres para o idioma (en-US, no-NB, en-AU).</span><span class="sxs-lookup"><span data-stu-id="a7403-132">Contains the four-character BCP47 name for the language (en-US, no-NB, en-AU).</span></span>                                                                                  |

## <a name="relationships"></a><span data-ttu-id="a7403-133">Relações</span><span class="sxs-lookup"><span data-stu-id="a7403-133">Relationships</span></span>

<span data-ttu-id="a7403-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a7403-134">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a7403-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a7403-135">JSON representation</span></span>

<span data-ttu-id="a7403-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a7403-136">The following is a JSON representation of the resource.</span></span> 

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
