---
title: Tipo de recurso cloudPcConnection
description: Representa uma conexão de computador na nuvem para um determinado locatário gerenciado.
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f7f306a54354d0c6d4860abd0866001f5e8626f
ms.sourcegitcommit: 71186ad44d8d0df15e10b0f89df68d2ef0cf9d14
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2022
ms.locfileid: "61860429"
---
# <a name="cloudpcconnection-resource-type"></a>Tipo de recurso cloudPcConnection

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma conexão de computador na nuvem para um determinado locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar cloudPcConnections](../api/managedtenants-managedtenant-list-cloudpcconnections.md)|[coleção microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|Obter uma lista dos objetos [cloudPcConnection](../resources/managedtenants-cloudpcconnection.md) e suas propriedades.|
|[Obter cloudPcConnection](../api/managedtenants-cloudpcconnection-get.md)|[microsoft.graph.managedTenants.cloudPcConnection](../resources/managedtenants-cloudpcconnection.md)|Leia as propriedades e as relações de um [objeto cloudPcConnection.](../resources/managedtenants-cloudpcconnection.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|displayName|String|O nome de exibição da conexão do computador na nuvem. Obrigatório. Somente leitura.|
|healthCheckStatus|String|O status de saúde da conexão do computador na nuvem. Os valores possíveis são: `pending`, `running`, `passed`, `failed`, `unknownFutureValue`.  Obrigatório. Somente leitura.|
|id|String|O identificador exclusivo para a conexão de computador na nuvem. Obrigatório. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Obrigatório. Somente leitura.|
|tenantDisplayName|String|O nome de exibição do locatário gerenciado. Obrigatório. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Obrigatório. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.cloudPcConnection",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.cloudPcConnection",
  "id": "String (identifier)",
  "displayName": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "healthCheckStatus": "String",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
