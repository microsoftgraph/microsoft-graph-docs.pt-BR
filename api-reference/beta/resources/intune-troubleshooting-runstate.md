---
title: Tipo de número runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivos.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4f25057c0fcd19b3a9ad121471876f7b6f1e5d15
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020172"
---
# <a name="runstate-enum-type"></a>Tipo de número runState

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivos.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Resultado desconhecido.|
|sucesso|1|O script é executado com êxito.|
|fail|2|Falha ao executar o script.|
|scriptError|3|Erro de acertos de script de descoberta.|
|pendente|4 |O script está pendente para ser executado.|
|notApplicable|5 |Script não é aplicável para este dispositivo.|




