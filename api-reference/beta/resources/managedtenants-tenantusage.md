---
title: Tipo de recurso tenantUsage
description: Representa o número de usuários ativos mensais por serviço em um locatário gerenciado do mês anterior. O período de tempo para os dados é uma janela deslizante que tira um instantâneo uma vez por dia.
author: kylewirpel
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: f1d568e2218c460aeef9bff54db636f30ac94d07
ms.sourcegitcommit: d7efd03a6782da5e44b422c9016869c779d64add
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2022
ms.locfileid: "65398637"
---
# <a name="tenantusage-resource-type"></a>Tipo de recurso tenantUsage

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa o número de usuários ativos mensais por serviço em um locatário gerenciado do mês anterior. O período de tempo para os dados é uma janela deslizante que tira um instantâneo uma vez por dia.


## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar tenantUsage](../api/managedtenants-managedtenant-list-tenantusage.md)|[Coleção microsoft.graph.managedTenants.tenantUsage](../resources/managedtenants-tenantusage.md)|Obtém [os dados de uso mensal para cada serviço](../resources/managedtenants-tenantusage.md) em um [locatário gerenciado](../resources/managedtenants-managedtenant.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo do locatário. Obrigatório. Somente leitura.|
|reportDateTime|DateTimeOffset|O dia em que o relatório foi gerado para o mês anterior. Obrigatório. Somente leitura.|
|serviceUsages|[Coleção microsoft.graph.managedTenants.serviceUsage](../resources/managedtenants-serviceusage.md)|O número de usuários ativos mensais para cada serviço no locatário. Serviços de exemplo: , , , , , `Word``Teams`. `Outlook``Intune``Exchange``Excel` Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory de locatário do locatário [gerenciado](../resources/managedtenants-tenant.md). Somente leitura.|
|totalActiveUsers|Int32|O número total de usuários exclusivos e ativos. Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.tenantUsage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantUsage",
  "id": "String (identifier)",
  "serviceUsages": [
    {
      "@odata.type": "microsoft.graph.managedTenants.serviceUsage"
    }
  ],
  "tenantId": "String",
  "reportDateTime": "String (timestamp)",
  "totalActiveUsers": "Integer"
}
```
