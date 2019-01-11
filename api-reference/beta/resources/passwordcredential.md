---
title: tipo de recurso passwordCredential
description: Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço. A propriedade **passwordCredentials** da entidade servicePrincipal e da entidade do aplicativo é uma coleção de **passwordCredential**.
localization_priority: Normal
ms.openlocfilehash: 5cb995c00a7dcfcfb4bda331e24dcb4d732f04f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814438"
---
# <a name="passwordcredential-resource-type"></a>tipo de recurso passwordCredential

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Contém uma credencial de senha associada a um aplicativo ou uma entidade de serviço. A propriedade **passwordCredentials** da entidade [servicePrincipal](serviceprincipal.md) e da entidade do [aplicativo](application.md) é uma coleção de **passwordCredential**.


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|customKeyIdentifier|Binária|            |
|endDateTime|DateTimeOffset|A data e hora em que a senha expira. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|keyId|Guid|            |
|startDateTime|DateTimeOffset|A data e a hora em que a senha se torna válida. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`|
|secretText|Cadeia de caracteres| As senhas devem ser 16-64 caracteres de comprimento |
|Dica|Cadeia de caracteres|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
