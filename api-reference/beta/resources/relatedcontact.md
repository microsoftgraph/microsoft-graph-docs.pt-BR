---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para tutores, auxiliares, médicos e assim por diante.
author: mmast-msft
ms.author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 37c494d58896af34c1da12e6e500a0561d877911
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960331"
---
# <a name="relatedcontact-resource-type"></a>tipo de recurso relatedContact

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Registro de contato relacionado a [um educationUser](../resources/educationuser.md) que fornece informações para tutores, auxiliares, médicos e assim por diante.

## <a name="methods"></a>Métodos

| Método                                    | Tipo de retorno                   | Descrição                                                             |
| :---------------------------------------- | :---------------------------- | :---------------------------------------------------------------------- |
| [Update](../api/relatedcontact-update.md) | **coleção relatedContact** | Atualizar os **relatedContacts** para um [educationUser](educationuser.md) |

## <a name="properties"></a>Propriedades

| Propriedade      | Tipo                | Descrição                                                                                                                                |
| :------------ | :------------------ | :----------------------------------------------------------------------------------------------------------------------------------------- |
| displayName   | Cadeia de caracteres              | Nome do contato. Obrigatório.                                                                                                             |
| accessConsent | Booliano             | Indica se o usuário foi consentido para acessar dados de alunos.                                                                      |
| emailAddress  | String              | Endereço de email do contato.                                                                                                              |
| mobilePhone   | String              | Número de telefone celular do contato.                                                                                                        |
| relação  | contactRelationship | Relação com o usuário. Os valores possíveis são: `parent`, `relative`, `aide`, `doctor`, `guardian`, `child`, `other`, `unknownFutureValue`. |

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.relatedContact"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.relatedContact",
  "displayName": "String",
  "emailAddress": "String",
  "mobilePhone": "String",
  "relationship": "String",
  "accessConsent": "Boolean"
}
```
