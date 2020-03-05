---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f922cf51729f178ab9ca94db127efb5b70bb94fe
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523890"
---
# <a name="roleassignmentscopetype-enum-type"></a>tipo de enumeração roleAssignmentScopeType

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica o tipo de escopo de uma atribuição de função.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|resourceScope|,0|Permite atribuições para o ResourceScopes especificado.|
|objectdevices|1 |Permitir atribuições de todos os dispositivos do Intune.|
|allLicensedUsers|2 |Permitir atribuições a todos os usuários licenciados do Intune.|
|allDevicesAndLicensedUsers|3 |Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.|



