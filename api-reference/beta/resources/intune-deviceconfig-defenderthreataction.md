---
title: Tipo de número defenderThreatAction
description: Ação padrão do Defender para assumir ameaças de Malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3026c49e54ced17b3442458df20a15044123a25fc1dda23f303624ce49816093
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54242992"
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
|clean|1 |Limpe a ameaça detectada.|
|quarantine|2|Coloque em quarentena a ameaça detectada.|
|remove|3 |Remova a ameaça detectada.|
|allow|4 |Permitir a ameaça detectada.|
|userDefined|5 |Permita que o usuário determine a ação a ser tomada com a ameaça detectada.|
|block|6 |Bloqueie a ameaça detectada.|




