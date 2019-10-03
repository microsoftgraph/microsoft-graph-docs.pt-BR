---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bc8291bfcd1161212c24758fb726d25fc243c805
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366689"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

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




