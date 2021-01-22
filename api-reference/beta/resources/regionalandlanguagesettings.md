---
title: Tipo de recurso regionalAndLanguageSettings
description: Um recurso que representa preferências regionais e de idioma de usuários
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: 66734cba4c5d0e2997a4bfd5b70c54156821f5da
ms.sourcegitcommit: 744c2d8be5a1ce158068bcfeaad1aabf8166c556
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/22/2021
ms.locfileid: "49934909"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="8ec37-103">Tipo de recurso regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="8ec37-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="8ec37-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ec37-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ec37-105">Um tipo aberto que representa as preferências de um usuário para idiomas em vários contextos e para a localidade regional e a formatação que orientam o calendário padrão e a formatação de data e hora.</span><span class="sxs-lookup"><span data-stu-id="8ec37-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="8ec37-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="8ec37-106">Methods</span></span>

| <span data-ttu-id="8ec37-107">Método</span><span class="sxs-lookup"><span data-stu-id="8ec37-107">Method</span></span>                                                 | <span data-ttu-id="8ec37-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ec37-108">Return Type</span></span>                                                   | <span data-ttu-id="8ec37-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec37-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="8ec37-110">Get</span><span class="sxs-lookup"><span data-stu-id="8ec37-110">Get</span></span>](../api/regionalAndLanguageSettings-get.md)       | [<span data-ttu-id="8ec37-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="8ec37-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="8ec37-112">Ler propriedades de um **objeto regionalAndLanguageSettings.**</span><span class="sxs-lookup"><span data-stu-id="8ec37-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="8ec37-113">Update</span><span class="sxs-lookup"><span data-stu-id="8ec37-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="8ec37-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="8ec37-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="8ec37-115">Atualize todo ou um subconjunto das propriedades do **objeto regionalAndLanguageSettings** para um usuário.</span><span class="sxs-lookup"><span data-stu-id="8ec37-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ec37-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ec37-116">Properties</span></span>
| <span data-ttu-id="8ec37-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ec37-117">Property</span></span>                   | <span data-ttu-id="8ec37-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ec37-118">Type</span></span>                                                  | <span data-ttu-id="8ec37-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ec37-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8ec37-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="8ec37-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="8ec37-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ec37-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="8ec37-122">Idioma preferencial da interface do usuário (menus, botões, faixas de opções, mensagens de aviso) para aplicativos Web da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8ec37-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="8ec37-123">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ec37-123">Returned by default.</span></span> <span data-ttu-id="8ec37-124">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="8ec37-124">Not nullable.</span></span> |
| <span data-ttu-id="8ec37-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="8ec37-125">authoringLanguages</span></span>         | <span data-ttu-id="8ec37-126">Coleção localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ec37-126">localeInfo collection</span></span>                                 | <span data-ttu-id="8ec37-127">Lista priorizada de idiomas em que o usuário lê e os autores.</span><span class="sxs-lookup"><span data-stu-id="8ec37-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="8ec37-128">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ec37-128">Returned by default.</span></span> <span data-ttu-id="8ec37-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="8ec37-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="8ec37-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="8ec37-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="8ec37-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ec37-131">localeInfo</span></span>                                            | <span data-ttu-id="8ec37-132">O idioma em que um usuário espera ter documentos, emails e mensagens traduzidos.</span><span class="sxs-lookup"><span data-stu-id="8ec37-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="8ec37-133">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ec37-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="8ec37-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="8ec37-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="8ec37-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ec37-135">localeInfo</span></span>                                            | <span data-ttu-id="8ec37-136">O idioma que um usuário esperava usar como entrada para cenários de texto em fala.</span><span class="sxs-lookup"><span data-stu-id="8ec37-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="8ec37-137">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ec37-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="8ec37-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="8ec37-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="8ec37-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ec37-139">localeInfo</span></span>                                            | <span data-ttu-id="8ec37-140">A localidade que orienta a formatação padrão de data, hora e calendário.</span><span class="sxs-lookup"><span data-stu-id="8ec37-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="8ec37-141">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ec37-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="8ec37-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="8ec37-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="8ec37-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="8ec37-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="8ec37-144">Permite que o usuário substitua defaultRegionalFormat por formatos específicos de campo.</span><span class="sxs-lookup"><span data-stu-id="8ec37-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="8ec37-145">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ec37-145">Returned by default.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="8ec37-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ec37-146">JSON representation</span></span>

<span data-ttu-id="8ec37-147">A seguir está uma definição JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ec37-147">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages": [{"@odata.type":"microsoft.graph.localeInfo"}],
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat": {"@odata.type":"microsoft.graph.localeInfo"},
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


