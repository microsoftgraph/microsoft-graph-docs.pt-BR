---
title: tipo de enum embeddedSIMDeviceStateValue
description: Descreve os diversos estados de um código de ativação SIM incorporado.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: a3974c0df65ef9f59242f390b7166e11c3e0c592
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27886055"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>tipo de enum embeddedSIMDeviceStateValue

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Descreve os diversos estados de um código de ativação SIM incorporado.
## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|notEvaluated|0|Designa que o código de ativação SIM incorporado é gratuito e disponível para ser atribuído a um dispositivo.|
|Falha|1|Designa que Intune Service falhou ao entregar esse perfil para um dispositivo.|
|Instalando|2|Designa que o código de ativação SIM incorporado tenha sido atribuído a um dispositivo e o dispositivo está instalando o token.|
|instalado|3|Designa se o código de ativação SIM incorporado foi instalado com êxito no dispositivo de destino.|
|excluindo|4|Designa Intune Service está tentando excluir o perfil do dispositivo.|
|erro|5|Designa o que há um erro com esse perfil.|
|deleted|6|Designa que o perfil é excluído do dispositivo.|
|removedByUser|7|Designa que o perfil é removido do dispositivo pelo usuário|





