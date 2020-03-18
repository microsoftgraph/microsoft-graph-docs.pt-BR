---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 845fdacfb0b29449e4464ec0eea03924632e861b
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795902"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1|Notifique o download.|
|autoInstallAtMaintenanceTime|duas|Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3D|Instalação automática e reinicialização no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|4 |Instalação automática e reinicialização no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5 |Instalação e reinício automáticos sem controle de usuário final|
|windowsDefault|6 |Redefina como o valor padrão do Windows.|



