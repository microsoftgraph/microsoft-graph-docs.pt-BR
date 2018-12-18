---
title: tipo de enum roleAssignmentScopeType
description: Especifica o tipo de escopo para uma atribuição de função.
author: tfitzmac
ms.openlocfilehash: 0a3286b3b7bc583323204ca39ff85e01869ddbe7
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343124"
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





