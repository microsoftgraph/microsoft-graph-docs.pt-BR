---
title: Tipo de recurso tenantContactInformation
description: Representa um contato em um locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f852bbae5a08c00d101e122443b9e5b50382eb62
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860457"
---
# <a name="tenantcontactinformation-resource-type"></a>Tipo de recurso tenantContactInformation

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa um contato em um locatário gerenciado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|email|Cadeia de caracteres|O endereço de email do contato. Opcional|
|nome|String|O nome do contato. Obrigatório.|
|notes|String|As anotações associadas ao contato. Opcional|
|phone|Cadeia de caracteres|O número de telefone do contato. Opcional.|
|title|String|O título do contato. Obrigatório.|

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
