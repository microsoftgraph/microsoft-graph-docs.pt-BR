---
title: tipo de enum embeddedSIMDeviceStateValue
description: Descreve os diversos estados de um código de ativação SIM incorporado.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b2da255ef2d0cf192dd09a6351bbd337f3cd9b5c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421323"
---
# <a name="embeddedsimdevicestatevalue-enum-type"></a>tipo de enum embeddedSIMDeviceStateValue

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

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




