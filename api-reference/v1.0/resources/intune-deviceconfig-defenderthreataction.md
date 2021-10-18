---
title: Tipo de número defenderThreatAction
description: Ação padrão do Defender para assumir ameaças de Malware detectadas.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a29ca5d0016c90d49ac6cc8febdf21b95feafef6
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60454597"
---
# <a name="defenderthreataction-enum-type"></a>Tipo de número defenderThreatAction

Namespace: microsoft.graph

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
|userDefined|5|Permita que o usuário determine a ação a ser tomada com a ameaça detectada.|
|block|6 |Bloqueie a ameaça detectada.|



