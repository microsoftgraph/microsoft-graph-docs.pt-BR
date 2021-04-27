---
title: tipo de recurso relatedContact
description: Registro de contato relacionado a um educationUser que fornece informações para tutores, auxiliares, médicos e assim por diante.
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 4859492f016b88a39c375d3556270f5496b8b318
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52035950"
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
| displayName   | String              | Nome do contato. Obrigatório.                                                                                                             |
| accessConsent | Boolean             | Indica se o usuário foi consentido para acessar dados de alunos.                                                                      |
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
