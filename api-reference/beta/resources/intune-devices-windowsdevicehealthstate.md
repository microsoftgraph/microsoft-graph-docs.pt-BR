---
title: Tipo denum windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 69323863875fa47d7763c904552b2fcd27dd0ae6
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58787845"
---
# <a name="windowsdevicehealthstate-enum-type"></a>Tipo denum windowsDeviceHealthState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estado de proteção do ponto de extremidade do computador

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|clean|0|O computador está limpo e nenhuma ação é necessária|
|fullScanPending|1|O computador está em estado de verificação completa pendente|
|rebootPending|2|O computador está em estado de reinicialização pendente|
|manualStepsPending|4 |O computador está em estado de etapas manuais pendentes|
|offlineScanPending|8 |O computador está em estado de verificação offline pendente|
|critical|16 |O computador está em estado crítico de falha|



