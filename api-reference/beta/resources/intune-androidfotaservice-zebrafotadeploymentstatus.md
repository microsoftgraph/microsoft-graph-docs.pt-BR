---
title: Tipo de recurso zebraFotaDeploymentStatus
description: Descreve o status de uma única implantação do FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bcc9c905c580b8d20d1bd43ed818e339aaa7ff93
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213053"
---
# <a name="zebrafotadeploymentstatus-resource-type"></a>Tipo de recurso zebraFotaDeploymentStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Descreve o status de uma única implantação do FOTA.

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|state|[zebraFotaDeploymentState](../resources/intune-androidfotaservice-zebrafotadeploymentstate.md)|Consulte a enumeração zebraFotaDeploymentState para obter os valores possíveis. Os valores possíveis são: `pendingCreation`, `createFailed`, `created`, `inProgress`, `completed`, `pendingCancel`, `canceled`, `unknownFutureValue`.|
|totalDevices|Int32|Um inteiro que indica o número total de dispositivos na implantação.|
|totalCreated|Int32|Um inteiro que indica o número total de dispositivos que têm um trabalho no estado CREATED. Normalmente, indica trabalhos que não alcançaram os dispositivos. |
|totalScheduled|Int32|Um inteiro que indica o número total de dispositivos que receberam o json e estão agendados. |
|totalDownloading|Int32|Um inteiro que indica o número total de dispositivos em que a instalação foi bem-sucedida.|
|totalAwaitingInstall|Int32|Um inteiro que indica o número total de dispositivos em que a instalação foi bem-sucedida.|
|totalSucceededInstall|Int32|Um inteiro que indica o número total de dispositivos em que a instalação foi bem-sucedida.|
|totalCanceled|Int32|Um inteiro que indica o número total de dispositivos em que a instalação foi cancelada.|
|totalUnknown|Int32|Um inteiro que indica o número total de dispositivos em que nenhum status de implantação ou estado final foi recebido, mesmo depois que a data de término agendada foi atingida.|
|totalFailedDownload|Int32|Um inteiro que indica o número total de dispositivos que falharam ao baixar o novo arquivo do sistema operacional.|
|totalFailedInstall|Int32|Um inteiro que indica o número total de dispositivos que falharam ao instalar o novo arquivo do sistema operacional.|
|completeOrCanceledDateTime|DateTimeOffset|A data e a hora em que essa implantação foi concluída ou cancelada. A hora de data real é determinada pelo valor do estado. Se o estado for cancelado, essa propriedade manterá a data/hora de cancelamento. Se o estado for concluído, essa propriedade manterá a data/hora de conclusão. Se a implantação não for concluída antes da data de término da implantação, a data/hora e a data/hora de término concluídas serão as mesmas. Isso sempre está no fuso horário de implantação. Observação: uma instalação em andamento pode continuar após a data de término da implantação.|
|cancelRequested|Booliano|Um booliano que indica se um cancelamento foi solicitado na implantação. OBSERVAÇÃO: uma solicitação de cancelamento não garante que a implantação foi cancelada.|
|lastUpdatedDateTime|DateTimeOffset| Data e hora em que o status da implantação foi atualizado da Zebra|

## <a name="relationships"></a>Relações
Nenhuma

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.zebraFotaDeploymentStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.zebraFotaDeploymentStatus",
  "state": "String",
  "totalDevices": 1024,
  "totalCreated": 1024,
  "totalScheduled": 1024,
  "totalDownloading": 1024,
  "totalAwaitingInstall": 1024,
  "totalSucceededInstall": 1024,
  "totalCanceled": 1024,
  "totalUnknown": 1024,
  "totalFailedDownload": 1024,
  "totalFailedInstall": 1024,
  "completeOrCanceledDateTime": "String (timestamp)",
  "cancelRequested": true,
  "lastUpdatedDateTime": "String (timestamp)"
}
```




