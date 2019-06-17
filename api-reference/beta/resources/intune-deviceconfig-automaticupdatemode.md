---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d2fffa3e1b1a5e7efa43d7ce653792247e3ad790
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983628"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1|Notifique o download.|
|autoInstallAtMaintenanceTime|duas|Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3D|Instalação automática e reinicialização no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|quatro|Instalação automática e reinicialização no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|0,5|Instalação e reinício automáticos sem controle de usuário final|
|windowsDefault|6|Redefina como o valor padrão do Windows.|





