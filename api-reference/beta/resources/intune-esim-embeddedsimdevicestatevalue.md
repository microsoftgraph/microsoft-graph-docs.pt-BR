---
title: tipo de enumeração embeddedSIMDeviceStateValue
description: Descreve os vários Estados de um código de ativação do SIM incorporado.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8a4369a891af8ebdda818a0e7b62d4c8d827d029
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36326713"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>tipo de enumeração embeddedSIMDeviceStateValue

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve os vários Estados de um código de ativação do SIM incorporado.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Não avaliado|,0|Designa que o código de ativação do SIM incorporado está livre e disponível para ser atribuído a um dispositivo.|
|falhou|1|Designa que o serviço do Intune não pôde entregar este perfil a um dispositivo.|
|instalado|duas|Designa que o código de ativação do SIM incorporado tenha sido atribuído a um dispositivo e que o dispositivo esteja instalando o token.|
|instalação|3D|Designa que o código de ativação do SIM incorporado tenha sido instalado com êxito no dispositivo de destino.|
|deleta|quatro|Designa que o serviço do Intune está tentando excluir o perfil do dispositivo.|
|erro|0,5|Designa que há um erro com esse perfil.|
|deleted|6|Designa que o perfil é excluído do dispositivo.|
|removedByUser|178|Designa que o perfil foi removido do dispositivo pelo usuário|



