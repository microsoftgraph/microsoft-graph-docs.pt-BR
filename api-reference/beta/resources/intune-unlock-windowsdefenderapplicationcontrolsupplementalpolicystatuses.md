---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1999c999597d152396590e3faee6d7b472189500
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37537654"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|O status da política suplementar do WindowsDefenderApplicationControl não é conhecido.|
|sucesso|1|A política suplementar do WindowsDefenderApplicationControl está em vigor.|
|tokenError|duas|A política suplementar do WindowsDefenderApplicationControl está estruturalmente, mas há um erro com a autorização do token.|
|notAuthorizedByToken|3D|O token não autoriza esta política complementar do WindowsDefenderApplicationControl.|
|policyNotFound|4 |A política suplementar do WindowsDefenderApplicationControl não foi encontrada.|



