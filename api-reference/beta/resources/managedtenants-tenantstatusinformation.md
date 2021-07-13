---
title: Tipo de recurso tenantStatusInformation
description: Representa informações de status de integração para um locatário gerenciado.
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 3e01ac003cda223788e0fc8e6dae01f18667da11
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2021
ms.locfileid: "53401991"
---
# <a name="tenantstatusinformation-resource-type"></a>Tipo de recurso tenantStatusInformation

Namespace: microsoft.graph.managedTenants

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa informações de status de integração para um locatário gerenciado.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|delegatedPrivilegeStatus|delegatedPrivilegeStatus|O status da relação de privilégio de administrador delegada entre a entidade de gerenciamento e o locatário gerenciado. Os valores possíveis são: `none`, `delegatedAdminPrivileges`, `unknownFutureValue`. Opcional. Somente leitura.|
|lastDelegatedPrivilegeRefreshDateTime|DateTimeOffset|A data e a hora em que o status dos privilégios de administrador delegado foi atualizado. Opcional. Somente leitura.|
|offboardedByUserId|Cadeia de caracteres|O identificador da conta que desarmou o locatário gerenciado. Opcional. Somente leitura.|
|offboardedDateTime|DateTimeOffset|A data e a hora em que o locatário gerenciado foi desligado. Opcional. Somente leitura.|
|onboardedByUserId|Cadeia de caracteres|O identificador da conta que integrava o locatário gerenciado. Opcional. Somente leitura.|
|onboardedDateTime|DateTimeOffset|A data e a hora em que o locatário gerenciado foi internado. Opcional. Somente leitura.|
|onboardingStatus|tenantOnboardingStatus|O status de integração do locatário gerenciado. Os valores possíveis são: `ineligible`, `inProcess`, `active`, `inactive`, `unknownFutureValue`. Opcional. Somente leitura.|
|workloadStatuses|[coleção microsoft.graph.managedTenants.workloadStatus](../resources/managedtenants-workloadstatus.md)|A coleção de estatuetas de carga de trabalho para o locatário gerenciado. Opcional. Somente leitura.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.tenantStatusInformation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.tenantStatusInformation",
  "onboardingStatus": "String",
  "onboardedDateTime": "String (timestamp)",
  "onboardedByUserId": "String",
  "offboardedDateTime": "String (timestamp)",
  "offboardedByUserId": "String",
  "delegatedPrivilegeStatus": "String",
  "lastDelegatedPrivilegeRefreshDateTime": "String (timestamp)",
  "workloadStatuses": [
    {
      "@odata.type": "microsoft.graph.managedTenants.workloadStatus"
    }
  ]
}
```
