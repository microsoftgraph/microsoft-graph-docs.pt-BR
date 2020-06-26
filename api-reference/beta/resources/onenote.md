---
title: tipo de recurso do onenote
description: O ponto de entrada para os recursos do OneNote.
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: e213f12110399b90513d33af4d1745be3cdf3eae
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44898062"
---
# <a name="onenote-resource-type"></a>tipo de recurso do onenote

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

O ponto de entrada para os recursos do OneNote.

Todas as chamadas para o serviço do OneNote pela API do Microsoft Graph usam essa URL raiz de serviço:

```
https://graph.microsoft.com/{version}/{location}/onenote/ 
```

O local pode ser blocos de anotações do usuário no Microsoft 365 ou no OneDrive do consumidor, nos blocos de anotações de grupo ou em blocos de anotações de equipe hospedados no site do SharePoint no Microsoft 365. 

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
|notebooks|Coleção [bloco de anotações](notebook.md)|A coleção de blocos de anotações do OneNote que pertencem ao usuário ou ao grupo. Somente leitura. Anulável.|
|operations|coleção [onenoteOperation](onenoteoperation.md) |O status das operações do OneNote. Não há suporte para a obtenção de uma coleção de operações, mas você pode obter o status das operações longas se o cabeçalho `Operation-Location` for retornado na resposta. Somente leitura. Anulável.|
|páginas|coleção [onenotePage](onenotepage.md)|As páginas em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|
|recursos|coleção [onenoteResource](onenoteresource.md) |A imagem e outros recursos de arquivos nas páginas do OneNote. Não há suporte para a obtenção de uma coleção de recursos, mas você pode [obter o conteúdo de um recurso binário específico](onenoteresource.md). Somente leitura. Anulável.|
|sectionGroups|coleção de [seções](sectiongroup.md)|Os grupos de seção em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|
|seções|coleção [onenoteSection](onenotesection.md)|As seções em todos os blocos de anotações do OneNote que pertencem ao usuário ou ao grupo.  Somente leitura. Anulável.|

## <a name="methods"></a>Métodos

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Create notebook](../api/onenote-post-notebooks.md) |[bloco de anotações](notebook.md)| Crie um bloco de anotações postando na coleção notebooks.|
|[List notebooks](../api/onenote-list-notebooks.md) |Coleção [bloco de anotações](notebook.md)| Obter uma coleção de blocos de anotações.|
|[Create page](../api/onenote-post-pages.md) |[onenotePage](onenotepage.md) | Crie uma página postando na coleção pages.|
|[List pages](../api/onenote-list-pages.md) |coleção [onenotePage](onenotepage.md)| Obter uma coleção de páginas.|
|[List section groups](../api/onenote-list-sectiongroups.md) |coleção de [seções](sectiongroup.md)| Obter uma coleção de grupos de seção.|
|[Listar seções](../api/onenote-list-sections.md) |coleção [onenoteSection](onenotesection.md)| Obter uma coleção de seções.|
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.onenote"
}-->
``` json
{
  "notebooks": [{ "@odata.type": "microsoft.graph.notebook" }],
  "operations": [{ "@odata.type": "microsoft.graph.onenoteOperation" }],
  "pages": [{ "@odata.type": "microsoft.graph.onenotePage" }],
  "resources": [ { "@odata.type": "microsoft.graph.onenoteResource" } ],
  "sectionGroups": [ { "@odata.type": "microsoft.graph.sectionGroup" } ],
  "sections": [ { "@odata.type": "microsoft.graph.onenoteSection" } ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "onenote resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
