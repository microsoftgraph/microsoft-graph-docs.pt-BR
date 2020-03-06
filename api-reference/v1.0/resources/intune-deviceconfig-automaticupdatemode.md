---
title: tipo de enumeração Propriedades automaticupdatemode
description: Valores possíveis para o modo de atualização automática.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d0723bef94d187452d6b622c290f7e4cb0182db
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42532614"
---
# <a name="automaticupdatemode-enum-type"></a>tipo de enumeração Propriedades automaticupdatemode

Namespace: microsoft.graph

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




