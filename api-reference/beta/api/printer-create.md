---
title: 'printer: create'
description: Cria (registra) uma impressora com o serviço Impressão Universal.
author: braedenp-msft
ms.localizationpriority: medium
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 328f4d1bb9ada8ceb99be79caa60a9683d15d368
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028086"
---
# <a name="printer-create"></a>printer: create

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Crie (registre) uma impressora com o serviço Impressão Universal. Esta é uma operação de longa duração e, como tal, retorna uma [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usada para rastrear e verificar o registro da impressora.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa. O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | {token} de portador. Obrigatório. |
| Content-type  | application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, forneça um objeto JSON com as seguintes propriedades.

| Parâmetro      | Tipo    |Descrição| Obrigatório? |
|:---------------|:--------|:----------|:----------|
|displayName|Cadeia de caracteres|O nome de exibição a ser atribuído à impressora.|Sim|
|fabricante|String|O fabricante da impressora.|Sim|
|modelo|String|O modelo da impressora.|Sim|
|physicalDeviceId|String|O UUID do dispositivo físico da impressora. Obrigatório se a `hasPhysicalDevice` propriedade for true.|Não|
|hasPhysicalDevice|Booliano|True se a impressora tiver um dispositivo de saída físico, false caso contrário. Se omitido, o valor padrão será true.|Não|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|A Solicitação de Assinatura de Certificado X.509 (CSR) para o certificado criado e usado pela impressora para se identificar.|Sim|
|connectorId|Cadeia de caracteres|ID do Conector atuando como proxy para a impressora.|Não|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um link para `202 Accepted` a [impressora associadaCreateOperation](../resources/printercreateoperation.md) no `Operation-Location` header.

Fazer uma solicitação GET para a URL vinculada pode ser usada para obter o status de um registro de impressora em andamento. Depois que o registro da impressora for concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto de impressora criado e o certificado registrado.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação
Este é um exemplo de solicitação.


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/create-printer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
Este é um exemplo de resposta.

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
