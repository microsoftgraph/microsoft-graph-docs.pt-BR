---
title: tipo de recurso riskyUser
description: Representa uma conta sinalizada para risco em cada locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3f66998080abcf9580cdd36e0f3e4b24edab2d2d
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402142"
---
# <a name="riskyuser-resource-type"></a>tipo de recurso riskyUser

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma conta sinalizada para risco em cada locatário gerenciado.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar riskyUsers](../api/managedtenants-managedtenant-list-riskyusers.md)|[coleção microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)|Obter uma lista dos [objetos riskyUser](../resources/managedtenants-riskyuser.md) e suas propriedades.|
|[Obter riskyUser](../api/managedtenants-riskyuser-get.md)|[microsoft.graph.managedTenants.riskyUser](../resources/managedtenants-riskyuser.md)|Leia as propriedades e as relações de um [objeto riskyUser.](../resources/managedtenants-riskyuser.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|O identificador exclusivo dessa entidade. Obrigatório. Somente leitura.|
|isDeleted|Boolean|Um sinalizador indicando se a conta foi excluída. Opcional. Somente leitura.|
|lastRefreshedDateTime|DateTimeOffset|Data e hora em que a entidade foi atualizada pela última vez na plataforma de gerenciamento de vários locatários. Opcional. Somente leitura.|
|riskDetail|Cadeia de caracteres|Os detalhes de risco para a conta sinalizada para risco. Opcional. Somente leitura.|
|riskLastUpdatedDateTime|DateTimeOffset|A data e a hora em que as informações de risco foram atualizadas pela última vez. Opcional. Somente leitura.|
|riskLevel|Cadeia de caracteres|O nível de risco detectado. Os possíveis valores são: `low`, `medium`, `high`, `hidden`, `none`, `unknownFutureValue`. Opcional. Somente leitura.|
|riskState|Cadeia de caracteres|O estado de risco detectado. Os valores possíveis são: `none`, `confirmedSafe`, `remediated`, `dismissed`, `atRisk`, `confirmedCompromised`, `unknownFutureValue`. Opcional. Somente leitura.|
|tenantDisplayName|Cadeia de caracteres|O nome de exibição do locatário gerenciado. Opcional. Somente leitura.|
|tenantId|String|O Azure Active Directory do locatário para o [locatário gerenciado.](../resources/managedtenants-tenant.md) Obrigatório. Somente leitura.|
|userDisplayName|Cadeia de caracteres|O nome de exibição da conta onde o risco foi detectado. Opcional. Somente leitura.|
|userId|Cadeia de caracteres|O identificador da conta de usuário onde o risco foi detectado. Obrigatório. Somente leitura.|
|userPrincipalName|Cadeia de caracteres|O nome principal do usuário (UPN) para a conta onde o risco foi detectado. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedTenants.riskyUser",
  "baseType": "microsoft.graph.entity",
  "openType": true
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.riskyUser",
  "id": "String (identifier)",
  "userId": "String",
  "tenantId": "String",
  "tenantDisplayName": "String",
  "userDisplayName": "String",
  "userPrincipalName": "String",
  "riskState": "String",
  "riskLevel": "String",
  "riskDetail": "String",
  "isDeleted": "Boolean",
  "riskLastUpdatedDateTime": "String (timestamp)",
  "lastRefreshedDateTime": "String (timestamp)"
}
```
