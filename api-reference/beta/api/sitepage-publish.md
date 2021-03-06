---
author: rahmit
description: Publicar a versão mais recente de um recurso sitePage, que torna a versão da página disponível para todos os usuários. Se a página estiver com check-out, faça check-in na página e publique-a. Se a página estiver com check-out para o chamador desta API, a página será automaticamente verificada e publicada.
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: e40f864ce224916a2c60e5c82e0aecbfff213fbc
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48044375"
---
# <a name="sitepage-publish"></a>sitePage: publish

Namespace: microsoft.graph

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
  "suppressions": []
}
-->


