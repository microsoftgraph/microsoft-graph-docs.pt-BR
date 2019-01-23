---
title: tipo de enum windowsUpdateStatus
description: Windows update para os estados de dispositivo de configuração de negócios
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 74493359eeccdbc6df1c351ecec771b5990649b6
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431294"
---
# <a name="windowsupdatestatus-enum-type"></a>tipo de enum windowsUpdateStatus

> **Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.

Windows update para os estados de dispositivo de configuração de negócios

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|upToDate|0|Não existem atualizações pendentes, não pendentes atualizações de reinicialização e falhas de atualização.|
|pendingInstallation|1|Há atualizações da instalação que inclui atualizações que não estão aprovadas pendente. Há atualizações sem reinicialização pendente, não há falhas de atualização.|
|pendingReboot|2|Há atualizações que exige reinicialização. Não há falhas de atualização.|
|Falha|3|Há atualizações Falha ao instalar no dispositivo.|




