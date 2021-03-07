---
title: Criar printerShare
description: Cria um novo compartilhamento de impressora para a impressora especificada.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: f22101ff6a621a48285f8064595916e491eb996d
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516880"
---
# <a name="create-printershare"></a>Criar printerShare
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Crie uma nova **printerShare** para a impressora [especificada](../resources/printer.md).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Para usar o serviço Impressão Universal, o usuário ou locatário do aplicativo deve ter uma assinatura de Impressão Universal ativa, além das permissões listadas na tabela a seguir. O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| PrinterShare.ReadWrite.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/shares
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON do [objeto printerShare.](../resources/printershare.md)

A tabela a seguir mostra as propriedades que podem ser fornecidas ao criar [a printerShare](../resources/printershare.md).

|Propriedade|Tipo|Descrição|Obrigatório?|
|:---|:---|:---|:---|
|impressora|microsoft.graph.printer|A impressora à que essa impressora está relacionada. Use a `printer@odata.bind` sintaxe, conforme mostrado no exemplo a seguir.|Sim|
|displayName|Cadeia de caracteres|O nome do compartilhamento de impressora que os clientes de impressão devem exibir. O comprimento máximo permitido é de 50 caracteres.|Sim|
|allowAllUsers|Booliano|Se `true` , todos os usuários e grupos terão acesso a esse compartilhamento de impressora. Isso sobressalta as listas de permissão definidas pelas propriedades de navegação **allowedUsers** e **allowedGroups.**|Não|

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código `201 Created` de resposta e um objeto [printerShare](../resources/printershare.md) no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/shares
Content-Type: application/json
Content-length: 509

{
  "displayName": "ShareName",
  "allowAllUsers": false,
  "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}"
}
```

### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "status": {
    "state": "ready",
    "details": [],
    "description": ""
  }
}
```

