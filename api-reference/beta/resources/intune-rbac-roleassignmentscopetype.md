---
title: tipo de enum roleAssignmentScopeType
description: Especifica o tipo de escopo para uma atribuição de função.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 738579fbd8bcda9ac438ada2f7746e020396d225
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871537"
---
# <a name="roleassignmentscopetype-enum-type"></a>tipo de enum roleAssignmentScopeType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Especifica o tipo de escopo para uma atribuição de função.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|resourceScope|0|Permitir que as atribuições para o ResourceScopes especificado.|
|allDevices|1|Permitir que as atribuições para todos os dispositivos Intune.|
|allLicensedUsers|2|Permitir que as atribuições para todos os usuários licenciado do Intune.|
|allDevicesAndLicensedUsers|3|Permitir que as atribuições para todos os dispositivos de Intune e os usuários licenciados.|





