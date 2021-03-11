---
title: Tipo de recurso regionalAndLanguageSettings
description: Um recurso que representa as preferências regionais e de idioma dos usuários
localization_priority: Normal
author: jasonbro
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 25af8de5a93bc67ed774b161ec63c1698434efb2
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721310"
---
# <a name="regionalandlanguagesettings-resource-type"></a>Tipo de recurso regionalAndLanguageSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Um tipo aberto que representa as preferências de um usuário para idiomas em vários contextos e para a localidade regional e a formatação que conduz o calendário padrão e a formatação para data e hora.

## <a name="methods"></a>Métodos

| Método                                                 | Tipo de retorno                                                   | Descrição                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [Get](../api/regionalAndLanguageSettings-get.md)       | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | Ler propriedades de **um objeto regionalAndLanguageSettings.**                                       |
| [Update](../api/regionalandlanguagesettings-update.md) | [regionalAndLanguageSettings](regionalAndLanguageSettings.md) | Atualize todo ou um subconjunto das propriedades do **objeto regionalAndLanguageSettings** para um usuário. |

## <a name="properties"></a>Propriedades
| Propriedade                   | Tipo                                                  | Descrição                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| defaultDisplayLanguage     | [localeInfo](localeinfo.md)                           | Idioma de interface do usuário preferencial do usuário (menus, botões, faixas de opções, mensagens de aviso) para aplicativos Web da Microsoft.<br><br>Retornado por padrão. Não anulável. |
| authoringLanguages         | Coleção [localeInfo](localeinfo.md)                                 | Lista priorizada de idiomas em que o usuário lê e os autores.<br><br>Retornado por padrão. Não anulável.                                                              |
| defaultTranslationLanguage | [localeInfo](localeinfo.md)                 | O idioma em que um usuário espera ter documentos, emails e mensagens convertidos.<br><br>Retornado por padrão.                                                    |
| defaultSpeechInputLanguage | [localeInfo](localeinfo.md)                 | O idioma que um usuário espera usar como entrada para cenários de texto em fala.<br><br>Retornado por padrão.                                                              |
| defaultRegionalFormat      | [localeInfo](localeinfo.md)            | A localidade que conduz a formatação padrão de data, hora e calendário.<br><br>Retornado por padrão.                                                                 |
| regionalFormatOverrides    | [regionalFormatOverrides](regionalformatoverrides.md) | Permite que um usuário substitua seu defaultRegionalFormat por formatos específicos de campo.<br><br>Retornado por padrão.                                                      |
| translationPreferences     | [translationPreferences](translationPreferences.md)   | As configurações preferidas do usuário ao consumir documentos convertidos, emails, mensagens e sites.<br><br>Retornado por padrão. Não anulável.                                       |

## <a name="json-representation"></a>Representação JSON

A seguir está uma definição JSON do recurso.

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


