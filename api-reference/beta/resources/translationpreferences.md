---
title: Tipo de recurso translationPreferences
description: Um recurso que representa as preferências de configurações de conversão do usuário.
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: b2e45f797709067e52f142c3de3f2be566b55201
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50518137"
---
# <a name="translationpreferences-resource-type"></a><span data-ttu-id="aa8ac-103">Tipo de recurso translationPreferences</span><span class="sxs-lookup"><span data-stu-id="aa8ac-103">translationPreferences resource type</span></span>

<span data-ttu-id="aa8ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa8ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa8ac-105">Representa uma entrada na lista de substituição de idioma de tradução de um usuário.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-105">Represents an entry in a user's translation language override list.</span></span>

## <a name="properties"></a><span data-ttu-id="aa8ac-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aa8ac-106">Properties</span></span>

|<span data-ttu-id="aa8ac-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aa8ac-107">Property</span></span>             |<span data-ttu-id="aa8ac-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="aa8ac-108">Type</span></span>                                         |<span data-ttu-id="aa8ac-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa8ac-109">Description</span></span>                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|<span data-ttu-id="aa8ac-110">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="aa8ac-110">translationBehavior</span></span>  |[<span data-ttu-id="aa8ac-111">translationBehavior</span><span class="sxs-lookup"><span data-stu-id="aa8ac-111">translationBehavior</span></span>](#translationbehavior-values)       |<span data-ttu-id="aa8ac-112">O comportamento de conversão preferencial do usuário.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-112">The user's preferred translation behavior.</span></span><br><br><span data-ttu-id="aa8ac-113">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-113">Returned by default.</span></span> <span data-ttu-id="aa8ac-114">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-114">Not nullable.</span></span> |                   
|<span data-ttu-id="aa8ac-115">languageOverrides</span><span class="sxs-lookup"><span data-stu-id="aa8ac-115">languageOverrides</span></span>    |<span data-ttu-id="aa8ac-116">[Coleção translationLanguageOverride](translationLanguageOverride.md)</span><span class="sxs-lookup"><span data-stu-id="aa8ac-116">[translationLanguageOverride](translationLanguageOverride.md) collection</span></span>                | <span data-ttu-id="aa8ac-117">Comportamento de substituição de conversão para idiomas, se for o caso.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-117">Translation override behavior for languages, if any.</span></span><br><br><span data-ttu-id="aa8ac-118">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-118">Returned by default.</span></span>|
|<span data-ttu-id="aa8ac-119">untranslatedLanguages</span><span class="sxs-lookup"><span data-stu-id="aa8ac-119">untranslatedLanguages</span></span>|<span data-ttu-id="aa8ac-120">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aa8ac-120">String collection</span></span>| <span data-ttu-id="aa8ac-121">A lista de idiomas que o usuário não precisa traduzir.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-121">The list of languages the user does not need translated.</span></span> <span data-ttu-id="aa8ac-122">Isso é calculado da coleção **authoringLanguages** [em regionalAndLanguageSettings](regionalandlanguagesettings.md)e da coleção **languageOverrides** em **translationPreferences**.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-122">This is computed from the **authoringLanguages** collection in [regionalAndLanguageSettings](regionalandlanguagesettings.md), and the **languageOverrides** collection in **translationPreferences**.</span></span> <span data-ttu-id="aa8ac-123">A lista especifica valores de cultura neutros que incluem o código de idioma sem qualquer associação de país ou região.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-123">The list specifies neutral culture values that include the language code without any country or region association.</span></span> <span data-ttu-id="aa8ac-124">Por exemplo, ele especificaria "fr" para a cultura francesa neutra, mas não "fr-FR" para a cultura francesa na França.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-124">For example, it would specify "fr" for the neutral French culture, but not "fr-FR" for the French culture in France.</span></span> <br><br><span data-ttu-id="aa8ac-125">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-125">Returned by default.</span></span> <span data-ttu-id="aa8ac-126">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-126">Read only.</span></span>| 

### <a name="translationbehavior-values"></a><span data-ttu-id="aa8ac-127">valores translationBehavior</span><span class="sxs-lookup"><span data-stu-id="aa8ac-127">translationBehavior values</span></span>

|<span data-ttu-id="aa8ac-128">Member</span><span class="sxs-lookup"><span data-stu-id="aa8ac-128">Member</span></span> |<span data-ttu-id="aa8ac-129">Descrição</span><span class="sxs-lookup"><span data-stu-id="aa8ac-129">Description</span></span>                                                                  |
|-------|-----------------------------------------------------------------------------|
|<span data-ttu-id="aa8ac-130">Pergunte</span><span class="sxs-lookup"><span data-stu-id="aa8ac-130">Ask</span></span>    |<span data-ttu-id="aa8ac-131">Solicitar ao usuário antes de traduzir as mensagens/chats/páginas da Web para o usuário.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-131">Prompt the user before translating the messages/chats/web pages for the user.</span></span>|
|<span data-ttu-id="aa8ac-132">Sim</span><span class="sxs-lookup"><span data-stu-id="aa8ac-132">Yes</span></span>    |<span data-ttu-id="aa8ac-133">Traduza automaticamente as mensagens/chats/páginas da Web para o usuário.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-133">Automatically translate the messages/chats/web pages for the user.</span></span>           |
|<span data-ttu-id="aa8ac-134">Não</span><span class="sxs-lookup"><span data-stu-id="aa8ac-134">No</span></span>     |<span data-ttu-id="aa8ac-135">Não ofereça tradução automática ou solicitada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-135">Do not offer prompted or automatic translation for the user.</span></span>                 |



## <a name="json-representation"></a><span data-ttu-id="aa8ac-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aa8ac-136">JSON representation</span></span>

<span data-ttu-id="aa8ac-137">A seguir está uma definição JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aa8ac-137">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.translationPreferences"
}-->

```json
{
    "translationBehavior": "string",
    "languageOverrides": [{"@odata.type":"microsoft.graph.translationLanguageOverride"}],
    "untranslatedLanguages": ["string"]
}
```
<!-- {
  "type": "#page.annotation",
  "description": translationPreferences resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


