---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
author: tfitzmac
ms.openlocfilehash: 7eafffbfac115c95cbf2c62be630cf7958965ce9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306563"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>Tipo de recurso sharedPCAccountManagerPolicy

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accountDeletionPolicy|[sharedPCAccountDeletionPolicyType](../resources/intune-deviceconfig-sharedpcaccountdeletionpolicytype.md)|Configura quando as contas são excluídas. Os valores possíveis são: `immediate`, `diskSpaceThreshold`, `diskSpaceThresholdOrInactiveThreshold`.|
|cacheAccountsAboveDiskFreePercentage|Int32|Define a porcentagem de espaço em disco disponível que um computador deve ter antes de parar de excluir contas do computador compartilhadas em cache. Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold. Valores válidos de 0 a 100|
|inactiveThresholdDays|Int32|Especifica quando as contas começarão a ser excluídas quando não forem conectadas durante o período especificado, fornecido como um número de dias. Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThreshold ou DiskSpaceThresholdOrInactiveThreshold.|
|removeAccountsBelowDiskFreePercentage|Int32|Define a porcentagem de espaço em disco restante em um computador antes que contas em cache sejam excluídas para liberar espaço em disco. Contas inativas há mais tempo serão excluídas primeiro. Aplicável apenas quando AccountDeletionPolicy é DiskSpaceThresholdOrInactiveThreshold. Valores válidos de 0 a 100|

## <a name="relationships"></a>Relações
Nenhum
## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.sharedPCAccountManagerPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.sharedPCAccountManagerPolicy",
  "accountDeletionPolicy": "String",
  "cacheAccountsAboveDiskFreePercentage": 1024,
  "inactiveThresholdDays": 1024,
  "removeAccountsBelowDiskFreePercentage": 1024
}
```



