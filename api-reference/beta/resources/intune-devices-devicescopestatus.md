---
title: Tipo de enumeração deviceScopeStatus
description: 'Indica o status do escopo do dispositivo depois que o escopo do dispositivo foi habilitado. Os valores possíveis são: none, computing, insufficientData ou completed. O valor padrão é none.'
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8347440c0c02f0f6c148717457616a19c22bc03f
ms.sourcegitcommit: 435d70e7adb27e6cedaf485ebfdab7c3ef9ffacf
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/02/2022
ms.locfileid: "65858495"
---
# <a name="devicescopestatus-enum-type"></a>Tipo de enumeração deviceScopeStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Indica o status do escopo do dispositivo depois que o escopo do dispositivo foi habilitado. Os valores possíveis são: none, computing, insufficientData ou completed. O valor padrão é none.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|none|0|Indica que o escopo do dispositivo não está habilitado e não há cálculos em andamento.|
|Computação|1|Indica que o escopo do dispositivo está habilitado e os dados de métricas de relatório estão sendo recalculados pelo serviço.|
|insufficientData|2|Indica que o escopo do dispositivo está habilitado, mas não há dados suficientes para calcular os resultados. O sistema requer informações de pelo menos 5 dispositivos antes que os cálculos possam ocorrer.|
|Concluído|3|O escopo do dispositivo está habilitado e terminou de recalcular a métrica de relatório. O escopo do dispositivo agora está pronto para ser usado.|
|unknownFutureValue|4|Valor de espaço reservado para expansão futura.|




