---
title: 'printer: create'
description: Crie (registre) uma impressora com o serviço Impressão Universal.
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 58285c3c6908812edce8ad80915f44f4df08fcb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516867"
---
# <a name="printer-create"></a>printer: create
Namespace: microsoft.graph

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

Crie (registre) uma impressora com o serviço Impressão Universal. Esta é uma operação de longa duração e, como tal, retorna uma [printerCreateOperation](../resources/printercreateoperation.md) que pode ser usada para rastrear e verificar o registro da impressora.

Para ajudar a criar a CSR (Solicitação de Assinatura de Certificado) necessária para a criação da impressora, consulte o exemplo de código de geração [CSR](/universal-print/hardware/universal-print-oem-certificate-signing-request).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa. O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Sem suporte. |

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-Type|application/json. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
No corpo da solicitação, fornece uma representação JSON dos parâmetros.

A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.

| Parâmetro      | Tipo    |Descrição| Obrigatório? |
|:---------------|:--------|:----------|:----------|
|displayName|Cadeia de caracteres|O nome de exibição a ser atribuído à impressora.|Sim|
|fabricante|String|O fabricante da impressora.|Sim|
|modelo|String|O modelo da impressora.|Sim|
|physicalDeviceId|Cadeia de caracteres|O UUID do dispositivo físico da impressora. Obrigatório se a `hasPhysicalDevice` propriedade for true.|Não|
|hasPhysicalDevice|Booliano|True se a impressora tiver um dispositivo de saída físico, false caso contrário. Se omitido, o valor padrão será true.|Não|
|certificateSigningRequest|[printCertificateSigningRequest](../resources/printcertificatesigningrequest.md)|A Solicitação de Assinatura de Certificado X.509 (CSR) para o certificado criado e usado pela impressora para se identificar.|Sim|
|connectorId|Cadeia de caracteres|ID do conector atuando como proxy para a impressora.|Não|

## <a name="response"></a>Resposta
Se tiver êxito, este método retornará um código de resposta e um link para `202 Accepted` a [impressora associadaCreateOperation](../resources/printercreateoperation.md) no `Operation-Location` header.

Você faz uma solicitação GET para a URL vinculada para obter o status de um registro de impressora em andamento. Depois que o registro da impressora for concluído com êxito, uma solicitação GET para a URL vinculada conterá o objeto de impressora criado e o certificado registrado.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json
Content-length: 287

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


### <a name="response"></a>Resposta

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/v1.0/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

