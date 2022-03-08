---
title: Configurar respostas administrativas de pesquisa para usuários em uma organização (visualização)
description: Pesquisa da Microsoft permite que os administradores associem termos de pesquisa a significados ou páginas da Web específicas de suas organizações e incluam essas associações como respostas de pesquisa.
author: jakeost-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: conceptualPageType
ms.openlocfilehash: 542f1c3dc3d280ba72c3c64d032c19594c6bc29c
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63337885"
---
# <a name="set-up-administrative-search-answers-for-users-in-an-organization-preview"></a>Configurar respostas administrativas de pesquisa para usuários em uma organização (visualização)

Pesquisa da Microsoft permite que os administradores associem termos de pesquisa a significados ou páginas da Web específicas de suas organizações e incluam essas associações como respostas de pesquisa. Por exemplo, os usuários em uma organização podem executar em um acrônimo desconhecido que representa um nome de projeto interno ou um nome de equipe associado a uma página da Web de equipe. Os administradores podem configurar acrônimos, [indicadores](/microsoftsearch/manage-bookmarks) ou [QnA](/microsoftsearch/manage-qas) no [Centro de administração do Microsoft 365, em](https://admin.microsoft.com/) **Search & intelligence**.[](/microsoftsearch/manage-acronyms) Isso permite que os usuários usem a pesquisa para navegar e se familiarizar com seu trabalho.

Os administradores também podem usar a API de pesquisa na Microsoft Graph gerenciar programaticamente respostas de pesquisa administrativas na organização. Essas respostas são exibidas em Pesquisa da Microsoft resultados quando disparados por um acrônimo ou palavra-chave definido nos tipos de recursos de resposta de [pesquisa disponíveis:](/graph/api/resources/search-acronym) acrônimo[, indicador](/graph/api/resources/search-bookmark) e [recursos QnA](/graph/api/resources/search-qna).

Quando disparadas por um acrônimo ou palavra-chave definido, essas respostas de pesquisa aparecerão na parte superior da página de resultados da pesquisa em sua organização.

## <a name="example-create-a-new-acronym"></a>Exemplo: Criar um novo acrônimo

A solicitação a seguir cria um novo acrônimo que será exibido na página de resultados da pesquisa quando um usuário pesquisa por ele.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_acronym_from_acronyms"
}-->
```http
POST https://graph.microsoft.com/beta/search/acronyms
Content-Type: application/json

{
  "displayName": "GDPR",
  "standsFor": "General Data Protection Regulation",
  "description": "A European Union (EU) regulation on data protection and privacy in the EU and the European Economic Area (EEA) that enhances individuals' control and rights over their personal data, simplifies the regulatory environment for international business, and addresses the transfer of personal data outside the EU and EEA areas.",
  "webUrl": "http://contoso.com/GDPR",
  "state": "published"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.acronym"
}-->
```http
HTTP/1.1 200 Ok
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

## <a name="example-create-a-new-bookmark"></a>Exemplo: Criar um novo indicador

A solicitação a seguir cria um novo indicador que será exibido na página de resultados da pesquisa quando um usuário procurar pelo menos uma de suas palavras-chave.

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_bookmark_from_bookmarks"
}-->
```http
POST https://graph.microsoft.com/beta/search/bookmarks
Content-Type: application/json

{
  "displayName": "Contoso Install Site",
  "webUrl": "http://www.contoso.com/",
  "description": "Try or buy Contoso for Home or Business and view product information",
  "keywords":  {
    "keywords": ["Contoso", "install"],
    "reservedKeywords": ["Contoso"],
    "matchSimilarKeywords": true
  },
  "state": "published"
}
```

### <a name="response"></a>Resposta
Veja a seguir um exemplo da resposta.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.search.bookmark"
}-->
```http
HTTP/1.1 201 CREATED
Location: /733b26d5-af76-4eea-ac69-1a0ce8716897
Content-Type: application/json

{
  "id": "733b26d5-af76-4eea-ac69-1a0ce8716897"
}
```

## <a name="next-steps"></a>Próximas etapas
- Familiarizar-se com os cenários e recursos da API de Pesquisa: [Pesquisa da Microsoft visão geral da API](/graph/search-concept-overview).
- Explore as APIs no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer).
- [Gerenciar respostas administrativas de pesquisa](search-concept-answers.md).
