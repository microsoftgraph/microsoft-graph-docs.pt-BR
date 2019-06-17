---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8ace0b42b09093ce2e9d485271ec607ffd618c9e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34978686"
---
# <a name="windowsupdatestatus-enum-type"></a>tipo de enumeração windowsUpdateStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados do dispositivo de configuração do Windows Update para empresas

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|upToDate|,0|Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.|
|pendingInstallation|1|Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas. Não há atualizações de reinicialização pendentes, não há atualizações com falha.|
|pendingReboot|duas|Há atualizações que exigem reinicialização. Não há atualizações com falha.|
|falhou|3D|Há atualizações que não puderam ser instaladas no dispositivo.|





