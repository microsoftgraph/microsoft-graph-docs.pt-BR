---
title: tipo de recurso profileCardAnnotation
description: Permite que um administrador Personalize a aparência dos campos selecionados no cartão de perfil do Microsoft 365.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 57b6378c811727676f7b34c1812955639598054b
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47973726"
---
# <a name="profilecardannotation-resource-type"></a><span data-ttu-id="bea84-103">tipo de recurso profileCardAnnotation</span><span class="sxs-lookup"><span data-stu-id="bea84-103">profileCardAnnotation resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bea84-104">Usado para definir um nome de exibição personalizado para os campos que são exibidos em um Microsoft 365 People experieence compartilhado.</span><span class="sxs-lookup"><span data-stu-id="bea84-104">Used to set a custom display name for fields that surface in a shared Microsoft 365 people experieence.</span></span> <span data-ttu-id="bea84-105">Um administrador pode definir uma cadeia de caracteres de nome para exibição padrão e um conjunto de traduções alternativas para os idiomas que eles dão suporte em sua organização.</span><span class="sxs-lookup"><span data-stu-id="bea84-105">An administrator can define a default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

## <a name="properties"></a><span data-ttu-id="bea84-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="bea84-106">Properties</span></span>

| <span data-ttu-id="bea84-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="bea84-107">Property</span></span>     | <span data-ttu-id="bea84-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="bea84-108">Type</span></span>                                                            | <span data-ttu-id="bea84-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="bea84-109">Description</span></span>                                                                                                                       |
|:-------------|:----------------------------------------------------------------|:----------------------------------------------------------------------------------------------------------------------------------|
|<span data-ttu-id="bea84-110">displayName</span><span class="sxs-lookup"><span data-stu-id="bea84-110">displayName</span></span>   |<span data-ttu-id="bea84-111">String</span><span class="sxs-lookup"><span data-stu-id="bea84-111">String</span></span>                                                           | <span data-ttu-id="bea84-112">Se presente, o valor desse campo é usado pelo cartão de perfil como rótulo de propriedade padrão na experiência (por exemplo, "centro de custo").</span><span class="sxs-lookup"><span data-stu-id="bea84-112">If present, the value of this field is used by the profile card as the default property label in the experience (for example, "Cost Center").</span></span> |
|<span data-ttu-id="bea84-113">localizações</span><span class="sxs-lookup"><span data-stu-id="bea84-113">localizations</span></span> |<span data-ttu-id="bea84-114">coleção [displayNameLocalization](displaynamelocalization.md)</span><span class="sxs-lookup"><span data-stu-id="bea84-114">[displayNameLocalization](displaynamelocalization.md) collection</span></span> | <span data-ttu-id="bea84-115">Cada recurso dessa coleção representa o valor localizado do nome do atributo para um determinado idioma, usado como rótulo padrão para essa localidade.</span><span class="sxs-lookup"><span data-stu-id="bea84-115">Each resource in this collection represents the localized value of the attribute name for a given language, used as the default label for that locale.</span></span> <span data-ttu-id="bea84-116">Por exemplo, um usuário com um `no-NB` cliente recebe "Kostnads Senter" como o rótulo do atributo, em vez de "centro de custo".</span><span class="sxs-lookup"><span data-stu-id="bea84-116">For example, a user with a `no-NB` client gets "Kostnads Senter" as the attribute label, rather than "Cost Center."</span></span>|

## <a name="json-representation"></a><span data-ttu-id="bea84-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="bea84-117">JSON representation</span></span>

<span data-ttu-id="bea84-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="bea84-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardAnnotation",
  "baseType": null
}-->

```json
{
  "displayName": "String",
  "localizations": [
    {
      "displayName": "String",
      "languageTag": "String"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardAnnotation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


