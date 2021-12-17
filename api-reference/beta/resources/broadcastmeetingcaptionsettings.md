---
title: Tipo de recurso broadcastMeetingCaptionSettings
description: Representa as configurações de legenda de um evento Microsoft Teams ao vivo.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: resourcePageType
ms.openlocfilehash: 52239562480eed674b5b41000d9d3bedb7abfc54
ms.sourcegitcommit: 1a607ea5bee096944e0fea14167d372f1ff652f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/16/2021
ms.locfileid: "61547659"
---
# <a name="broadcastmeetingcaptionsettings-resource-type"></a>Tipo de recurso broadcastMeetingCaptionSettings

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as configurações de legenda de um evento Microsoft Teams [ao vivo](/microsoftteams/teams-live-events/what-are-teams-live-events). Para obter detalhes sobre como usar legendas ao vivo no cliente Teams, consulte [Usar legendas](https://support.microsoft.com/en-us/office/use-live-captions-in-a-live-event-1d6778d4-6c65-4189-ab13-e2d77beb9e2a)ao vivo em um evento ao vivo .

## <a name="properties"></a>Propriedades

| Propriedade             | Tipo              | Descrição                                                     |
|:---------------------|:------------------|:----------------------------------------------------------------|
| isCaptionEnabled     | Booliano           | Indica se a legenda está habilitada para esse evento Teams ao vivo. |
| spokenLanguage       | Cadeia de caracteres            | O idioma falado.                                            |
| translationLanguages | Coleção de cadeias de caracteres | Os idiomas de tradução (escolha até 6).                     |

> [!TIP]
>
> Os idiomas de tradução não podem conter o mesmo código de idioma que o idioma falado.

### <a name="spokenlanguage-values"></a>valores spokenLanguage

A tabela a seguir mostra os códigos de idioma com suporte para idiomas falados.

| Idioma falado           | Valor   |
|:--------------------------|:--------|
| Chinês (Simplificado, PRC) | zh-Hans |
| Holandês (Holanda)       | nl      |
| Inglês (Estados Unidos)   | en      |
| Francês (Canadá)           | fr-ca   |
| Francês (França)           | fr      |
| Alemão (Alemanha)          | de      |
| Hindi (Índia)             | Oi      |
| Italiano (Itália)           | it      |
| Japonês (Japão)          | ja      |
| Coreano (Coreia)            | ko      |
| Português (Brasil)       | pt      |
| Russo (Rússia)          | ru      |
| Espanhol (Espanha)           | es      |
| Espanhol (México)          | es-mx   |
| Sueco (Suécia)          | sv      |

### <a name="translationlanguaes-values"></a>valores translationLanguaes

A tabela a seguir mostra os códigos de idioma com suporte para idiomas de tradução.

| Idioma de tradução                     | Valor   |
|------------------------------------------|---------|
| Afrikaans (África do Sul)                 | af      |
| Árabe (Egito)                           | ar      |
| Bósnio (latino)                          | bs      |
| Búlgaro (Bulgária)                     | bg      |
| Catalão                                  | ca      |
| Chinês (Simplificado, PRC)                | zh-Hans |
| Chinês (Tranditional, Hong Kong S.A.R.) | yue     |
| Chinês (Tranditional)                   | zh-Hant |
| Crioulo (Haiti)                           | ht      |
| Croata (Croácia)                       | hr      |
| Tcheco (República Tcheca)                   | cs      |
| Dinamarquês (Dinamarca)                         | da      |
| Holandês (Holanda)                      | nl      |
| Inglês (Estados Unidos)                  | en      |
| Estoniano (Estônia)                       | et      |
| Filipino (Filipinas)                   | fil     |
| Finlandês (Finlândia)                        | fi      |
| Francês (Canadá)                          | fr-ca   |
| Francês (França)                          | fr      |
| Alemão (Alemanha)                         | de      |
| Grego (Grécia)                           | el      |
| Hebraico (Israel)                          | he      |
| Hindi (Índia)                            | Oi      |
| Hmong                                    | mww     |
| Húngaro (Hungria)                      | hu      |
| Indonésio                               | id      |
| Italiano (Itália)                          | it      |
| Japonês (Japão)                         | ja      |
| Klingon                                  | tlh     |
| Coreano (Coreia)                           | ko      |
| Letão (Letônia)                         | lv      |
| Lituano (Lituânia)                   | lt      |
| Malagasy (Madagáscar)                    | mg      |
| Malaio (Malásia)                         | ms      |
| Maltês (Malta)                          | mt      |
| Persa (Irã)                           | fa      |
| Polonês (Polônia)                          | pl      |
| Português (Brasil)                      | pt      |
| Querétaro Otomi                          | otq     |
| Romeno (Romênia)                       | ro      |
| Russo (Rússia)                         | ru      |
| Samoano                                   | sm      |
| Sérvio (latino)                          | sr-latn |
| Serbian Cyrillic                         | sr-cyrl |
| Eslovaco (Eslováquia)                        | sk      |
| Esloveno                                | sl      |
| Espanhol (Espanha)                          | es      |
| Swahili (Quênia)                          | sw      |
| Sueco (Suécia)                         | sv      |
| Taitiano                                 | ty      |
| Tailandês (Tailândia)                          | th      |
| Tongan                                   | para      |
| Turco (Turquia)                         | tr      |
| Ucraniano (Ucrânia)                      | uk      |
| Urdu (República Islâmica do Paquistão)      | your      |
| Vietnamita (Vietnã)                     | vi      |
| Galês (Reino Unido)                   | cy      |
| Yucatec Maya                             | yua     |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.broadcastMeetingCaptionSettings"
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.broadcastMeetingCaptionSettings",
  "isCaptionEnabled": "Boolean",
  "spokenLanguage": "String",
  "translationLanguages": [
    "String"
  ]
}
```
