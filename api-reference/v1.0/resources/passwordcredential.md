---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou a uma entidade de serviço. A propriedade **passwordCredentials** da entidade servicePrincipalName e da entidade Application é uma coleção de **passwordCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 9d7b1013d572f98f10634ac6470367fd44ffbb66
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938853"
---
# <a name="passwordcredential-resource-type"></a>tipo de recurso passwordCredential

Representa uma credencial de senha associada a um aplicativo ou a uma entidade de serviço. A propriedade **passwordCredentials** do [aplicativo](application.md) <!--and [servicePrincipal](serviceprincipal.md) entitites--> Entity é uma coleção de objetos **passwordCredential** .

> Observação: não há suporte para o uso de PATCH para atualizar o passwordCredentials. Use o usar os métodos addpassword e removePassword para atualizar a senha de um aplicativo <!--or a servicePrincipal-->.
>
> - Application- [Addpassword](../api/application-addpassword.md)
> - aplicativo- [removePassword](../api/application-removepassword.md)
<!--
> - servicePrincipal - [addPassword](../api/serviceprincipal-addpassword.md)
> - servicePrincipal - [removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binária | Não usar. |
| displayName | Cadeia de caracteres | Nome amigável da senha. Opcional. |
| endDateTime | DateTimeOffset | A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`. Opcional. |
| Dica | Cadeia de caracteres | Contém os três primeiros caracteres da senha. Somente leitura. |
| keyId | Guid | O identificador exclusivo da senha. |
| secretText | Cadeia de caracteres | Somente leitura; Contém as senhas fortes geradas pelo Azure AD que têm 16-64 caracteres de comprimento. O valor da senha gerada só é retornado durante a solicitação POST inicial para [addpassword](../api/application-addpassword.md). Não há como recuperar essa senha no futuro. |
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
