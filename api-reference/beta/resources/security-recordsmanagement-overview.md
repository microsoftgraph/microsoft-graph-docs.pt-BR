---
title: Usar a API de gerenciamento de registros do Microsoft Graph
description: As APIs do Gerenciamento de Registros do Microsoft Purview ajudam as organizações a gerenciar a retenção e a exclusão de dados para atender às suas obrigações legais e regulamentos de conformidade e aumenta a eficiência, permitindo a disposição regular de itens que não precisam mais ser retidos.
ms.localizationpriority: medium
author: sseth-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: ffc809ecf368b6ca13d57ee6ffcd36ecd958a39a
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447489"
---
# <a name="use-the-microsoft-graph-records-management-apis"></a>Usar as APIs de gerenciamento de registros do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As APIs do Gerenciamento de Registros do Microsoft Purview ajudam as organizações a gerenciar a retenção e a exclusão de dados para atender às suas obrigações legais e regulamentos de conformidade e aumenta a eficiência, permitindo a disposição regular de itens que não precisam mais ser retidos.

A solução de gerenciamento de registros faz parte do centro de conformidade do Microsoft Purview.

## <a name="manage-retention-labels"></a>Gerenciar rótulos de retenção
Os administradores e desenvolvedores de gerenciamento de registros precisam manter sistemas de gerenciamento de registros com rótulos criados, atualizados e excluídos periodicamente.

Os desenvolvedores e administradores de conformidade podem usar as APIs de gerenciamento de registros para executar operações em rótulos de gerenciamento de registros para manter seus sistemas.

## <a name="trigger-events-for-an-existing-label"></a>Disparar eventos para um rótulo existente
Quando um funcionário sai de uma empresa, as informações são atualizadas no sistema de gerenciamento de RH. A partir da data de licença, os documentos confidenciais precisam ser retidos por um período de 7 anos. Esses documentos têm o rótulo `Employee_departure` aplicado.

Os desenvolvedores e administradores de conformidade podem usar APIs de gerenciamento de registros para ler o rótulo `Employee_departure` e pesquisar o tipo de evento associado `Event-employee_departure`.

Os administradores de conformidade podem usar APIs de gerenciamento de registros para criar um evento para o tipo de evento associado. O período de retenção para os documentos confidenciais começa após a criação desse evento.

## <a name="entities"></a>Entidades
A API de gerenciamento de registros inclui as seguintes entidades principais.

| Nome | Tipo       | Caso de uso |
|:-|:-|:-|
| Rótulo | [microsoft.graph.security.retentionLabel](../resources/security-retentionlabel.md) | Contém configurações de retenção e ações que podem ser aplicadas a um item no final de um período. |
| Evento de retenção | [microsoft.graph.security.retentionEvent](../resources/security-retentionevent.md) | Representa um gatilho para retenção baseada em evento, em que um período de retenção começa após o evento. |
| Tipo de evento de retenção | [microsoft.graph.security.retentionEventType](../resources/security-retentioneventtype.md) | Representa um único grupo para o mesmo tipo de eventos de retenção. |
