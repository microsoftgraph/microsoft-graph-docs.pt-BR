---
title: Práticas recomendadas para trabalhar com a API do OneNote
description: Descubra recomendações para trabalhar com a API do OneNote no Microsoft Graph com base em respostas para perguntas comuns sobre o Microsoft Q&A e o Twitter.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 8d67f5ca0a6f21fc9fb4fab01534634f52e15cef
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66442833"
---
# <a name="best-practices-for-working-with-the-onenote-api-in-microsoft-graph"></a>Práticas recomendadas para trabalhar com a API do OneNote no Microsoft Graph

Este artigo fornece recomendações para trabalhar com APIs do OneNote no Microsoft Graph. Essas recomendações se baseiam em respostas a perguntas comuns sobre [o Microsoft Q&A](/answers/topics/microsoft-graph-notes.html)  e o Twitter.

## <a name="use-select-to-select-the-minimum-set-of-properties-you-need"></a>Use $select para selecionar o conjunto mínimo de propriedades de que você precisa

Quando você consulta um recurso (por exemplo, seções em um bloco de anotações), faz uma solicitação semelhante à seguinte.

```http
GET ~/notebooks/{id}/sections
```

Isso recupera todas as propriedades das seções. No entanto, você pode não precisar de todas as propriedades. Você pode usar o parâmetro de consulta `$select` para retornar apenas as propriedades desejadas, conforme mostrado no exemplo a seguir.

```http
GET ~/notebooks/{id}/sections?$select=id,displayName
```

A mesma abordagem se aplica a outras APIs do OneNote.

## <a name="use-expand-instead-of-making-multiple-api-calls"></a>Use $expand em vez de várias chamadas à API

Suponha que você queira recuperar todos os blocos de anotações, seções e grupos de seções do usuário em uma exibição hierárquica. Você pode fazer isso seguindo este procedimento:

* Chamar `GET ~/notebooks` para obter a lista de blocos de anotações.

* Para cada bloco de anotações recuperado, chame `GET ~/notebooks/{notebookId}/sections` para recuperar a lista de seções.

* Para cada bloco de anotações recuperado, chame `GET ~/notebooks/{notebookId}/sectionGroups` para recuperar a lista de grupos de seções.

* Opcionalmente, iterar de forma repetida em grupos de seções.

Embora isso funcione (com algumas viagens de ida e volta sequenciais extra ao serviço), uma abordagem melhor é usar o parâmetro de consulta `$expand`. 

```http
GET ~/notebooks?$expand=sections,sectionGroups($expand=sections)
```

Isso produzirá os mesmos resultados de ida e volta na rede, com melhor desempenho.

## <a name="when-getting-all-pages-for-a-user-do-so-for-each-section-separately"></a>Ao obter todas as páginas de um usuário, faça isso para cada seção separadamente

Embora o Microsoft Graph exponha um ponto de extremidade para recuperar todas as páginas, essa não é a melhor maneira de obter todas as páginas às quais o usuário tem acesso. Quando o usuário tem muitas seções, isso pode causar tempos limite ou mau desempenho. É melhor iterar cada seção, obtendo páginas para cada uma separadamente.

Por exemplo, em vez de usar essa chamada (essa API é paginada; portanto, você não poderá buscar todas as páginas de uma só vez):

```http
GET ~/pages
```

É melhor usar a seguinte chamada várias vezes (especialmente se você não precisar de todas as seções):

```http
GET ~/sections/{id}/pages
```

Ao obter metadados de página, substitua a ordenação padrão `lastModifiedDateTime`. É mais rápido acessar páginas quando não é preciso classificá-las por `lastModifiedDateTime`. Para fazer isso, você pode classificar por qualquer outra propriedade; por exemplo:

```http
GET ~/sections/{id}/pages?$select=id,title,createdDateTime&$orderby=createdDateTime
```
