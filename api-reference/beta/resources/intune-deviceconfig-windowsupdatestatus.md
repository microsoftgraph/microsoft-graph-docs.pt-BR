---
title: Tipo de número windowsUpdateStatus
description: Windows atualização para estados de dispositivo de configuração de negócios
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 7da061fafd5ed59c215031b2e2626c8d0d42a50661089e9646455ae6d96c4668
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54213155"
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
|pendingInstallation|1 |Há atualizações que estão pendentes de instalação que incluem atualizações que não são aprovadas. Não há atualizações pendentes de reinicialização, nem atualizações com falha.|
|pendingReboot|2|Há atualizações que exigem reinicialização. Não há atualizações com falha.|
|failed|3 |Há atualizações que não foram instaladas no dispositivo.|




