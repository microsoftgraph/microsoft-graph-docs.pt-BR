---
author: rahmit
ms.author: rahmit
ms.date: 09/10/2018
title: Publicar página
localization_priority: Normal
ms.openlocfilehash: 0b98f22dda2c4b08d04150b8b24126fdff5ca505
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27836152"
---
# <a name="sitepage-publish"></a>sitePage: publicar

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Publique a versão mais recente de um recurso de [sitePage][] , o que disponibiliza a versão da página para todos os usuários. Se a página está com check-out, check-in de página e publicá-lo. Se a página é verificada com o chamador desta API, a página é automaticamente check-in e, em seguida, publicada.

[sitePage]: ../resources/sitepage.md

## <a name="permissions"></a>Permissions

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

Esta mensagem não tem um corpo da solicitação. Qualquer corpo da solicitação enviado será ignorado.

## <a name="response"></a>Resposta

Se tiver êxito, a chamada API retorna um código `204 No Content`.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 204 No Content
```


<!-- {
  "type": "#page.annotation",
  "description": "Publish a page.",
  "keywords": "publish page",
  "section": "documentation",
  "tocPath": "Pages/Publish"
} -->
