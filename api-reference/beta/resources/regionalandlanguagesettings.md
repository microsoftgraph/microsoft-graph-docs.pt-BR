---
title: tipo de recurso regionalAndLanguageSettings
description: Um recurso que representa as preferências regionais e de idioma de um usuário
localization_priority: Normal
author: jasonbro
ms.prod: settings
doc_type: resourcePageType
ms.openlocfilehash: ba8666b78023b7345d936516fc3aec2b116520ad
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44845677"
---
# <a name="regionalandlanguagesettings-resource-type"></a><span data-ttu-id="8ea02-103">tipo de recurso regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="8ea02-103">regionalAndLanguageSettings resource type</span></span>

<span data-ttu-id="8ea02-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8ea02-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ea02-105">Um tipo aberto que representa as preferências de um usuário para idiomas em vários contextos e para a localidade e a formatação regionais que orientam o calendário padrão e a formatação de data e hora.</span><span class="sxs-lookup"><span data-stu-id="8ea02-105">An open type that represents a user's preferences for languages in various contexts, and for regional locale and formatting that drives the default calendar, and formatting for date and time.</span></span>

## <a name="methods"></a><span data-ttu-id="8ea02-106">Methods</span><span class="sxs-lookup"><span data-stu-id="8ea02-106">Methods</span></span>

