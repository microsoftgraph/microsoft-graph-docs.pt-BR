---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 12e6b53230a46aaaade658de093312a518649345
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783288"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>tipo de enumeração embeddedSIMDeviceStateValue

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve os vários Estados de um código de ativação do SIM incorporado.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não avaliado|,0|Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.|
|falhou|1|Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.|
|instalado|duas|Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.|
|instalação|3D|Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.|
|deleta|4 |Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.|
|erro|5 |Designa que há um erro com esse perfil.|
|deleted|6 |Designa que o perfil é excluído do dispositivo.|
|removedByUser|7 |Designa que o perfil foi removido do dispositivo pelo usuário|



