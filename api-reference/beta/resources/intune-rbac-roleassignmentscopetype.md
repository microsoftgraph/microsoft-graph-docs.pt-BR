---
title: Tipo denum roleAssignmentScopeType
description: Especifica o tipo de escopo de uma atribuição de função.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: c067a139cf301a25b6c03bc3b343331031d897c8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59039585"
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



