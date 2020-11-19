---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3a09aca9ce1ac4cd81e09b8db8da10ea563f1f03
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49272364"
---
# <a name="windowsupdatestatus-enum-type"></a>tipo de enumeração windowsUpdateStatus

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados do dispositivo de configuração do Windows Update para empresas

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|upToDate|,0|Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.|
|pendingInstallation|1|Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas. Não há atualizações de reinicialização pendentes, não há atualizações com falha.|
|pendingReboot|duas|Há atualizações que exigem reinicialização. Não há atualizações com falha.|
|falhou|3D|Há atualizações que não puderam ser instaladas no dispositivo.|




