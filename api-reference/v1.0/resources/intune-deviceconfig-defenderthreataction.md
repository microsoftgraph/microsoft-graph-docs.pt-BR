---
title: Tipo de número defenderThreatAction
description: Ação padrão do Defender para assumir ameaças de Malware detectadas.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 706a068817d972ba1a9ed2bc3c55d880c849cddb
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59044661"
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
|userDefined|5 |Permita que o usuário determine a ação a ser tomada com a ameaça detectada.|
|block|6 |Bloqueie a ameaça detectada.|




