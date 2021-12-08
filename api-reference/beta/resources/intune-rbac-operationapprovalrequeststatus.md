---
title: tipo denum operationApprovalRequestStatus
description: Status da Solicitação de Aprovação atual
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b60e9071de452cdf42a8ef58246be77bdfd868a8
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/08/2021
ms.locfileid: "61342234"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>tipo denum operationApprovalRequestStatus

Namespace: microsoft.graph

> **Importante:** As GRAPH da Microsoft na versão /beta estão sujeitas a alterações; o uso de produção não é suportado.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status da Solicitação de Aprovação atual

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Status Desconhecido|
|needsApproval|1|A solicitação de aprovação precisa de aprovação antes que a ação possa ser concluída.|
|aprovado|2|Solicitação de aprovação aprovada, a ação agora pode ser concluída.|
|rejected|3|Solicitação de aprovação rejeitada, ação não aprovada e nenhuma outra ação pode ser tomada.|
|cancelado|4|Solicitação de aprovação cancelada pelo usuário, não exigindo mais nenhuma ação.|
|completed|5|Solicitação de aprovação concluída, não exigindo mais nenhuma ação.|
|expirado|6 |A solicitação de aprovação expirou, uma nova aprovação deve ser feita para concluir essa solicitação.|




