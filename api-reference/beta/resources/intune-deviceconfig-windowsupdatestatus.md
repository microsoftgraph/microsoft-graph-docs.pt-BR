---
title: Tipo de número windowsUpdateStatus
description: Windows atualização para estados de dispositivo de configuração de negócios
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 73404f8d01ab6ea047cb94ecc3b21939e4fb3a6c
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58803802"
---
# <a name="windowsupdatestatus-enum-type"></a>Tipo de número windowsUpdateStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Windows atualização para estados de dispositivo de configuração de negócios

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|upToDate|0|Não há atualizações pendentes, nenhuma atualização de reinicialização pendente e nenhuma atualização com falha.|
|pendingInstallation|1|Há atualizações que estão pendentes de instalação que incluem atualizações que não são aprovadas. Não há atualizações pendentes de reinicialização, nem atualizações com falha.|
|pendingReboot|2|Há atualizações que exigem reinicialização. Não há atualizações com falha.|
|failed|3|Há atualizações que não foram instaladas no dispositivo.|



