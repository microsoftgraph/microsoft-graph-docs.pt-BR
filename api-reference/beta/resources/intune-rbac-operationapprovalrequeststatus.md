---
title: tipo denum operationApprovalRequestStatus
description: Status da Solicitação de Aprovação atual
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 22053b80a983af725720aa5fe11e8e93176cea49
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/19/2021
ms.locfileid: "60494348"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>tipo denum operationApprovalRequestStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status da Solicitação de Aprovação atual

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Status Desconhecido|
|needsApproval|1|A solicitação de aprovação precisa de aprovação antes que a ação possa ser concluída.|
|aprovado|2|Solicitação de aprovação aprovada, a ação agora pode ser concluída.|
|rejected|3|Solicitação de aprovação rejeitada, ação não aprovada e nenhuma outra ação pode ser tomada.|
|cancelado|4 |Solicitação de aprovação cancelada pelo usuário, não exigindo mais nenhuma ação.|
|completed|5|Solicitação de aprovação concluída, não exigindo mais nenhuma ação.|
|expirado|6 |A solicitação de aprovação expirou, uma nova aprovação deve ser feita para concluir essa solicitação.|



