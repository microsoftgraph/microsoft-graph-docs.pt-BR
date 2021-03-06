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
# <a name="translationpreferences-resource-type"></a>Tipo de recurso translationPreferences

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma entrada na lista de substituição de idioma de tradução de um usuário.

## <a name="properties"></a>Propriedades

|Propriedade             |Tipo                                         |Descrição                                                            |
|---------------------|-------------------------------------------------------------|-----------------------------------------------------------------------|
|translationBehavior  |[translationBehavior](#translationbehavior-values)       |O comportamento de conversão preferencial do usuário.<br><br>Retornado por padrão. Não anulável. |                   
|languageOverrides    |[Coleção translationLanguageOverride](translationLanguageOverride.md)                | Comportamento de substituição de conversão para idiomas, se for o caso.<br><br>Retornado por padrão.|
|untranslatedLanguages|Conjunto de cadeias de caracteres| A lista de idiomas que o usuário não precisa traduzir. Isso é calculado da coleção **authoringLanguages** [em regionalAndLanguageSettings](regionalandlanguagesettings.md)e da coleção **languageOverrides** em **translationPreferences**. A lista especifica valores de cultura neutros que incluem o código de idioma sem qualquer associação de país ou região. Por exemplo, ele especificaria "fr" para a cultura francesa neutra, mas não "fr-FR" para a cultura francesa na França. <br><br>Retornado por padrão. Somente leitura.| 

### <a name="translationbehavior-values"></a>valores translationBehavior

|Member |Descrição                                                                  |
|-------|-----------------------------------------------------------------------------|
|Pergunte    |Solicitar ao usuário antes de traduzir as mensagens/chats/páginas da Web para o usuário.|
|Sim    |Traduza automaticamente as mensagens/chats/páginas da Web para o usuário.           |
|Não     |Não ofereça tradução automática ou solicitada para o usuário.                 |



## <a name="json-representation"></a>Representação JSON

A seguir está uma definição JSON do recurso.

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


