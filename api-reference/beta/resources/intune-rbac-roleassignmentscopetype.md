---
title: tipo de enumeração roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d9659c4eaa1f4080ef5dd07a5e69f76a7a14d50
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32573050"
---
# <a name="roleassignmentscopetype-enum-type"></a>tipo de enumeração roleAssignmentScopeType

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica o tipo de escopo de uma atribuição de função.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|resourceScope|,0|Permite atribuições para o ResourceScopes especificado.|
|objectDevices|1 |Permitir atribuições de todos os dispositivos do Intune.|
|allLicensedUsers|2 |Permitir atribuições a todos os usuários licenciados do Intune.|
|allDevicesAndLicensedUsers|3 |Permitir atribuições de todos os dispositivos do Intune e usuários licenciados.|





