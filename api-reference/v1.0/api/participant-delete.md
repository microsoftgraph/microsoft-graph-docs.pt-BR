---
title: Excluir participante
description: Exclua um participante específico na chamada.
manager: zhengni
author: jackry6350
ms.author: yoren
localization_priority: Normal
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 8c08821f723152adb82cde0255d21ea3d8718a8e
ms.sourcegitcommit: d12bd5435c198bcd096e1f7f6a2716f4a04631cc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/19/2020
ms.locfileid: "48137152"
---
# <a name="delete-participant"></a>Excluir participante

Excluir um participante específico em uma chamada. Em algumas situações, é apropriado que um aplicativo remova um participante de uma chamada ativa. Esta ação pode ser realizada antes ou depois de o participante responder a chamada. Quando um chamador ativo é removido, ele é imediatamente descartado da chamada sem notificação prévia ou após a remoção.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | Não suportado                               |
| Delegado (conta pessoal da Microsoft) | Não suportado                               |
| Aplicativo                            | Nenhum                                        |

A configuração de reunião de aplicativo em nível de locatário é necessária para permitir que um aplicativo chame esta API. O administrador do locatário deve chamar o seguinte cmdlet no PowerShell remoto do locatário para conceder a permissão ao aplicativo para chamar esta API. Para obter mais informações, consulte [set-CsApplicationMeetingConfiguration](https://github.com/MicrosoftDocs/office-docs-powershell/blob/master/skype/skype-ps/skype/Set-CsApplicationMeetingConfiguration.md).
```
PS C:\> Set-CsApplicationMeetingConfiguration -AllowRemoveParticipantAppIds @{Add="app_id"}
```

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /communications/calls/{id}/participants/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

##### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.
<!-- {
  "blockType": "request",
  "name": "delete-participant"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/communications/calls/{id}/participants/{id}
```

##### <a name="response"></a>Resposta

> **Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete participant",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
