---
title: Atualização da impressora
description: Atualize as propriedades de um objeto printer.
author: nilakhan
ms.localizationpriority: medium
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 8f52b320187aade2db0d91fb5c82b2e9a5d42ce4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/20/2022
ms.locfileid: "62091971"
---
# <a name="update-printer"></a>Atualização da impressora
Namespace: microsoft.graph

Atualize as propriedades de um [objeto printer.](../resources/printer.md)

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

Além das permissões a seguir, o locatário do usuário deve ter uma assinatura de Impressão Universal ativa. O usuário inscreveu deve ser um [Administrador de Impressora.](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)

>**Observação:** Somente o aplicativo que registrou a impressora tem permissão para atualizar a impressora usando permissões de aplicativo.

|Tipo de permissão | Permissões (da com menos para a com mais privilégios) |
|:---------------|:--------------------------------------------|
|Delegado (conta corporativa ou de estudante)| Printer.ReadWrite.All, Printer.FullControl.All |
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo| Printer.ReadWrite.All |

>**Observação:** No momento, somente as impressoras que não têm dispositivo físico podem ser atualizadas usando permissões de aplicativo.

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|
|Content-type|`application/json` ao usar permissões delegadas `application/ipp` ou ao usar permissões de `application/json` aplicativo. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

### <a name="delegated-permissions-and-json-payload"></a>Permissões delegadas e carga JSON

Se estiver usando permissões delegadas, no corpo da solicitação, forneça os valores para os campos de [impressora relevantes](../resources/printer.md) que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados. 

As propriedades a seguir podem ser atualizadas usando permissões delegadas.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|defaults|[printerDefaults](../resources/printerdefaults.md)|As configurações de impressão padrão da impressora.|
|localização|[printerLocation](../resources/printerlocation.md)|O local físico e/ou organizacional da impressora.|
|displayName|Cadeia de caracteres|O nome da impressora.|

### <a name="application-permissions-and-json-payload"></a>Permissões de aplicativo e carga JSON
No corpo da solicitação, fornece os valores para os campos de [impressora relevantes](../resources/printer.md) que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados. 

As propriedades a seguir podem ser atualizadas usando permissões de aplicativo.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|defaults|[printerDefaults](../resources/printerdefaults.md)|As configurações de impressão padrão da impressora.|
|capabilities|[printerCapabilities](../resources/printerCapabilities.md)|Os recursos da impressora associados a esse compartilhamento de impressora.|
|displayName|Cadeia de caracteres|O nome da impressora.|
|fabricante|String|O fabricante da impressora.|
|modelo|String|O nome do modelo da impressora.|
|status|[printerStatus](../resources/printerstatus.md)|O status de processamento da impressora, incluindo quaisquer erros.|
|isAcceptingJobs|Booliano|Se a impressora está aceitando novos trabalhos de impressão no momento.|

### <a name="application-permissions-and-ipp-payload"></a>Permissões de aplicativo e carga IPP

Com permissões de aplicativo, uma impressora também pode ser atualizada usando uma carga IPP (Internet Printing Protocol). Nesse caso, o corpo da solicitação contém um fluxo binário que representa o grupo Atributos da Impressora na [codificação IPP.](https://tools.ietf.org/html/rfc8010)

O cliente DEVE fornecer um conjunto de atributos printer com um ou mais valores (incluindo valores fora de banda explicitamente permitidos), conforme definido em Atributos de Descrição da Impressora [RFC8011 seção 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Atributos de Modelo de Trabalho ("xxx-default", "xxx-supported" e "xxx-ready"), Atributos de Descrição da Impressora da Seção [5.4](https://tools.ietf.org/html/rfc8011#section-5.4) e quaisquer extensões de atributo suportadas pela Impressora. Os valores de cada atributo Printer fornecido substituem os valores do atributo Printer correspondente no objeto Printer de destino. Para atributos que podem ter vários valores (1setOf), todos os valores fornecidos pelo cliente substituem todos os valores do atributo de objeto Printer correspondente.

> **Observação:** Não passe atributos de operação no corpo da solicitação. O corpo da solicitação deve conter apenas atributos de impressora.


> **Observação:** Para que as impressoras funcionem com uma plataforma específica, ela deve atender aos requisitos dessa plataforma. Por exemplo, no cliente windows, é esperado que a impressora especifique todos os atributos considerados obrigatórios de acordo com as especificações [MOPRIA.](https://mopria.org) Observe que as especificações MOPRIA estão disponíveis apenas para os membros pagos da MOPRIA.

## <a name="response"></a>Resposta

### <a name="delegated-permissions-and-json-payload"></a>Permissões delegadas e carga JSON

Se estiver usando permissões delegadas, se bem-sucedido, este método retornará um código de resposta e um objeto de impressora `200 OK` atualizado no corpo da resposta. [](../resources/printer.md)

### <a name="application-permissions-and-json-payload"></a>Permissões de aplicativo e carga JSON

Se estiver usando permissões delegadas, se bem-sucedido, este método retornará um código de resposta e um objeto de impressora `200 OK` atualizado no corpo da resposta. [](../resources/printer.md)

### <a name="application-permissions-and-ipp-payload"></a>Permissões de aplicativo e carga IPP

Se estiver usando permissões de aplicativo, se bem-sucedido, este método retornará `204 No content` o código de resposta. Não retorna nada no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}
Content-Type: application/json

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Go](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-printer-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-printer-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
    "state": "idle",
    "details": [],
    "description": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "contentType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

