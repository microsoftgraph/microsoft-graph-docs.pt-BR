---
title: Tipo de número runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: efa06c63cd3154bcc7ecc993011f314c2dea9a92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63378725"
---
# <a name="runstate-enum-type"></a>Tipo de número runState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Resultado desconhecido.|
|sucesso|1|O script é executado com êxito.|
|fail|2|Falha ao executar o script.|
|scriptError|3|Erro de acertos de script de descoberta.|
|pendente|4|O script está pendente para ser executado.|
|notApplicable|5|Script não é aplicável para este dispositivo.|




