---
title: Parar accessReview
description: No Windows Azure AD para acessar o recurso de revisões, parar uma accessReview ativa no momento.  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  (Para impedir que uma análise mais acesso recorrente iniciando a instâncias futuras, atualizá-lo para alterar sua data de término agendada).  Após o acesso revisar paradas, revisores não podem dar entrada e as decisões de revisão de acesso podem ser aplicadas.
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8d71796272cf9852683688a47f3d78eebd849357
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27941461"
---
# <a name="stop-accessreview"></a>Parar accessReview

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

O recurso [acesso analisa](../resources/accessreviews-root.md) Azure AD, pare de um ativo no momento [accessReview](../resources/accessreview.md).  O objeto de destino pode ser uma revisão de acesso de uma única vez, ou uma instância de uma análise mais acesso recorrente.  (Para impedir que uma análise mais acesso recorrente iniciando a instâncias futuras, [atualizá-la](accessreview-update.md) para alterar sua data de término agendada).  Após o acesso revisar paradas, revisores não podem dar entrada e as decisões de revisão de acesso podem ser aplicadas.
## <a name="permissions"></a>Permissions
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão                        | Permissões (da com menos para a com mais privilégios)              |
|:--------------------------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante)     | AccessReview.ReadWrite.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo                            | Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /accessReviews('<id>')/stop()
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome         | Tipo        | Descrição |
|:-------------|:------------|:------------|
| Autorização | string | Portador \{token\}. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.


## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204, No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo
##### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "stop_accessReview"
}-->
```http
POST https://graph.microsoft.com/beta/accessReviews('2975E9B5-44CE-4E71-93D3-30F03B5AA992')/stop()
```
##### <a name="response"></a>Resposta
>**Observação: **o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Stop accessReview",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