| <span data-ttu-id="8ea02-107">Método</span><span class="sxs-lookup"><span data-stu-id="8ea02-107">Method</span></span>                                                 | <span data-ttu-id="8ea02-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8ea02-108">Return Type</span></span>                                                   | <span data-ttu-id="8ea02-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ea02-109">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="8ea02-110">Get</span><span class="sxs-lookup"><span data-stu-id="8ea02-110">Get</span></span>](../api/regionalAndLanguageSettings-get.md)       | [<span data-ttu-id="8ea02-111">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="8ea02-111">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="8ea02-112">Ler as propriedades de um objeto **regionalAndLanguageSettings** .</span><span class="sxs-lookup"><span data-stu-id="8ea02-112">Read properties of a **regionalAndLanguageSettings** object.</span></span>                                       |
| [<span data-ttu-id="8ea02-113">Atualização</span><span class="sxs-lookup"><span data-stu-id="8ea02-113">Update</span></span>](../api/regionalandlanguagesettings-update.md) | [<span data-ttu-id="8ea02-114">regionalAndLanguageSettings</span><span class="sxs-lookup"><span data-stu-id="8ea02-114">regionalAndLanguageSettings</span></span>](regionalAndLanguageSettings.md) | <span data-ttu-id="8ea02-115">Atualizar tudo ou um subconjunto das propriedades do objeto **regionalAndLanguageSettings** para um usuário.</span><span class="sxs-lookup"><span data-stu-id="8ea02-115">Update all or a subset of the properties of the **regionalAndLanguageSettings** object for a user.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ea02-116">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8ea02-116">Properties</span></span>
| <span data-ttu-id="8ea02-117">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8ea02-117">Property</span></span>                   | <span data-ttu-id="8ea02-118">Tipo</span><span class="sxs-lookup"><span data-stu-id="8ea02-118">Type</span></span>                                                  | <span data-ttu-id="8ea02-119">Descrição</span><span class="sxs-lookup"><span data-stu-id="8ea02-119">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="8ea02-120">defaultDisplayLanguage</span><span class="sxs-lookup"><span data-stu-id="8ea02-120">defaultDisplayLanguage</span></span>     | [<span data-ttu-id="8ea02-121">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ea02-121">localeInfo</span></span>](localeinfo.md)                           | <span data-ttu-id="8ea02-122">Idioma preferencial da interface de usuário do usuário (menus, botões, faixas de opções, mensagens de aviso) para aplicativos da Web da Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8ea02-122">The  user's preferred user interface language (menus, buttons, ribbons, warning messages) for Microsoft web applications.</span></span><br><br><span data-ttu-id="8ea02-123">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-123">Returned by default.</span></span> <span data-ttu-id="8ea02-124">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="8ea02-124">Not nullable.</span></span> |
| <span data-ttu-id="8ea02-125">authoringLanguages</span><span class="sxs-lookup"><span data-stu-id="8ea02-125">authoringLanguages</span></span>         | <span data-ttu-id="8ea02-126">Coleção localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ea02-126">localeInfo collection</span></span>                                 | <span data-ttu-id="8ea02-127">Lista priorizada de idiomas nos quais o usuário lê e autores.</span><span class="sxs-lookup"><span data-stu-id="8ea02-127">Prioritized list of languages the user reads and authors in.</span></span><br><br><span data-ttu-id="8ea02-128">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-128">Returned by default.</span></span> <span data-ttu-id="8ea02-129">Não anulável.</span><span class="sxs-lookup"><span data-stu-id="8ea02-129">Not nullable.</span></span>                                                              |
| <span data-ttu-id="8ea02-130">defaultTranslationLanguage</span><span class="sxs-lookup"><span data-stu-id="8ea02-130">defaultTranslationLanguage</span></span> | <span data-ttu-id="8ea02-131">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ea02-131">localeInfo</span></span>                                            | <span data-ttu-id="8ea02-132">O idioma que um usuário espera ter documentos, emails e mensagens traduzidos para o.</span><span class="sxs-lookup"><span data-stu-id="8ea02-132">The language a user expects to have documents, emails, and messages translated into.</span></span><br><br><span data-ttu-id="8ea02-133">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-133">Returned by default.</span></span>                                                    |
| <span data-ttu-id="8ea02-134">defaultSpeechInputLanguage</span><span class="sxs-lookup"><span data-stu-id="8ea02-134">defaultSpeechInputLanguage</span></span> | <span data-ttu-id="8ea02-135">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ea02-135">localeInfo</span></span>                                            | <span data-ttu-id="8ea02-136">O idioma que o usuário esperava usar como entrada para cenários de texto para fala.</span><span class="sxs-lookup"><span data-stu-id="8ea02-136">The language a user expected to use as input for text to speech scenarios.</span></span><br><br><span data-ttu-id="8ea02-137">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-137">Returned by default.</span></span>                                                              |
| <span data-ttu-id="8ea02-138">defaultRegionalFormat</span><span class="sxs-lookup"><span data-stu-id="8ea02-138">defaultRegionalFormat</span></span>      | <span data-ttu-id="8ea02-139">localeInfo</span><span class="sxs-lookup"><span data-stu-id="8ea02-139">localeInfo</span></span>                                            | <span data-ttu-id="8ea02-140">A localidade que orienta a data, a hora e a formatação de calendário padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-140">The locale that drives the default date, time, and calendar formatting.</span></span><br><br><span data-ttu-id="8ea02-141">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-141">Returned by default.</span></span>                                                                 |
| <span data-ttu-id="8ea02-142">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="8ea02-142">regionalFormatOverrides</span></span>    | [<span data-ttu-id="8ea02-143">regionalFormatOverrides</span><span class="sxs-lookup"><span data-stu-id="8ea02-143">regionalFormatOverrides</span></span>](regionalformatoverrides.md) | <span data-ttu-id="8ea02-144">Permite que um usuário substitua o defaultRegionalFormat por formatos específicos de campos.</span><span class="sxs-lookup"><span data-stu-id="8ea02-144">Allows a user to override their defaultRegionalFormat with field specific formats.</span></span><br><br><span data-ttu-id="8ea02-145">Retornado por padrão.</span><span class="sxs-lookup"><span data-stu-id="8ea02-145">Returned by default.</span></span>                                                      |

## <a name="json-representation"></a><span data-ttu-id="8ea02-146">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8ea02-146">JSON representation</span></span>

<span data-ttu-id="8ea02-147">A seguir está uma definição de JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8ea02-147">The following is a JSON definition of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.regionalAndLanguageSettings"
} -->

```json
{
    "defaultDisplayLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "authoringLanguages":[{"@odata.type":"microsoft.graph.localeInfo"}] ,
    "defaultTranslationLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultSpeechInputLanguage": {"@odata.type":"microsoft.graph.localeInfo"},
    "defaultRegionalFormat":{"@odata.type":"microsoft.graph.localeInfo"} ,
    "regionalFormatOverrides":{"@odata.type":"microsoft.graph.regionalFormatOverrides"}
}
```
<!-- {
  "type": "#page.annotation",
  "description": "regionalAndLanguageSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
