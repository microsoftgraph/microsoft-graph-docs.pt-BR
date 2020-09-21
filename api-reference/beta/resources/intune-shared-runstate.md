---
title: tipo de enumeração runState
description: Indica o tipo de status de execução do script de gerenciamento de dispositivo.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 36022987fb96671399523a5936c7799e97db33c8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48084041"
---
# <a name="runstate-enum-type"></a>tipo de enumeração runState

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o tipo de status de execução do script de gerenciamento de dispositivo.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|,0|Resultado desconhecido.|
|sucesso|1 |O script é executado com êxito.|
|fail|2 |O script não pôde ser executado.|
|scriptError|3D|Erro de ocorrências de script de descoberta.|
|função|4 |O script está pendente para execução.|
|Não aplicável|5 |O script não se aplica a este dispositivo.|






