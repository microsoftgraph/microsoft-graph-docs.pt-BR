---
title: Atualizar dispositivo
description: Atualize as propriedades de um dispositivo.
author: spunukol
ms.localizationpriority: medium
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d432fff2bafa5233d44238e57e06fafd461b96ba
ms.sourcegitcommit: 2f394a9f33f2fab3634d0f18882985ee211067d1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60127531"
---
# <a name="update-device"></a>Atualizar dispositivo

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualize as propriedades de um dispositivo. Somente determinadas propriedades de um dispositivo podem ser atualizadas por meio de aplicativos MDM (Gerenciamento de Dispositivo Móvel) aprovados.

## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão      | Permissões (da com menos para a com mais privilégios)              |
|:--------------------|:---------------------------------------------------------|
|Delegado (conta corporativa ou de estudante) | Device.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All |
|Delegado (conta pessoal da Microsoft) | Sem suporte. |
|Aplicativo | Device.ReadWrite.All, Directory.ReadWrite.All |

## <a name="http-request"></a>Solicitação HTTP

O `{id}` na solicitação é o valor da **propriedade id** do dispositivo, não a **propriedade deviceId.**

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
|accountEnabled|Booliano| `true` se a conta estiver habilitada; caso contrário, `false`. Somente chamadores nas funções Administrador Global e Administrador de Dispositivos de Nuvem podem atualizar essa propriedade. |
|operatingSystem|String|O tipo de sistema operacional do dispositivo.|
|operatingSystemVersion|Cadeia de caracteres|A versão do sistema operacional do dispositivo.|
|displayName|String|O nome de exibição do dispositivo.|
|isCompliant|Booliano|`true` se o dispositivo estiver em conformidade com políticas de Gerenciamento de Dispositivo Móvel (MDM); caso contrário, `false` . Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. |
|isManaged|Booliano|`true` se o dispositivo for gerenciado por um aplicativo MDM (Gerenciamento de Dispositivo Móvel). caso contrário, `false` . Isso só pode ser atualizado pelo Intune para qualquer tipo de sistema operacional de dispositivo ou por um [aplicativo MDM](/windows/client-management/mdm/azure-active-directory-integration-with-mdm) aprovado para Windows do sistema operacional. |

Como o **recurso de** dispositivo dá suporte a extensões, você pode usar a operação para adicionar, atualizar ou excluir seus próprios dados específicos do aplicativo em propriedades [personalizadas](/graph/extensibility-overview)de uma extensão em uma instância de dispositivo `PATCH` existente. 

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
PATCH https://graph.microsoft.com/beta/devices/{id}
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

## <a name="see-also"></a>Confira também

- [Adicionar dados personalizados a recursos usando extensões](/graph/extensibility-overview)
- [Adicionar dados personalizados aos usuários usando extensões abertas (visualização)](/graph/extensibility-open-users)
- [Adicionar dados personalizados a grupos usando extensões do esquema (visualização)](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update device",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
