---
title: Tipo de recurso sharedPCAccountManagerPolicy
description: Política do gerenciador de conta de PC compartilhado. Aplica-se somente quando o gerenciador de contas está habilitado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3d6b7e0ab86af78380f85da8ec37c643e662838c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410991"
---
# <a name="sharedpcaccountmanagerpolicy-resource-type"></a>Tipo de recurso sharedPCAccountManagerPolicy

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




