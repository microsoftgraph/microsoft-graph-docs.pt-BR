---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9e4c9edcd596d6dcd40b2cfe873b660651f74bb3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530857"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enumeração defenderThreatAction

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do defender a ser executada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Aplicar ação com base na definição de atualização.|
|ordena|1 |Limpe a ameaça detectada.|
|quarentena|2 |Colocar em quarentena a ameaça detectada.|
|remover|3 |Remova a ameaça detectada.|
|permitiu|4 |Permitir a ameaça detectada.|
|UserDefined|5 |Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Larga|6 |Bloquear a ameaça detectada.|




