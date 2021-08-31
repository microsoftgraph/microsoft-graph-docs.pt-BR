---
title: Tipo denum roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3de3f4852b25228e35aa5834fe8e984c6de953bc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58802940"
---
# <a name="roleassignmentscopetype-enum-type"></a>Tipo denum roleAssignmentScopeType

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Especifica o tipo de escopo de uma atribuição de função.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|resourceScope|0|Permitir atribuições aos ResourceScopes especificados.|
|allDevices|1|Permitir atribuições para todos os dispositivos Intune.|
|allLicensedUsers|2|Permitir atribuições para todos os usuários licenciados do Intune.|
|allDevicesAndLicensedUsers|3|Permitir atribuições para todos os dispositivos Intune e usuários licenciados.|



