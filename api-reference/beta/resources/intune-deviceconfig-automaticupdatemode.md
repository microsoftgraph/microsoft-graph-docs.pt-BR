---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d44c4db05be66f568ba5c0b9182a6d2ab509088
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527070"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

Namespace: Microsoft. Graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|UserDefined|,0|Definido pelo usuário, valor padrão, sem intenção.|
|notifyDownload|1 |Notifique o download.|
|autoInstallAtMaintenanceTime|2 |Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3 |Instalação automática e reinicialização no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|4 |Instalação automática e reinicialização no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5 |Instalação e reinício automáticos sem controle de usuário final|
|windowsDefault|6 |Redefina como o valor padrão do Windows.|



