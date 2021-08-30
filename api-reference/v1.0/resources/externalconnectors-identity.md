---
title: tipo de recurso identity
description: Representa uma identidade usada para definir permissões no conteúdo externo adicionado ao Microsoft Graph.
author: sacampbe-msft
localization_priority: Normal
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 94733a3e9d6595341a515ff525cdf90050f41b4a
ms.sourcegitcommit: 6efd9df497d795988cd85474f379d1989b0995b7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/30/2021
ms.locfileid: "58697483"
---
# <a name="identity-resource-type"></a>tipo de recurso identity

Namespace: microsoft.graph.externalConnectors

Representa uma [identidade](externalconnectors-identity.md) usada para definir permissões no conteúdo externo adicionado ao Microsoft Graph.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar identidade](../api/externalconnectors-externalgroup-post-members.md)|[identity](externalconnectors-identity.md)|Criar um [recurso](../resources/externalconnectors-identity.md) de identidade para um novo membro em [um externalGroup](../resources/externalconnectors-externalgroup.md).|
|[Excluir identidade](../api/externalconnectors-identity-delete.md)|Nenhum|[Exclua um recurso](../resources/externalconnectors-identity.md) de identidade para remover o membro correspondente de um [externalGroup](../resources/externalconnectors-externalgroup.md).|

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                    | Descrição                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | Cadeia de caracteres                  | A ID exclusiva da identidade. Seria a propriedade objectId no caso de usuários ou grupos Azure Active Directory (Azure AD) e a **propriedade id** do **externalGroup** no caso de grupos externos.                                    |
| type           | microsoft.graph.externalConnectors.identityType | O tipo de identidade. Os valores possíveis são: `user` ou para identidades do `group` Azure AD `externalgroup` e para grupos em um sistema externo. |

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.externalConnectors.identity",
  "openType": false
}
-->
``` json
{
  "id": "String (identifier)",
  "type": "String"
}
```
