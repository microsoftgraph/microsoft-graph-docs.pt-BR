---
title: tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Enumerar valores para os vários status de implantação de política complementar do WindowsDefenderApplicationControl.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f40b20966b5f260b9f59ae397499d4e7e63d5266
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523230"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>tipo de enumeração windowsDefenderApplicationControlSupplementalPolicyStatuses

Namespace: Microsoft. Graph

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



