---
title: Tipo de enumeração operationApprovalRequestStatus
description: Status da Solicitação de Aprovação atual
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0068b5805ec8668e75a470b6d94ca16cdab2ca0e
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65210735"
---
# <a name="operationapprovalrequeststatus-enum-type"></a>Tipo de enumeração operationApprovalRequestStatus

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso em produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Status da Solicitação de Aprovação atual

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|desconhecido|0|Status Desconhecido|
|needsApproval|1|A solicitação de aprovação precisa de aprovação antes que a ação possa ser concluída.|
|Aprovado|2|Solicitação de aprovação aprovada, a ação agora pode ser concluída.|
|Rejeitado|3|Solicitação de aprovação rejeitada, ação não aprovada e nenhuma ação adicional pode ser tomada.|
|Cancelado|4|Solicitação de aprovação cancelada pelo usuário, não exigindo nenhuma ação adicional.|
|Concluído|5|Solicitação de aprovação concluída, não exigindo nenhuma ação adicional.|
|Expirado|6 |A solicitação de aprovação expirou, uma nova aprovação deve ser feita para concluir essa solicitação.|
|unknownFutureValue|99|Espaço reservado para futuros status de solicitação de aprovação da operação.|




