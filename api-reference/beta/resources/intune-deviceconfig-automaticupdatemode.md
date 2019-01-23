---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402633"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enum automaticUpdateMode

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1|Notifica baixados.|
|autoInstallAtMaintenanceTime|2|Instalar automaticamente em tempo de manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3|Instalar automaticamente e reinicialize em tempo de manutenção.|
|autoInstallAndRebootAtScheduledTime|4|Instalar automaticamente e reinicialize no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5|Instalar automaticamente e reinicie sem controle de usuário final|
|windowsDefault|6|Redefinido para o valor de padrão do Windows.|




