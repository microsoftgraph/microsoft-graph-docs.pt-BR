---
title: Tipo de número automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 32fd3240f72ee48b3550e23530ede460d0756b077329359d9d522e942f7aba84
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249304"
---
# <a name="automaticupdatemode-enum-type"></a>Tipo de número automaticUpdateMode

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|User Defined, default value, no intent.|
|notifyDownload|1|Notificar no download.|
|autoInstallAtMaintenanceTime|2|Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3|Instale e reinicie automaticamente no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|4 |Instale e reinicie automaticamente no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5 |Instalar e reiniciar automaticamente sem o controle do usuário final|




