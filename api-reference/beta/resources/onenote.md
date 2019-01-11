---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: Jewan-microsoft
localization_priority: Normal
ms.openlocfilehash: 7f282147912f5d73d2aa1655055a763c0cec3764
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878012"
---
# <a name="onenote-resource-type"></a>tipo de recurso do onenote

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O ponto de entrada para os recursos do OneNote.

Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

O local pode ser blocos de anotações do usuário no Office 365 ou consumidor OneDrive, blocos de anotações do grupo ou blocos de anotações do SharePoint team site hospedado no Office 365. 

**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Blocos de anotações de grupo** para acessar blocos de anotações que pertencem a um grupo, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**Blocos de anotações do site do SharePoint** para acessar blocos de anotações que pertencem a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>Autorização

Para obter informações sobre as permissões necessárias para trabalhar com o APIs do OneNote, confira [Permissões de anotações](/graph/permissions-reference#notes-permissions).

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notebooks|Coleção [Notebook](notebook.md)|A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.|
|operations|Coleção [Operation](onenoteoperation.md) |O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.|
|páginas|Coleção [Page](page.md)|As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|
|recursos|Coleção [Resource](resource.md) |A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](resource.md). Somente leitura. Anulável.|
|sectionGroups|Coleção [SectionGroup](sectiongroup.md)|Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|
|sections|Coleção [Section](section.md)|As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Create notebook](../api/onenote-post-notebooks.md) |[Notebook](notebook.md)| Crie um bloco de anotações postando na coleção notebooks.|
|[List notebooks](../api/onenote-list-notebooks.md) |Coleção [Notebook](notebook.md)| Obter uma coleção de blocos de anotações.|
|[Create page](../api/onenote-post-pages.md) |[Page](page.md)| Crie uma página postando na coleção pages.|
|[List pages](../api/onenote-list-pages.md) |Coleção [Page](page.md)| Obter uma coleção de páginas.|
|[List section groups](../api/onenote-list-sectiongroups.md) |Coleção [SectionGroup](sectiongroup.md)| Obter uma coleção de grupos de seção.|
|[List sections](../api/onenote-list-sections.md) |Coleção [Section](section.md)| Obter uma coleção de seções.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
