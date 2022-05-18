---
title: Usar a API de solicitação Graph direitos de entidade do Microsoft Graph
description: A API de solicitação de direitos de entidade fornece funcionalidade para que as organizações automatizem tarefas repetitivas e se integrem às ferramentas de solicitação de direitos de entidade existentes para criar fluxos de trabalho repetíveis que podem ajudar a atender aos regulamentos do setor.
ms.localizationpriority: medium
author: skadam-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: b3c3507fa475ea77720535d5ccb91c3455d92d4f
ms.sourcegitcommit: 3240ab7eca16a0dde88a39079a89469710f45139
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/18/2022
ms.locfileid: "65461559"
---
# <a name="use-the-microsoft-graph-subject-rights-request-api"></a>Usar a API de solicitação Graph direitos de entidade do Microsoft Graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

De acordo com determinados regulamentos de privacidade em todo o mundo, os indivíduos podem fazer solicitações para revisar ou gerenciar os dados pessoais sobre si mesmos que as empresas coletaram. Essas solicitações são chamadas de solicitações de direitos de entidade na solução Microsoft Priva; às vezes, elas também são chamadas de DSRs (solicitações de titulares de dados) ou DSARs (solicitações de acesso do titular dos dados). Microsoft Priva capacita a equipe responsável por atender às solicitações de direitos de entidade para identificar facilmente os titulares dos dados e encontrar suas informações pessoais entre os dados de uma organização no Exchange, SharePoint, OneDrive e Teams. 

As APIs do Microsoft Graph para solicitação de direitos de entidade fornecem funcionalidade para que as organizações automatizem tarefas repetitivas e se integrem às ferramentas de solicitação de titulares de dados existentes para habilitar a criação de fluxos de trabalho repetíveis que podem ser incorporados aos seus processos de negócios. Você pode usar as APIs de solicitação de direitos de entidade para ajudá-lo a automatizar e dimensionar a capacidade da sua organização de executar pesquisas de solicitações de direitos de entidade no Microsoft 365 e ajudar a atender aos regulamentos do setor com mais eficiência.

> [!IMPORTANT]
> As APIs do Microsoft Graph para solicitação de direitos de entidade destinam-se a ajudar a atender à necessidade de atender às solicitações de direitos de entidade nos serviços Microsoft 365 para Exchange Online, SharePoint Online, chats Teams e OneDrive for Business. Essas APIs não devem ser usadas como um substituto para pesquisar dados em qualquer outro sistema Microsoft 365 ou em qualquer outra área, pois esses cenários não têm suporte explícito.

A API inclui as seguintes entidades principais.

| Nome | Tipo       | Caso de uso |
|:-|:-|:-|
| Solicitação de direitos do sujeito | [microsoft.graph.subjectRightsRequest](subjectRightsRequest.md) | Representa uma solicitação formal de um titular dos dados a um controlador para executar uma ação em seus dados pessoais. |
| Titular dos dados | [microsoft.graph.datasubject](datasubject.md) | Contém informações relacionadas ao assunto de uma pesquisa de conteúdo. |
| Histórico de solicitações de direitos de entidade | [microsoft.graph.subjectRightsRequesthistory](subjectRightsRequesthistory.md) | Representa o histórico de uma solicitação de direitos de entidade. |
| Detalhes da solicitação de direitos da entidade | [microsoft.graph.subjectRightsRequestDetail](subjectRightsRequestDetail.md) | Representa os detalhes de uma solicitação de direitos de entidade, incluindo o número de itens encontrados, o número de itens revisados e assim por diante. |
| Detalhes do estágio de solicitação de direitos de entidade | [microsoft.graph.subjectRightsRequestStageDetail](subjectRightsRequestStageDetail.md) | Representa as propriedades dos estágios de uma solicitação de direitos de entidade. |




