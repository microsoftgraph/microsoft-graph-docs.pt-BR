---
title: tipo de enumeração remediable
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 49161209ad1a38123067ed3c434cbe31a3a2af70
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725425"
---
# <a name="remediationstate-enum-type"></a>tipo de enumeração remediable

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|ignorados|1|A execução do script de correção foi ignorada|
|sucesso|duas|O script de correção foi executado com êxito e corrigiu o estado do dispositivo|
|remediationFailed|3D|O script de correção foi executado com êxito, mas falhou ao corrigir o estado do dispositivo|
|scriptError|4 |Execução de script de correção encontrada e erro ou tempo limite esgotado|





