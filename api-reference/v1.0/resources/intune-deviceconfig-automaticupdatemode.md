---
title: Tipo de enumeração automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 58684517d3d6477b0647d29e28d1bd4e29dd1515
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732419"
---
# <a name="automaticupdatemode-enum-type"></a>Tipo de enumeração automaticUpdateMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|Userdefined|0|Definido pelo Usuário, valor padrão, sem intenção.|
|notifyDownload|1|Notificar sobre o download.|
|autoInstallAtMaintenanceTime|2|Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3|Instalação automática e reinicialização no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|4|Instalação automática e reinicialização no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5|Instalar e reiniciar automaticamente sem o controle do usuário final|





