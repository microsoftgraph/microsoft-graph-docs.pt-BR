---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ecf868f77bc5460af95375ef88d73e7384ef4ccf
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538697"
---
# <a name="runstate-enum-type"></a>tipo de enumeração runState

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|sucesso|1|O script é executado com êxito.|
|fail|duas|O script não pôde ser executado.|
|scriptError|3D|Erro de ocorrências de script de descoberta.|
|função|4 |O script está pendente para execução.|
|Não aplicável|5 |O script não se aplica a este dispositivo.|



