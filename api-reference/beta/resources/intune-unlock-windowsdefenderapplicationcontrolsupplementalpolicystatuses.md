---
title: tipo de número windowsDefenderApplicationControlSupplementalPolicyStatuses
description: Valores de enum para os vários status de implantação de política suplementar windowsDefenderApplicationControl.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8ef128d422e27ff747fda91eea6ee3ef046e963
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58805679"
---
# <a name="windowsdefenderapplicationcontrolsupplementalpolicystatuses-enum-type"></a>tipo de número windowsDefenderApplicationControlSupplementalPolicyStatuses

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores de enum para os vários status de implantação de política suplementar windowsDefenderApplicationControl.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|O status da política suplementar WindowsDefenderApplicationControl não é conhecido.|
|sucesso|1|A política suplementar WindowsDefenderApplicationControl está em vigor.|
|tokenError|2|A política suplementar WindowsDefenderApplicationControl está estruturalmente bem, mas há um erro ao autorizar o token.|
|notAuthorizedByToken|3|O token não autoriza essa política suplementar WindowsDefenderApplicationControl.|
|policyNotFound|4 |A política suplementar WindowsDefenderApplicationControl não foi encontrada.|



