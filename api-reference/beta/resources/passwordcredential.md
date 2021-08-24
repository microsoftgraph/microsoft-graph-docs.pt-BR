---
title: Tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: e1facb9b3a4de7c8cd5086efbd9ca4cea72fe84a
ms.sourcegitcommit: c6f7a931a8d83ac54f577b7bec08237fd17ce51a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/24/2021
ms.locfileid: "58490627"
---
# <a name="passwordcredential-resource-type"></a>Tipo de recurso passwordCredential

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma credencial de senha associada a um aplicativo ou uma entidade de serviço. A **propriedade passwordCredentials** dos direitos [de](application.md) aplicativo e [servicePrincipal](serviceprincipal.md) é uma coleção de **objetos passwordCredential.**

> [!IMPORTANT]
> Não há suporte para usar POST ou PATCH **para definir passwordCredential.** Use os seguintes métodos addPassword e removePassword para atualizar a senha de um aplicativo ou um servicePrincipal:
>
> - [application: addPassword](../api/application-addpassword.md)
> - [application: removePassword](../api/application-removepassword.md)
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
| customKeyIdentifier | Binário | Não usar. |
| displayName | Cadeia de caracteres | Nome amigável para a senha. Opcional. |
| endDateTime | DateTimeOffset | A data e a hora em que a senha expira representada usando o formato ISO 8601 e está sempre em horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional. |
| dica | Cadeia de caracteres | Contém os três primeiros caracteres da senha. Somente leitura. |
| keyId | Guid | O identificador exclusivo da senha. |
| secretText | Cadeia de caracteres | Somente leitura; Contém as senhas fortes geradas pelo Azure AD que têm entre 16 e 64 caracteres. O valor de senha gerado só é retornado durante a solicitação POST inicial [para addPassword](../api/application-addpassword.md). Não há como recuperar essa senha no futuro. |
| startDateTime | DateTimeOffset | A data e a hora em que a senha se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`. Opcional. |

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


