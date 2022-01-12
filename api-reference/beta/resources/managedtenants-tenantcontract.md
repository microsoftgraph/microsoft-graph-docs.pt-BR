---
title: Tipo de recurso tenantContract
description: Representa as informações de relação entre um locatário e a entidade de gerenciamento.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: d2531120eda65f90cd541e9f536f74733d423ec8
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61791858"
---
# <a name="tenantcontract-resource-type"></a>Tipo de recurso tenantContract

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa as informações de relação entre um locatário e a entidade de gerenciamento.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|contractType|Int32|O tipo de relação existente entre a entidade de gerenciamento e o locatário. Opcional. Somente leitura.|
|defaultDomainName|String|O nome de domínio padrão para o locatário. Obrigatório. Somente leitura.|
|displayName|String|O nome de exibição do locatário. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantContract"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantContract",
  "contractType": "Integer",
  "displayName": "String",
  "defaultDomainName": "String"
}
```
