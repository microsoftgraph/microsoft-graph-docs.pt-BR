---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3b2368ff23387867c0119ff85c387f714ce1c346
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078364"
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
|sucesso|1 |A política suplementar do WindowsDefenderApplicationControl está em vigor.|
|tokenError|2 |A política suplementar do WindowsDefenderApplicationControl está estruturalmente, mas há um erro com a autorização do token.|
|notAuthorizedByToken|3 |O token não autoriza esta política complementar do WindowsDefenderApplicationControl.|
|policyNotFound|4 |A política suplementar do WindowsDefenderApplicationControl não foi encontrada.|






