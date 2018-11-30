---
title: tipo de recurso de governancePermission
description: 'Representa a permissão de acesso que tenha um governanceSubject um governanceResource específico.  '
ms.openlocfilehash: d7b3e1eb70c89c278ccc2a8b3e9a16e265e4ae97
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037736"
---
# <a name="governancepermission-resource-type"></a>tipo de recurso de governancePermission

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem um específicos [governanceResource](../resources/governanceresource.md).  


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|String|O nível de acesso. Valores válidos: ``None``, ``UserRead``, ``AdminRead``, e ``AdminReadWrite``.|
|isActive|Booliano|Indique se o solicitante tem qualquer atribuição de função ativa para o nível de acesso.|
|isEligible|Booliano|Indica se o solicitante tem qualquer atribuição de função elegíveis para o nível de acesso.|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "accessLevel": "String",
  "isActive": true,
  "isEligible": true
}

```