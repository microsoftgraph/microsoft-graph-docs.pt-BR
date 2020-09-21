---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou a uma entidade de serviço.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: dd63f52485e27d44681a277df26492c33a1740f3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "47965405"
---
# <a name="passwordcredential-resource-type"></a>tipo de recurso passwordCredential

Namespace: microsoft.graph

Representa uma credencial de senha associada a um aplicativo ou a uma entidade de serviço. A propriedade **passwordCredentials** do [aplicativo](application.md) <!--and [servicePrincipal](serviceprincipal.md) entitites--> Entity é uma coleção de objetos **passwordCredential** .

> [!IMPORTANT]
> Não há suporte para o uso de POST ou PATCH para definir **passwordCredential** . Use os métodos addpassword e removePassword para atualizar a senha de um aplicativo ou de um servicePrincipalName:
>
> - [Application: addpassword](../api/application-addpassword.md)
> - [aplicativo: removePassword](../api/application-removepassword.md)
> - [servicePrincipalName: addpassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipalName: removePassword](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binária | Não usar. |
| displayName | String | Nome amigável da senha. Opcional. |
| endDateTime | DateTimeOffset | A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Opcional. |
| Dica | String | Contém os três primeiros caracteres da senha. Somente leitura. |
| keyId | Guid | O identificador exclusivo da senha. |
| secretText | String | Somente leitura; Contém as senhas fortes geradas pelo Azure AD que têm 16-64 caracteres de comprimento. O valor da senha gerada só é retornado durante a solicitação POST inicial para [addpassword](../api/application-addpassword.md). Não há como recuperar essa senha no futuro. |
| startDateTime | DateTimeOffset | A data e a hora em que a senha se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Opcional. |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "Guid",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

