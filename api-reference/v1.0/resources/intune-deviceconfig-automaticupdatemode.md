---
title: tipo de enum automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
ms.openlocfilehash: 01e71e51a47a06aff12dd82e132d7eb468f26229
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346988"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enum automaticUpdateMode

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



