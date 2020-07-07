---
title: Atualizar profileCardProperty
description: Atualiza as propriedades de um objeto profileCardProperty.
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 1271d36a0fb2ec11e117ac4fac4cb3c95dc06c70
ms.sourcegitcommit: 67433748b69541727185fc1f32ed356718bf6ff1
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2020
ms.locfileid: "45050989"
---
# <a name="update-profilecardproperty"></a>Atualizar profileCardProperty

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Atualizar as propriedades de um objeto [profileCardProperty](../resources/profilecardproperty.md) , identificadas por sua propriedade **directoryPropertyName** .

## <a name="permissions"></a>Permissões

One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).

| Tipo de permissão                        | Permissões (da com menos para a com mais privilégios) |
|:---------------------------------------|:--------------------------------------------|
| Delegado (conta corporativa ou de estudante)     | User. ReadWrite, User. ReadWrite. All          |
| Delegado (conta pessoal da Microsoft) | Sem suporte.                              |
| Aplicativo                            | Sem suporte.                              |

>**Observação:** O uso de permissões delegadas para esta operação exige que o usuário conectado tenha um administrador de locatários ou uma função de administrador global.

## <a name="http-request"></a>Solicitação HTTP

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

| Nome       | Descrição|
|:-----------|:-----------|
| Autorização | Bearer {token}. Required. |
| Content-Type  | application/json. Required. |

## <a name="request-body"></a>Corpo da solicitação

No corpo da solicitação, forneça os valores para os campos relevantes que devem ser atualizados. Propriedades existentes que não estão incluídas no corpo da solicitação terão seus valores anteriores mantidos ou serão recalculadas com base nas alterações a outros valores de propriedade. Para alcançar o melhor desempenho, não inclua valores existentes que não foram alterados.

| Propriedade     | Tipo        | Descrição |
|:-------------|:------------|:------------|
|anotações|coleção profileCardAnnotation| Contém quaisquer rótulos alternativos ou localizados que um administrador optou por especificar.|
|directoryPropertyName|String|Contém o nome da propriedade de diretório que se destina à superfície no cartão de perfil. |

## <a name="response"></a>Resposta

Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto [profileCardProperty](../resources/profilecardproperty.md) atualizado no corpo da resposta.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

O exemplo a seguir adiciona um rótulo localizado "Kostnads Senter" para a localidade "no-NB".
<!-- {
  "blockType": "request",
  "name": "update_profilecardproperty"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/settings/profileCardProperties/CustomAttribute1
Content-type: application/json

{
  "annotations": [
    {
      "localizations": [
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```

### <a name="response"></a>Resposta

Este é um exemplo de resposta.

> **Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        },
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilecardproperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
