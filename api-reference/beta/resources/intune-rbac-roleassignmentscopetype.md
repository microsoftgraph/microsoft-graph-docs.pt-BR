---
title: tipo de enum roleAssignmentScopeType
description: Especifica o tipo de escopo para uma atribuição de função.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1b815cf7eb396aa82f49df792ceee0612678077c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419888"
---
# <a name="roleassignmentscopetype-enum-type"></a>tipo de enum roleAssignmentScopeType

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Especifica o tipo de escopo para uma atribuição de função.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|resourceScope|0|Permitir que as atribuições para o ResourceScopes especificado.|
|allDevices|1|Permitir que as atribuições para todos os dispositivos Intune.|
|allLicensedUsers|2|Permitir que as atribuições para todos os usuários licenciado do Intune.|
|allDevicesAndLicensedUsers|3|Permitir que as atribuições para todos os dispositivos de Intune e os usuários licenciados.|




