---
title: 'printJob: start'
description: Envia o trabalho de impressão para a impressora ou printerShare associada. Ele será impresso depois que quaisquer trabalhos pendentes existentes são concluídos, cancelados ou cancelados.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 187e62e1de9f380f651433596b7d76fd91161c2c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517017"
---
# <a name="printjob-start"></a>printJob: start
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Envia o trabalho de impressão para a impressora [associada](../resources/printer.md) ou [printerShare](../resources/printershare.md). Ele será impresso depois que quaisquer trabalhos pendentes existentes **são** concluídos, abortados ou cancelados.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa e ter uma permissão que conceda [Obter](printer-get.md) impressora ou [Obter printerShare,](printershare-get.md) dependendo se a impressora ou impressoraShare está sendo usada.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| PrintJob.Create, PrintJob.ReadWriteBasic, PrintJob.ReadWrite, PrintJob.ReadWriteBasic.All, PrintJob.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares/{printerShareId}/jobs/{printJobId}/start
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código `200 OK` de resposta e um objeto [printJobStatus](../resources/printjobstatus.md) no corpo.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "printjob_start"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/jobs/{printJobId}/start
```

### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printJobStatus"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "state": "processing",
    "description": "The print job is currently being processed.",
    "isAcquiredByPrinter": false,
    "details": ["interpreting"]
}
```

