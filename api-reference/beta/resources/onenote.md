---
title: tipo de recurso do OneNote
description: O ponto de entrada para recursos do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 5ed063fb485acdbd029a977ffb6cd721bf7085c8
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32561646"
---
# <a name="onenote-resource-type"></a>tipo de recurso do OneNote

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O ponto de entrada para recursos do OneNote.

Todas as chamadas para o serviço do OneNote por meio da API do Microsoft Graph usam esta URL raiz do serviço:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

O local pode ser blocos de anotações do usuário no Office 365 ou no OneDrive do consumidor, nos blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Office 365. 

**Blocos de anotações do usuário** Para acessar blocos de anotações pessoais no OneDrive do consumidor ou no OneDrive for Business, use uma das seguintes URLs:

```
https://graph.microsoft.com/{version}/me/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{userPrincipalName}/onenote/{notebooks | sections | sectionGroups | pages} 
https://graph.microsoft.com/{version}/users/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

**Blocos de anotações de grupo** Para acessar blocos de anotações pertencentes a um grupo, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/groups/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```
**Blocos de anotações do site do SharePoint** Para acessar blocos de anotações pertencentes a um site de equipe do SharePoint, use a seguinte URL raiz de serviço:

```
https://graph.microsoft.com/{version}/sites/{id}/onenote/{notebooks | sections | sectionGroups | pages} 
```

## <a name="authorization"></a>Autorização

Para obter informações sobre as permissões necessárias para trabalhar com as APIs do OneNote, consulte [observações sobre permissões](/graph/permissions-reference#notes-permissions).

## <a name="relationships"></a>Relações
| Relação | Tipo   |Descrição|
|:---------------|:--------|:----------|
|notebooks|Coleção [Notebook](notebook.md)|O conjunto de blocos de anotações do OneNote pertencentes ao usuário ou grupo. Somente leitura. Anulável.|
|operations|Coleção [Operation](onenoteoperation.md) |O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status de operações de `Operation-Location` longa duração se o cabeçalho for retornado na resposta. Somente leitura. Anulável.|
|páginas|Coleção [Page](page.md)|As páginas de todos os blocos de anotações do OneNote pertencentes ao usuário ou grupo.  Somente leitura. Anulável.|
|recursos|Coleção de [recursos](resource.md) |A imagem e outros recursos de arquivo nas páginas do OneNote. Não há suporte para a obtenção de uma coleção Resources, mas você pode [obter o conteúdo binário de um recurso específico](resource.md). Somente leitura. Anulável.|
|sectionGroups|Coleção de [seções](sectiongroup.md)|Os grupos de seções de todos os blocos de anotações do OneNote pertencentes ao usuário ou grupo.  Somente leitura. Anulável.|
|sections|Coleção [Section](section.md)|As seções de todos os blocos de anotações do OneNote pertencentes ao usuário ou grupo.  Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Criar blocos de anotações](../api/onenote-post-notebooks.md) |[Bloco de anotações](notebook.md)| Crie um bloco de anotações postando na coleção de blocos de anotações.|
|[Listar blocos de anotações](../api/onenote-list-notebooks.md) |Coleção [Notebook](notebook.md)| Obter uma coleção de blocos de anotações.|
|[Criar página](../api/onenote-post-pages.md) |[Page](page.md)| Crie uma página postando na coleção Pages.|
|[Listar páginas](../api/onenote-list-pages.md) |Coleção [Page](page.md)| Obter uma coleção de páginas.|
|[Listar grupos de seções](../api/onenote-list-sectiongroups.md) |Coleção de [seções](sectiongroup.md)| Obter uma coleção de grupos de seções.|
|[Listar seções](../api/onenote-list-sections.md) |Coleção [Section](section.md)| Obter uma coleção de seções.|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/onenote.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
