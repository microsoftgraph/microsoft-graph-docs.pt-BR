---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549335"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|,0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1 |Notifique o download.|
|autoInstallAtMaintenanceTime|2 |Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3 |Instalação automática e reinicialização no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|4 |Instalação automática e reinicialização no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5 |Instalação e reinício automáticos sem controle de usuário final|
|windowsDefault|6 |ReDefina como o valor padrão do Windows.|





