---
title: tipo de recurso de governancePermission
description: 'Representa a permissão de acesso que tenha um governanceSubject um governanceResource específico.  '
localization_priority: Normal
ms.openlocfilehash: e082ca50e5642e865b3e30859eea607df63a03b4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27882870"
---
# <a name="governancepermission-resource-type"></a>tipo de recurso de governancePermission

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

Representa a permissão de acesso que um [governanceSubject](../resources/governancesubject.md) tem um específicos [governanceResource](../resources/governanceresource.md).  


## <a name="properties"></a>Propriedades
| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|accessLevel|Cadeia de caracteres|O nível de acesso. Valores válidos: ``None``, ``UserRead``, ``AdminRead``, e ``AdminReadWrite``.|
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
