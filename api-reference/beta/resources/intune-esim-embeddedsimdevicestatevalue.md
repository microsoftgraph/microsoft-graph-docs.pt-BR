---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 27e7b9e343d751f0417b7bd5dce3d526c93f131f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736125"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>tipo de enumeração embeddedSIMDeviceStateValue

Namespace: microsoft.graph

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





