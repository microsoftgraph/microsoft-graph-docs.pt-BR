---
title: Tipo de número automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ab80ab2f3e811435107fbbc8e1395b16f5c5340c39b4b68a138316d91ecc30b3
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54131189"
---
# <a name="automaticupdatemode-enum-type"></a>Tipo de número automaticUpdateMode

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Valores possíveis para o modo de atualização automática.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|userDefined|0|User Defined, default value, no intent.|
|notifyDownload|1 |Notificar no download.|
|autoInstallAtMaintenanceTime|2|Instalação automática no momento da manutenção.|
|autoInstallAndRebootAtMaintenanceTime|3 |Instale e reinicie automaticamente no momento da manutenção.|
|autoInstallAndRebootAtScheduledTime|4 |Instale e reinicie automaticamente no horário agendado.|
|autoInstallAndRebootWithoutEndUserControl|5 |Instalar e reiniciar automaticamente sem o controle do usuário final|
|windowsDefault|6 |Redefinir para Windows valor padrão.|




