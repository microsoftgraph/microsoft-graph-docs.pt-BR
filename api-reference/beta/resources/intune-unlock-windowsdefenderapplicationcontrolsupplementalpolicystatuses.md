---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 69f909f1bac3b33101d5e0e5515ad74588f46be2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449549"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O status da política suplementar do WindowsDefenderApplicationControl não é conhecido.|
|sucesso|1|A política suplementar do WindowsDefenderApplicationControl está em vigor.|
|tokenError|duas|A política suplementar do WindowsDefenderApplicationControl está estruturalmente, mas há um erro com a autorização do token.|
|notAuthorizedByToken|3D|O token não autoriza esta política complementar do WindowsDefenderApplicationControl.|
|policyNotFound|4 |A política suplementar do WindowsDefenderApplicationControl não foi encontrada.|



