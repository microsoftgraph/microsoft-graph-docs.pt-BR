---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aa66c84b04c51af52ad8f0054639c5f98cb9c665
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449122"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

Namespace: microsoft.graph

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







