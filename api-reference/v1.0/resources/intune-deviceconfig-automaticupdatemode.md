---
title: Tipo de número automaticUpdateMode
description: Valores possíveis para o modo de atualização automática.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e3a076fcc88cb64ddeebddcb7f97c3e77c2b34ec
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59136478"
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




