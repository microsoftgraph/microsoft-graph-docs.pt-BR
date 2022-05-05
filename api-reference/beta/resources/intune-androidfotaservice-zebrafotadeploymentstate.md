---
title: Tipo de enumeração zebraFotaDeploymentState
description: Representa o estado da implantação do Zebra FOTA.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5912f89249951db9ff4dd5a058169cb3b54113fc
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65213054"
---
# <a name="zebrafotadeploymentstate-enum-type"></a>Tipo de enumeração zebraFotaDeploymentState

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Representa o estado da implantação do Zebra FOTA.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|pendingCreation|0|A implantação foi criada, mas a Zebra não confirmou sua criação.|
|createFailed|1|A implantação não foi criada com êxito com a Zebra.|
|criadas|2|A implantação foi criada, mas ainda não foi implantada.|
|Inprogress|3|A implantação foi iniciada, mas não foi concluída.|
|Concluído|4|A implantação foi concluída ou a data de término foi aprovada.|
|pendingCancel|5|O administrador solicitou o cancelamento de uma implantação, mas a Zebra não confirmou o cancelamento.|
|Cancelado|6 |A implantação foi cancelada com êxito pela Zebra.|
|unknownFutureValue|99|Valor de enumeração futuro desconhecido.|




