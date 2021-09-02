---
title: Tipo de número runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivos.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fee3d6eef67b4af198e0a038875ece20fc640fc3
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817072"
---
# <a name="runstate-enum-type"></a>Tipo de número runState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

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



