---
title: Tipo de recurso tenantContactInformation
description: Representa um contato em um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: b60005cf60a9ac1b96a3b650a853f8b198d27e48
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402138"
---
# <a name="tenantcontactinformation-resource-type"></a>Tipo de recurso tenantContactInformation

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contato em um locatário gerenciado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|email|Cadeia de caracteres|O endereço de email do contato. Opcional|
|nome|Cadeia de caracteres|O nome do contato. Obrigatório.|
|notes|String|As anotações associadas ao contato. Opcional|
|phone|Cadeia de caracteres|O número de telefone do contato. Opcional.|
|title|Cadeia de caracteres|O título do contato. Obrigatório.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContactInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContactInformation",
  "name": "String",
  "title": "String",
  "email": "String",
  "phone": "String",
  "notes": "String"
}
```
