---
title: Excluir chamada
description: Excluir ou desligar uma chamada ativa.
author: mkhribech
ms.localizationpriority: medium
ms.prod: cloud-communications
doc_type: apiPageType
ms.openlocfilehash: 6f409c1fe0478bc92c2b4055d2d526f1bff539aa
ms.sourcegitcommit: 0076eb6abb89be3dca3575631924a74a5202be30
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/03/2022
ms.locfileid: "64629362"
---
# <a name="delete-call"></a>Excluir chamada

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Excluir ou desligar uma chamada ativa. Para chamadas de grupo, isso excluirá apenas sua etapa de chamada e a chamada de grupo subjacente continuará.

## <a name="permissions"></a>Permissões

| Tipo de permissão | Permissões (da com menos para a com mais privilégios)                  |
| :-------------- | :----------------------------------------------------------- |
| Delegado (conta corporativa ou de estudante)     | Sem suporte.                         |
| Delegada (conta pessoal da Microsoft) | Sem suporte.                         |
| Aplicativo                            | Calls.Initiate.All, Calls.AccessMedia.All |

> **Observação:** As permissões são verificadas quando a chamada é criada; nenhuma verificação de permissão adicional é feita ao chamar essa API. Calls.AccessMedia.All só é necessário para chamadas que usam mídia hospedada pelo aplicativo.

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
DELETE /app/calls/{id}
DELETE /communications/calls/{id}
```
> **Observação:** o caminho `/app` foi preterido. Daqui em diante, use o caminho `/communications`.

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição               |
|:--------------|:--------------------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se bem-sucedido, este método retorna um código de resposta `204 No Content`. Não retorna nada no corpo da resposta.

## <a name="example"></a>Exemplo

### <a name="request"></a>Solicitação
O exemplo a seguir mostra a solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete-call-1"
}-->
```http
DELETE https://graph.microsoft.com/beta/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-call-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-call-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-call-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-call-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/delete-call-1-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/delete-call-1-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta

> **Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="notification---terminating"></a>Notificação - término

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "updated",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminating"
      }
    }
  ]
}
  
```

### <a name="notification---terminated"></a>Notificação - encerrada

```http
POST https://bot.contoso.com/api/calls
Content-Type: application/json
```

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsNotifications"
}-->
```json
{
  "@odata.type": "#microsoft.graph.commsNotifications",
  "value": [
    {
      "@odata.type": "#microsoft.graph.commsNotification",
      "changeType": "deleted",
      "resourceUrl": "/communications/calls/57dab8b1-894c-409a-b240-bd8beae78896",
      "resourceData": {
        "@odata.type": "#microsoft.graph.call",
        "state": "terminated",
        "resultInfo": {
          "@odata.type": "#microsoft.graph.resultInfo",
          "code": "200",
          "subcode": "5001",
          "message": "The conversation has ended."
        }
      }
    }
  ]
}
```

#### <a name="call-end-reason-codes"></a>Códigos de motivo de término da chamada

Esses são alguns dos códigos de erro comuns recebidos por meio de notificação quando a chamada é encerrada.

| Código | Subcódigo | Motivo da terminação                                                                                 |
| :--- | :------  | :------------------------------------------------------------------------------------------------  |
| 200  | 4097     | Chamada encerrada pelo outro participante na chamada.                                                   |
| 200  | 4521     | Chamada encerrada pelo outro participante em chamada ponto a ponto.                                          |
| 200  | 5000     | Removido da conversa por outro participante.                                              |
| 200  | 5001     | A conversa terminou.                                                                        |
| 200  | 5002     | A conversa terminou como todos os outros participantes deixaram a chamada.                           |
| 200  | 5003     | A conversa terminou.                                                                        |
| 200  | 5007     | A conversa terminou como o iniciador da chamada de grupo que saiu da conversa.               |
| 200  | 5010     | A conversa terminou como apenas um participante permaneceu na conversa.                   |
| 200  | 5012     | A conversa terminou porque não há participantes na lista de entrada.                    |
| 200  | 5013     | A conversa terminou como ninguém mais ingressou na chamada de grupo.                               |
| 200  | 5014     | A conversa terminou porque não foi possível determinar um host em potencial para a chamada de grupo. |
| 200  | 5020     | A conversa terminou porque não há participantes não ocultos na lista de entrada.         |
| 200  | 5030     | A conversa terminou à medida que a duração da sala de saída decorrido.                              |
| 200  | 5300     | O participante foi removido da conversa por outro participante.                              |
| 200  | 5855     | O participante que aguardava no lobby foi removido da conversa após o tempo de inatividade do lobby.     |
| 200  | 7000     | A conversa terminou por bot.                                                                 |
| 200  | 7015     | A chamada terminou como a transferência concluída com êxito.                                                 |
| 200  | 10550    | A conversa terminou por bot.                                                                 |
| 200  | 18503    | O outro participante da chamada ponto a ponto deixou a conversa.                              |
| 200  | 540000/560000   | Chamada encerrada pelo usuário PSTN.                                                                |
| 408  | 8537     | Mantenha o tempo de vida, limpe a chamada inativa.                                                      |
| 408  | 1106     | Não foi recebido um reconhecimento para a aceitação da chamada no tempo alocado.                  |
| 408  | 10057    | Tempo de chamada em tempo hábil devido a nenhuma sinalização dos pontos de extremidade do chamador.                                          |
| 410  | 301005   | Falha na conectividade de mídia.                                                                        |
| 480  | 10037    | Nenhum ponto de extremidade do chamador foi encontrado.                                                                    |
| 480  | 10076    | Não foi possível alcançar o chamador.                                                                       |
| 480  | 10134    | Chamada rejeitada devido à incapacidade de rotear a chamada.                                                  |
| 480  | 10199    | A chamada rejeitada como chamada privada está desabilitada para o usuário.                                         |
| 500  | 1005     | O servidor encontrou um erro de conectividade com a mídia do Bot. Verifique a conectividade de mídia entre Bot e Microsoft. |


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete call",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


