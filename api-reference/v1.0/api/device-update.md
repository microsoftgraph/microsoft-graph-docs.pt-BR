---
title: Atualizar dispositivo
description: Atualiza as propriedades de um dispositivo registrado.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 25a5dce5242219384c42c5b363a5e7b6688d8e3f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59053657"
---
# <a name="update-device"></a>Atualizar dispositivo

Namespace: microsoft.graph

Atualiza as propriedades de um dispositivo registrado.

Somente algumas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos de gerenciamento de dispositivo móvel aprovados(MDM).

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegada (conta corporativa ou de estudante) | Device.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Delegada (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Device.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP
<!-- { "blockType": "ignored" } -->
```http
PATCH /devices/{id}
```
> Observação: A "id" na solicitação é a propriedade "id" do dispositivo, não a propriedade "deviceId".

## <a name="request-headers"></a>Cabeçalhos de solicitação
| Nome       | Tipo | Descrição|
|:-----------|:------|:----------|
| Autorização  | string  | {token} de portador. Obrigatório. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para as propriedades [device](../resources/device.md) que devem ser atualizadas. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para obter um melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accountEnabled|Booliano| **true** se a conta estiver habilitada; caso contrário, **false**. |
|operatingSystem|String|O tipo de sistema operacional do dispositivo.|
|operatingSystemVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo.|
|displayName|Cadeia de caracteres|O nome de exibição do dispositivo.|
|isCompliant|Booliano|**True** se o dispositivo está em conformidade com políticas de MDM (Gerenciamento de Dispositivo Móvel); caso contrário, **false**. Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. |
|isManaged|Booliano|**true** se o dispositivo for gerenciado por um aplicativo de gerenciamento de dispositivo móvel (MDM); caso contrário, **false**. Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um código de resposta `204 No Content`.

## <a name="example"></a>Exemplo
### <a name="request"></a>Solicitação


# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_device"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/devices/{id}
Content-type: application/json
Content-length: 31

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

---

### <a name="response"></a>Resposta

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
