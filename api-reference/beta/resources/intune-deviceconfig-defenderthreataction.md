---
title: Tipo de número defenderThreatAction
description: Ação padrão do Defender para assumir ameaças de Malware detectadas.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f533b3f9d751d52523c1fc2cb316604fa40827dc
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59120224"
---
# <a name="defenderthreataction-enum-type"></a>Tipo de número defenderThreatAction

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do Defender para assumir ameaças de Malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|0|Aplicar ação com base na definição de atualização.|
|clean|1|Limpe a ameaça detectada.|
|quarantine|2|Coloque em quarentena a ameaça detectada.|
|remove|3|Remova a ameaça detectada.|
|allow|4 |Permitir a ameaça detectada.|
|userDefined|5 |Permita que o usuário determine a ação a ser tomada com a ameaça detectada.|
|block|6 |Bloqueie a ameaça detectada.|



