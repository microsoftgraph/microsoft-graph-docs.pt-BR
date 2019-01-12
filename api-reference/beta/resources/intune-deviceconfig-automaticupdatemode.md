---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20aa217838848af6d85c023fd6587afe3427e82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913265"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enum automaticUpdateMode

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

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





