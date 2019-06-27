---
title: Como trabalhar com ações de execução longa (beta)
description: Este artigo descreve o trabalho com ações de execução longa.
localization_priority: Normal
author: daspek
ms.openlocfilehash: 0403dd8e099a5f21f3b1da7cf74859b664eefa43
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/27/2019
ms.locfileid: "35277767"
---
# <a name="working-with-long-running-actions-beta"></a>Como trabalhar com ações de execução longa (beta)


Algumas respostas de API exigem tempo indeterminado para serem concluídas.
Em vez de ter que esperar até que a ação seja concluída antes de retornar uma resposta, o Microsoft Graph pode usar um padrão de ações de execução longa.
Esse padrão fornece ao aplicativo uma espera para sondar se há atualizações de status em uma ação de execução longa, sem que qualquer solicitação aguarde até que a ação seja concluída.

O padrão geral segue estas etapas:

1. O aplicativo solicita uma ação de execução longa por meio da API. A API aceita a ação e retorna uma resposta `202 Accepted` junto com um cabeçalho de Local para que a URL de API recupere relatórios de status de ação.
2. O aplicativo solicita a URL de relatório de status de ação e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) com o progresso da ação de execução longa.
3. A ação de execução longa é concluída. 
4. O aplicativo solicita a URL de relatório de status da ação novamente e recebe uma resposta [AsyncJobStatus](/graph/api/resources/asyncjobstatus?view=graph-rest-beta) que mostra a conclusão da ação.

## <a name="initial-action-request"></a>Solicitação de ação inicial

Vamos percorrer as etapas para obter um cenário de exemplo de [DriveItem Copy](/graph/api/driveitem-copy?view=graph-rest-beta).
Neste cenário, o aplicativo solicita a cópia de uma pasta que contém uma grande quantidade de dados.
Essa solicitação provavelmente levará vários segundos para ser concluída, pois a quantidade de dados é grande.

<!-- { "blockType": "request", "name": "lro-copy-item-example", "scopes": "files.readwrite" } -->

```http
POST https://graph.microsoft.com/beta/me/drive/items/{folder-item-id}/copy
Content-Type: application/json

{
  "parentReference": {
    "path": "/drive/root:/Documents"
  },
  "name": "Copy of LargeFolder1"
}
```

A API responde que a ação foi aceita e fornece a URL para recuperar o status da ação de execução longa.

<!-- { "blockType": "response" } -->

```http
HTTP/1.1 202 Accepted
Location: https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

**Observação:** o local da URL retornado pode não estar no ponto de extremidade da API do Microsoft Graph.

Em muitos casos, esse pode ser o fim da solicitação, pois a ação de cópia será concluída sem que o aplicativo realize tarefas adicionais.
No entanto, se o aplicativo precisar mostrar o status da ação de cópia ou garantir que ela seja concluída sem erros, poderá fazer isso usando a URL de monitor.

## <a name="retrieve-a-status-report-from-the-monitor-url"></a>Recuperar um relatório de status da URL de monitor

Para verificar o status da ação de cópia, o aplicativo faz uma solicitação para a URL fornecida na resposta anterior. *Observação:* Essa solicitação não requer autenticação, pois a URL é de curta duração e exclusiva para o chamador original. 

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

O serviço responde com a informação de que a ação de execução longa ainda está em andamento:

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
  "operation": "ItemCopy",
  "percentageComplete": 27.8,
  "status": "inProgress"
}
```

As informações podem ser usadas para fornecer uma atualização ao usuário sobre o progresso da ação de cópia. O aplicativo pode continuar a sondar a URL de monitor para solicitar atualizações de status e acompanhar o andamento da ação.

## <a name="retrieve-a-completed-status-report-from-the-monitor-url"></a>Recuperar um relatório de status concluído da URL de monitor

Após alguns segundos, a operação de cópia foi concluída. Dessa vez, quando o aplicativo faz uma solicitação para a URL de monitor, a resposta é um redirecionamento para o resultado concluído da ação.

<!-- { "blockType": "request", "opaqueUrl": true, "name": "lro-check-status-complete", "scopes": "files.readwrite" } -->

```http
GET https://api.onedrive.com/monitor/4A3407B5-88FC-4504-8B21-0AABD3412717
```

Após a conclusão da ação, a resposta do serviço de monitor retornará a resourceId para obter os resultados.

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.asyncJobStatus" } -->

```http
HTTP/1.1 202 Accepted
Content-type: application/json

{
    "percentageComplete": 100.0,
    "resourceId": "01MOWKYVJML57KN2ANMBA3JZJS2MBGC7KM",
    "status": "completed"
}
```

## <a name="retrieve-the-results-of-the-completed-operation"></a>Recuperar os resultados da operação concluída

Depois que o trabalho for concluído, a URL do monitor retornará o resourceId do resultado. Neste caso, trata-se da nova cópia do item original.
Você pode resolver esse novo item usando resourceId; por exemplo:

<!-- {
  "blockType": "request",
  "name": "lro-copy-item-example-complete",
  "scopes": "files.readwrite"
} -->

```http
GET https://graph.microsoft.com/beta/me/drive/items/{item-id}
```

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.driveItem", "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "",
    "name": "Copy of LargeFolder1",
    "folder": { },
    "size": 12019
}
```
#### <a name="sdk-sample-code"></a>Código de exemplo do SDK
# <a name="ctabcs"></a>[C#](#tab/cs)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[Javascript](#tab/javascript)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[Objetivo-C](#tab/objective-c)
[!INCLUDE [sample-code](../includes/lro-copy-item-example-complete-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="supported-resources"></a>Recursos com suporte

Ações de execução longa têm suporte nos métodos de API a seguir

| **Recurso** | **API** |
|:------ | :------ |
| DriveItem | [Copiar](/graph/api/driveitem-copy?view=graph-rest-beta) |

## <a name="prerequisites"></a>Pré-requisitos

As mesmas [permissões](./permissions-reference.md) que são necessárias para realizar uma ação de execução longa também são necessárias para consultar o status de uma ação de execução longa.




<!-- {
  "type": "#page.annotation",
  "description": "Monitor the progress of long-running actions in the API.",
  "keywords": "monitor,long,running,operation,action",
  "section": "documentation",
  "suppressions": [
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /concepts/long-running-actions-overview.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: lro-check-status:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus",
    "Error: lro-check-status-complete:
      Unable to locate a definition for resource type: microsoft.graph.asyncJobStatus"
  ],
  "tocPath": "Concepts/Long running actions"
} -->
