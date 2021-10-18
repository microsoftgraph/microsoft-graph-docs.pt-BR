---
title: Usar a API de solicitação Graph direitos de assunto da Microsoft
description: A API Microsoft 365 de solicitação de direitos de entidade fornece funcionalidade para que as organizações automatizem tarefas repetitivas e se integrem às ferramentas de solicitação de direitos de entidade existentes para criar fluxos de trabalho repetidos que podem ajudar a atender aos regulamentos do setor.
ms.localizationpriority: medium
author: skadam-msft
ms.prod: compliance
doc_type: conceptualPageType
ms.openlocfilehash: 0f31c5358142e5a88ee8474bc9cb681eebcb529d
ms.sourcegitcommit: cd8611227a84db21449ab0ad40bedb665dacb9bb
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/18/2021
ms.locfileid: "60450127"
---
# <a name="use-the-microsoft-graph-subject-rights-request-api"></a>Usar a API de solicitação Graph direitos de assunto da Microsoft

De acordo com determinados regulamentos de privacidade em todo o mundo, os indivíduos podem fazer solicitações para revisar ou gerenciar os dados pessoais sobre si mesmos coletados pelas empresas. Essas solicitações são conhecidas como solicitações de direitos de assunto na solução Microsoft 365 gerenciamento de privacidade; às vezes, eles também são chamados de DSRs (solicitações de assunto de dados) ou DSARs (solicitações de acesso a dados). Microsoft 365 gerenciamento de privacidade capacita a equipe responsável por atender às solicitações de direitos de entidade para identificar facilmente os titulares de dados e encontrar suas informações pessoais entre os dados de uma organização em Exchange, SharePoint, OneDrive e Teams. 

As APIs do Microsoft Graph para solicitação de direitos de entidade fornecem funcionalidade para que as organizações automatizem tarefas repetitivas e se integrem às ferramentas de solicitação de entidades de dados existentes, para habilitar a criação de fluxos de trabalho repetidos que podem ser incorporados aos processos de negócios. Você pode usar as APIs de solicitação de direitos de assunto para ajudá-lo a automatizar e dimensionar a capacidade da sua organização de executar pesquisas de solicitações de direitos de assunto em Microsoft 365 e ajudar a atender aos regulamentos do setor com mais eficiência.

> [!IMPORTANT]
> As APIs do Microsoft Graph para solicitação de direitos de assunto destinam-se a ajudar a atender à necessidade de atender às solicitações de direitos de assunto nos serviços Microsoft 365 Exchange Online, SharePoint Online, chats Teams e OneDrive for Business. Essas APIs não devem ser usadas como um substituto para pesquisar dados em qualquer outro sistema Microsoft 365 ou em qualquer outra área, pois esses cenários não são explicitamente suportados.

A API inclui as seguintes entidades principais.

| Nome | Tipo       | Caso de uso |
|:-|:-|:-|
| Solicitação de direitos de assunto | [microsoft.graph.subjectRightsRequest](subjectRightsRequest.md) | Representa uma solicitação formal de um dado sujeito a um controlador para tomar uma ação em seus dados pessoais. |
| Assunto de dados | [microsoft.graph.datasubject](datasubject.md) | Contém informações relacionadas ao assunto de uma pesquisa de conteúdo. |
| Histórico de solicitações de direitos de assunto | [microsoft.graph.subjectRightsRequesthistory](subjectRightsRequesthistory.md) | Representa o histórico de uma solicitação de direitos de assunto. |
| Detalhes da solicitação de direitos de assunto | [microsoft.graph.subjectRightsRequestDetail](subjectRightsRequestDetail.md) | Representa os detalhes de uma solicitação de direitos de assunto, incluindo o número de itens encontrados, o número de itens revisados e assim por diante. |
| Detalhes do estágio de solicitação de direitos de assunto | [microsoft.graph.subjectRightsRequestStageDetail](subjectRightsRequestStageDetail.md) | Representa as propriedades dos estágios de uma solicitação de direitos de assunto. |

>[!IMPORTANT]
>As permissões de API de solicitação de direitos de assunto não estão disponíveis no momento. Para mais detalhes, confira [Problemas conhecidos](/graph/known-issues#compliance).

