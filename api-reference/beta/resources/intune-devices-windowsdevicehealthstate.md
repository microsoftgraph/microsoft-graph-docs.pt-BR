---
title: Tipo denum windowsDeviceHealthState
description: Estado de proteção do ponto de extremidade do computador
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5fe5692a8d694076cc060f2c21164fe6a5fe25bb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59142982"
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



