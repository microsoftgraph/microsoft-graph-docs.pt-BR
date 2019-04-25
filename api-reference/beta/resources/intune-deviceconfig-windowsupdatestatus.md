---
title: tipo de enumeração windowsUpdateStatus
description: Estados do dispositivo de configuração do Windows Update para empresas
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73cd3208b7729544d6fbd620a13ce295b39aff26
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523620"
---
# <a name="windowsupdatestatus-enum-type"></a>tipo de enumeração windowsUpdateStatus

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Estados do dispositivo de configuração do Windows Update para empresas

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|upToDate|,0|Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.|
|pendingInstallation|1 |Há atualizações com instalação pendente que inclui atualizações que não foram aprovadas. Não há atualizações de reinicialização pendentes, não há atualizações com falha.|
|pendingReboot|2 |Há atualizações que exigem reinicialização. Não há atualizações com falha.|
|falhou|3 |Há atualizações que não puderam ser instaladas no dispositivo.|





