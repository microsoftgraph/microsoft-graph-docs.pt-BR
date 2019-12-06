---
title: Usar a API do Microsoft Graph para integrar a pesquisa de dados relevantes sobre pessoas em um aplicativo
description: O Microsoft Graph permite o acesso a dados úteis sobre pessoas e documentos com os quais eles interagem.
author: simonhult
localization_priority: Priority
ms.prod: insights
doc_type: conceptualPageType
ms.openlocfilehash: 43d2c00e9651c6bbf73e82102a36eb25efd94215
ms.sourcegitcommit: 1cdb3bcddf34e7445e65477b9bf661d4d10c7311
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/05/2019
ms.locfileid: "39845032"
---
# <a name="use-the-microsoft-graph-api-to-integrate-people-intelligence-in-an-app"></a>Usar a API do Microsoft Graph para integrar a pesquisa de dados relevantes sobre pessoas em um aplicativo

O Microsoft Graph permite o acesso a dados úteis sobre pessoas e documentos com os quais eles interagem.

## <a name="aggregate-and-extract-specific-information-about-people"></a>Agregar e extraia informações específicas sobre pessoas

Recurso: Pessoas

Você pode usar o recurso [pessoa](../resources/person.md) e a API de Pessoas para agregar informações sobre uma pessoa provenientes de emails, contatos e redes sociais. Os resultados são ordenados por relevância com base em vários padrões de comunicação e colaboração e em relações comerciais. A API permite navegar, classificar, selecionar, filtrar ou procurar pessoas com base em critérios selecionados.

Para ver cenários e exemplos, confira [Obter informações sobre pessoas relevantes](/graph/people-example).

Para usar a API, confira o seguinte:

- [Listar pessoas](../api/user-list-people.md)


## <a name="help-users-get-the-most-relevant-documents-for-their-work"></a>Ajudar os usuários a obter os documentos mais relevantes para seu trabalho

Recurso: Ideias do documento

Usar a API insights para identificar os documentos mais relevantes para o usuário:

- Listar documentos [mais populares](../api/insights-list-trending.md) de um usuário
- Listar documentos [usados por](../api/insights-list-used.md) um usuário
- Listar documentos [compartilhados com ou por](../api/insights-list-shared.md) um usuário
