---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso depois que quaisquer trabalhos pendentes existentes são concluídos, cancelados ou cancelados.
author: braedenp-msft
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 288e3b8cfcd1458f7d71c8fb43ae57ac97237e56
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52049874"
---
# <a name="printjob-start"></a>printJob: start

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Envia o trabalho de impressão para a impressora [associada](../resources/printer.md) ou [printerShare](../resources/printershare.md). Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, abortados ou cancelados.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [Obter](printer-get.md) impressora ou [Obter printerShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Application| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
```http
POST /print/shares/{id}/jobs/{id}/start
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome          | Descrição   |
|:--------------|:--------------|
| Autorização | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

Não envie um corpo de solicitação para este método. 

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.

## <a name="example"></a>Exemplo
O exemplo a seguir mostra como chamar essa API.
##### <a name="request"></a>Solicitação

```http
POST https://graph.microsoft.com/beta/print/shares/{id}/jobs/{id}/start
```

##### <a name="response"></a>Resposta
Este é um exemplo de resposta. 
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.

```http
HTTP/1.1 200 OK

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```


