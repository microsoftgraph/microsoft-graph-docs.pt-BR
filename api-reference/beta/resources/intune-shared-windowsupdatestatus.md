---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1ce9ae47680408f50ef5ce42606cd856ac13ddc1
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199573"
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



