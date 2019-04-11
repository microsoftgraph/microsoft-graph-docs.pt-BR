---
title: tipo de enumeração defenderThreatAction
description: Ação padrão do defender a ser executada em ameaças de malware detectadas.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8e16ea7734b61213286d15467701fa3512ebb7d6
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/11/2019
ms.locfileid: "31781131"
---
# <a name="defenderthreataction-enum-type"></a>tipo de enumeração defenderThreatAction

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Ação padrão do defender a ser executada em ameaças de malware detectadas.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|deviceDefault|,0|Aplicar ação com base na definição de atualização.|
|ordena|1|Limpe a ameaça detectada.|
|quarentena|duas|Colocar em quarentena a ameaça detectada.|
|remover|3D|Remova a ameaça detectada.|
|permitiu|quatro|Permitir a ameaça detectada.|
|userDefined|0,5|Permitir que o usuário determine a ação a ser tomada com a ameaça detectada.|
|Larga|6|Bloquear a ameaça detectada.|





