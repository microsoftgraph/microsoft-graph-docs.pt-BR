---
title: Valores de enumeração de gerenciamento multilocatário
description: Valores de enumeração de gerenciamento multilocatário do Microsoft Graph
author: idwilliams
ms.localizationpriority: medium
ms.prod: microsoft-365-lighthouse
doc_type: enumTypes
ms.openlocfilehash: 9b93794e763025b409ff00c0a2b5d13909ca705d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095948"
---
# <a name="multi-tenant-management-enumeration-values"></a>Valores de enumeração de gerenciamento multilocatário

### <a name="delegatedprivilegestatus-values"></a>valores delegatedPrivilegeStatus

|Member|
|:---|
|none|
|delegatedAdminPrivileges|
|unknownFutureValue|
|granularDelegatedAdminPrivileges|
|delegatedAndGranularDelegetedAdminPrivileges|

### <a name="managementactionstatus-values"></a>Valores managementActionStatus

|Member|
|:---|
|toAddress|
|Concluído|
|erro|
|Timeout|
|Inprogress|
|Planejado|
|resolvedBy3rdParty|
|resolvedThroughAlternateMitigation|
|riskAccepted|
|unknownFutureValue|

### <a name="managementcategory-values"></a>valores managementCategory

|Member|
|:---|
|Personalizado|
|dispositivos|
|Identidade|
|unknownFutureValue|

### <a name="managementparametervaluetype-values"></a>Valores managementParameterValueType

|Member|
|:---|
|string|
|inteiro|
|booliano|
|guid|
|Stringcollection|
|Integercollection|
|booleanCollection|
|guidCollection|
|unknownFutureValue|

### <a name="tenantonboardingstatus-values"></a>Valores tenantOnboardingStatus

|Member|
|:---|
|Inelegível|
|inProcess|
|Ativo|
|Inativo|
|unknownFutureValue|

### <a name="tenantonboardingeligibilityreason-values"></a>Valores tenantOnboardingEligibilityReason

|Member|
|:---|
|none|
|Contracttype|
|delegatedAdminPrivileges|
|usersCount|
|license|
|unknownFutureValue|

### <a name="workloadactioncategory-values"></a>Valores workloadActionCategory

|Member|
|:---|
|Automatizado|
|Manual|
|unknownFutureValue|

### <a name="workloadactionstatus-values"></a>Valores workloadActionStatus

|Member|
|:---|
|toAddress|
|Concluído|
|erro|
|Timeout|
|Inprogress|
|unknownFutureValue|

### <a name="workloadonboardingstatus-values"></a>Valores workloadOnboardingStatus

|Member|
|:---|
|notOnboarded|
|integrado|
|unknownFutureValue|
