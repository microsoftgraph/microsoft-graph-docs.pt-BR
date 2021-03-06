---
title: Tipo de recurso regionalAndLanguageSettings
description: Um recurso que representa as preferências regionais e de idioma dos usuários
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: d5fd77038735ed1faa175d77ed2bd10b3b2ef784
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516483"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="abf24-103">Tipo de recurso regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="abf24-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="abf24-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="abf24-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="abf24-105">Um tipo aberto que representa as preferências de um usuário para idiomas em vários contextos e para a localidade regional e a formatação que conduz o calendário padrão e a formatação para data e hora.</span><span class="sxs-lookup"><span data-stu-id="abf24-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="abf24-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="abf24-106">Methods</span></span>

| <span data-ttu-id="abf24-107">Método</span><span class="sxs-lookup"><span data-stu-id="abf24-107">Method</span></span>                                                 | <span data-ttu-id="abf24-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="abf24-108">Return Type</span></span>                                                   | <span data-ttu-id="abf24-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="abf24-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="abf24-110">Get</span><span class="sxs-lookup"><span data-stu-id="abf24-110">Get</span></span>](../api/regionalAndLanguageSettings-get.md)       | [<span data-ttu-id="abf24-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="abf24-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="abf24-112">Ler propriedades de **um objeto regionalAndLanguageSettings.**</span><span class="sxs-lookup"><span data-stu-id="abf24-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="abf24-113">Update</span><span class="sxs-lookup"><span data-stu-id="abf24-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="abf24-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="abf24-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="abf24-115">Atualize todo ou um subconjunto das propriedades do **objeto regionalAndLanguageSettings** para um usuário.</span><span class="sxs-lookup"><span data-stu-id="abf24-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="abf24-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="abf24-116">Properties</span></span>
| <span data-ttu-id="abf24-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="abf24-117">Property</span></span>                   | <span data-ttu-id="abf24-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="abf24-118">Type</span></span>                                                  | <span data-ttu-id="abf24-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="abf24-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="abf24-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="abf24-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="abf24-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="abf24-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="abf24-122">Idioma de interface do usuário preferencial do usuário (menus, botões, faixas de opções, mensagens de aviso) para aplicativos Web da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="abf24-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="abf24-123">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-123">Returned by default.</span></span> <span data-ttu-id="abf24-124">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="abf24-124">Not nullable.</span></span> |
| <span data-ttu-id="abf24-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="abf24-125">authoringLanguages</span></span>         | <span data-ttu-id="abf24-126">Coleção localeInfo</span><span class="sxs-lookup"><span data-stu-id="abf24-126">localeInfo collection</span></span>                                 | <span data-ttu-id="abf24-127">Lista priorizada de idiomas em que o usuário lê e os autores.</span><span class="sxs-lookup"><span data-stu-id="abf24-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="abf24-128">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-128">Returned by default.</span></span> <span data-ttu-id="abf24-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="abf24-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="abf24-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="abf24-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="abf24-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="abf24-131">localeInfo</span></span>                                            | <span data-ttu-id="abf24-132">O idioma em que um usuário espera ter documentos, emails e mensagens convertidos.</span><span class="sxs-lookup"><span data-stu-id="abf24-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="abf24-133">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="abf24-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="abf24-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="abf24-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="abf24-135">localeInfo</span></span>                                            | <span data-ttu-id="abf24-136">O idioma que um usuário espera usar como entrada para cenários de texto em fala.</span><span class="sxs-lookup"><span data-stu-id="abf24-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="abf24-137">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="abf24-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="abf24-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="abf24-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="abf24-139">localeInfo</span></span>                                            | <span data-ttu-id="abf24-140">A localidade que conduz a formatação padrão de data, hora e calendário.</span><span class="sxs-lookup"><span data-stu-id="abf24-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="abf24-141">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="abf24-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="abf24-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="abf24-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="abf24-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="abf24-144">Permite que um usuário substitua seu defaultRegionalFormat por formatos específicos de campo.</span><span class="sxs-lookup"><span data-stu-id="abf24-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="abf24-145">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-145">Returned by default.</span></span>                                                      |
| <span data-ttu-id="abf24-146">translationPreferences</span><span class="sxs-lookup"><span data-stu-id="abf24-146">translationPreferences</span></span>     | [<span data-ttu-id="abf24-147">translationPreferences</span><span class="sxs-lookup"><span data-stu-id="abf24-147">translationPreferences</span></span>](translationPreferences.md)   | <span data-ttu-id="abf24-148">As configurações preferidas do usuário ao consumir documentos convertidos, emails, mensagens e sites.</span><span class="sxs-lookup"><span data-stu-id="abf24-148">The user's preferred settings when consuming translated documents, emails, messages, and websites.</span></span><br><br><span data-ttu-id="abf24-149">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="abf24-149">Returned by default.</span></span> <span data-ttu-id="abf24-150">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="abf24-150">Not nullable.</span></span>                                       |

## <a name="json-representation"></a><span data-ttu-id="abf24-151">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="abf24-151">JSON representation</span></span>

<span data-ttu-id="abf24-152">A seguir está uma definição JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="abf24-152">The following is a JSON definition of the resource.</span></span>

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
    "regionalFormatOverrides": {"@odata.type":"microsoft.graph.regionalFormatOverrides"},
    "translationPreferences":{"@odata.type":"microsoft.graph.translationPreferences"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


