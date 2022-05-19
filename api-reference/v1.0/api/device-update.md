---
title: Atualizar dispositivo
description: Atualiza as propriedades de um dispositivo registrado.
author: sandeo-MSFT
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 99307a2f2de13a6b526dceed38134440e92f8118
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549621"
---
# <a name="update-device"></a>Atualizar dispositivo

Namespace: microsoft.graph

Atualiza as propriedades de um dispositivo registrado.

Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Directory.AccessAsUser.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Device.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

O `{id}` na solicitação é o valor da **propriedade de ID** do dispositivo, não a **propriedade deviceId** .
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```


## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. Somente chamadores nas funções administrador global e administrador de dispositivo de nuvem podem atualizar essa propriedade.|
|operatingSystem|String|O tipo de sistema operacional do dispositivo.|
|operatingSystemVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo.|
|displayName|Cadeia de caracteres|O nome de exibição do dispositivo.|
|isCompliant|Booliano|`true`se o dispositivo estiver em conformidade com as políticas de MDM (mobile Gerenciamento de Dispositivos), caso contrário, `false`. Isso só pode ser atualizado por Intune para qualquer tipo de sistema operacional do dispositivo ou por um aplicativo [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. |
|isManaged|Booliano|`true`se o dispositivo for gerenciado por um aplicativo MDM (mobile Gerenciamento de Dispositivos), caso contrário, `false`. Isso só pode ser atualizado por Intune para qualquer tipo de sistema operacional do dispositivo ou por um aplicativo [MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="examples"></a>Exemplos

### <a name="example-1-update-the-accountenabled-property-of-a-device"></a>Exemplo 1: atualizar a propriedade accountEnabled de um dispositivo

#### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
Content-type: application/json

{
  "accountEnabled": false
}
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-device-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-device-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-device-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-device-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/update-device-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/update-device-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

### <a name="example-2--write-extensionattributes-on-a-device"></a>Exemplo 2: Gravar extensionAttributes em um dispositivo

#### <a name="request"></a>Solicitação


<!-- {
  "blockType": "request",
  "name": "update_device_extensionAttributes"
}-->
```msgraph-interactive
PATCH https://graph.microsoft.com/v1.0/devices/7c06cd31-7c30-4f3b-a5c3-444cd8dd63ac
Content-type: application/json

{
    "extensionAttributes": {
        "extensionAttribute1": "BYOD-Device"
    }
}
```


#### <a name="response"></a>Resposta

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79 
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Example",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
