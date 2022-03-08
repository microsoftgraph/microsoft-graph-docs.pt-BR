---
title: Use a API Pesquisa da Microsoft para gerenciar respostas administrativas
description: Use o Microsoft Graph para gerenciar respostas de pesquisa administrativa na experiência de Pesquisa da Microsoft.
ms.localizationpriority: high
author: jakeost-msft
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 4e3204594dde96fc5c51b1f27337ad3e84125fb8
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63338117"
---
# <a name="use-the-microsoft-search-api-to-manage-administrative-answers"></a>Use a API Pesquisa da Microsoft para gerenciar respostas administrativas

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Você pode usar o Microsoft Graph para gerenciar resultados de resposta de pesquisa administrativa na experiência [Pesquisa da Microsoft](/microsoftsearch/overview-microsoft-search).

As solicitações para gerenciar as respostas da pesquisa administrativa são executadas por administradores globais, administradores de pesquisa, editores de pesquisa, ou são executadas em nome de um aplicativo sem a presença de um usuário conectado, identificado usando um [token de acesso com permissão do aplicativo](/graph/auth-v2-service).

## <a name="common-use-cases"></a>Casos de uso comuns

Os casos de uso das APIs nesta seção envolvem o gerenciamento de respostas administrativas, como acrônimos, indicadores e QnAs de uma organização.

| Casos de uso                                        | Recursos REST                              |
|:-------------------------------------------------|:--------------------------------------------|
| **Ações de resposta de pesquisa**                        |                                             |
| Criar, atualizar ou excluir uma resposta de pesquisa        | [acrônimo](search-acronym.md), [indicador](search-bookmark.md), [qna](search-qna.md) |

## <a name="supported-language-tags"></a>Rótulos do idioma com suporte
Uma marca de idioma de um [indicador](search-bookmark.md) ou [ qna](search-qna.md) representa um idioma geograficamente específico no qual essa resposta de pesquisa (**indicador** ou **qna**) pode ser exibida. Uma marca de idioma segue o padrão {language}-{REGION}. Para obter mais informações sobre o padrão, consulte [RFC 4646](https://datatracker.ietf.org/doc/html/rfc4646).

A tabela a seguir lista as marcas de idioma, localidades e o país ou região correspondente que você pode definir no [Centro de administração do Microsoft 365](https://admin.microsoft.com/) para publicar uma resposta de pesquisa. A coluna **Localidade** descreve o idioma usado nesse país ou região.

| Marca de idioma com suporte | Locale | Escolha do país ou região no Centro de administração do Microsoft 365  |
| ----------- | ----------  | ----------  |
|`es-AR`| Espanhol (Argentina) | Argentina | 
|`en-AU`| Inglês (Austrália) | Austrália |
|`de-AT`| Alemão (Áustria) |Áustria | 
|`fr-BE`| Francês (Bélgica) |Bélgica – francês | 
|`nl-BE`| Holandês (Bélgica) | Bélgica – holandês | 
|`en-CA`| Inglês (Canadá) | Canadá - inglês | 
|`fr-CA`| Francês (Canadá) | Canadá - francês | 
|`fr-FR`| Francês (França) | França | 
|`de-DE`| Alemão (Alemanha) | Alemanha | 
|`zh-HK`| Chinês (Hong Kong) | Hong-Kong |
|`en-IN`| Inglês (Índia) | Índia |
|`it-IT`| Italiano (Itália) | Itália |
|`pt-BR`| Português (Brasil) | Brasil |
|`en-ID`| Inglês (Indonésia) | Indonésia |
|`ja-JP`| Japonês (Japão) | Japão |
|`ko-KR`| Coreano (Coréia do Sul) | Coreia |
|`en-MY`| Inglês (Malásia) | Malásia |
|`es-MX`| Espanhol (México) | México |
|`nl-NL`| Holandês (Países Baixos) | Países Baixos |
|`nb-NO`| Norueguês Bokmål (Noruega) | Noruega |
|`zh-CN`| Chinês (China) | República Popular da China |
|`pl-PL`| Polonês (Polônia) | Polônia |
|`ru-RU`| Russo (Rússia) | Rússia |
|`ar-SA`| Arábico (Arábia Saudita) | Arábia Saudita |
|`sv-SE`| Sueco (Suécia) | Suécia |
|`es-ES`| Espanhol (Espanha) | Espanha |
|`fr-CH`| Francês (Suíça) | Suíça – francês |
|`de-CH`| Alemão (Suíça) | Suíça – alemão |
|`en-ZA`| Inglês (África do Sul) | África do Sul |
|`zh-TW`| Chinês (Taiwan) | Taiwan |
|`tr-TR`| Turco (Turquia) | Turquia |
|`en-GB`| Inglês (Reino Unido) | Reino Unido |
|`en-US`| Inglês (Estados Unidos) | Estados Unidos - inglês |
|`es-US`| Espanhol (Estados Unidos) | Estados Unidos - espanhol |

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.

## <a name="next-steps"></a>Próximas etapas

- Confira a [Visão geral da API de Pesquisa da Microsoft](/graph/search-concept-overview).
- Faça uma análise dos métodos, propriedades e relações dos recursos do tipo de resposta: [indicadores](search-bookmark.md), [acrônimos](search-acronym.md) e [QnAs](search-qna.md).

