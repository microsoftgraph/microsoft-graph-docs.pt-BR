---
title: tipo de recurso identity
description: Representa uma identidade usada para definir permissões no conteúdo externo adicionado ao Microsoft Graph.
author: sacampbe-msft
ms.localizationpriority: medium
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: fd1b5ce0cb828e4c409062a8fcb05f51c82a943f
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123381"
---
# <a name="identity-resource-type"></a>tipo de recurso identity

Namespace: microsoft.graph.externalConnectors

Representa uma [identidade](externalconnectors-identity.md) usada para definir permissões no conteúdo externo adicionado ao Microsoft Graph.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar identidade](../api/externalconnectors-externalgroup-post-members.md)|[identity](externalconnectors-identity.md)|Criar um [recurso](../resources/externalconnectors-identity.md) de identidade para um novo membro em [um externalGroup](../resources/externalconnectors-externalgroup.md).|
|[Excluir identidade](../api/externalconnectors-identity-delete.md)|Nenhum(a)|[Exclua um recurso](../resources/externalconnectors-identity.md) de identidade para remover o membro correspondente de um [externalGroup](../resources/externalconnectors-externalgroup.md).|

## <a name="properties"></a>Propriedades

| Propriedade       | Tipo                    | Descrição                                                          |
|:---------------|:------------------------|:---------------------------------------------------------------------|
| id             | Cadeia de caracteres                  | A ID exclusiva da identidade. Seria a propriedade objectId no caso de usuários ou grupos Azure Active Directory (Azure AD) e a **propriedade id** do **externalGroup** no caso de grupos externos.                                    |
| tipo           | microsoft.graph.externalConnectors.identityType | O tipo de identidade. Os valores possíveis são: `user` ou para identidades do `group` Azure AD `externalgroup` e para grupos em um sistema externo. |

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
