---
title: Sincronização de pausa em um educationSynchronizationProfile
description: Pause a sincronização de um perfil de sincronização de dados escola específico no inquilino.
author: mmast-msft
ms.openlocfilehash: 14e94cf4a083e8f37b03f96b287a75aa40b7afed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27313283"
---
# <a name="pause-sync-on-an-educationsynchronizationprofile"></a>Sincronização de pausa em um educationSynchronizationProfile

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Pause a sincronização de um de dados específicos escola [perfil de sincronização](../resources/educationsynchronizationprofile.md) no inquilino.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão | Permissões |
|:-----------|:----------|
| Delegado (conta corporativa ou de estudante) | EduAdministration.ReadWrite |
|Delegada (conta pessoal da Microsoft|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /synchronizationProfiles/{id}/pause
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório.  |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.
## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta `200 OK`.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.
<!-- {
  "blockType": "request",
  "name": "post_synchronizationProfile_pause"
}-->
```http
POST https://graph.microsoft.com/beta/education/synchronizationProfiles/{id}/pause
```

##### <a name="response"></a>Resposta

Não há nenhum corpo de resposta.

<!-- {
  "blockType": "response",
  "name": "post_synchronizationProfile_pause"
}-->
```
HTTP/1.1 200 OK
```