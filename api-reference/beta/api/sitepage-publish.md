---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 5a00a69542c2b59b1b268433b08656c87d194feb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32545213"
---
# <a name="sitepage-publish"></a>sitePage: publish

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Publicar a versão mais recente de um recurso [sitePage][] , que torna a versão da página disponível para todos os usuários. Se a página estiver com check-out, faça check-in na página e publique-a. Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a>Permissões

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Files.ReadWrite, Files.ReadWrite.All, Sites.ReadWrite.All    |
|Delegado (conta pessoal da Microsoft) | Files.ReadWrite, Files.ReadWrite.All    |
|Aplicativo | Files.ReadWrite.All, Sites.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
POST /sites/{siteId}/pages/{pageId}/publish
```

## <a name="request-body"></a>Corpo da solicitação

Esta mensagem não tem um corpo de solicitação. Qualquer corpo de solicitação enviado será ignorado.

## <a name="response"></a>Resposta

Se tiver êxito, a chamada API retorna um código `204 No Content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!--
{
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish",
  "suppressions": [
    "Error: /api-reference/beta/api/sitepage-publish.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
