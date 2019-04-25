---
title: Diretrizes de limitação do Microsoft Graph
description: Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.
author: piotrci
localization_priority: Priority
ms.openlocfilehash: 8b3b8c5b0ec5a5209ad96f87dc677f4331c24e0b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32580978"
---
# <a name="microsoft-graph-throttling-guidance"></a>Diretrizes de limitação do Microsoft Graph


Os limites de controle limitam número de chamadas simultâneas para um serviço para evitar a utilização exagerada dos recursos. O Microsoft Graph foi projetado para lidar com um alto volume de solicitações. Se ocorrer um número impressionante de solicitações, a limitação ajuda a manter um desempenho ideal e a confiabilidade do serviço Microsoft Graph.

Os limites de controle variam de acordo com o cenário. Por exemplo, se você estiver executando um grande volume de gravações, a possibilidade de limitação é mais alta do que se você estiver realizando apenas leituras.

## <a name="what-happens-when-throttling-occurs"></a>O que acontece quando a limitação ocorre?

Quando um limite de controle é excedido, o Microsoft Graph limitas quaisquer outras solicitações desse cliente por um período. Quando a limitação acontece, o Microsoft Graph retorna o código de status HTTP 429 (solicitações demais) e as solicitações falham. Um tempo de espera sugerido é retornado no cabeçalho da resposta da solicitação com falha. O comportamento de limitação pode depender do tipo e do número de solicitações. Por exemplo, se você tiver um grande volume de solicitações, todos os tipos de solicitação são limitados. Os limites de controle variam com base no tipo de solicitação. Portanto, você pode encontrar um cenário onde as gravações são limitadas, mas leituras ainda são permitidas. 

## <a name="common-throttling-scenarios"></a>Cenários comuns de limitação

As causas mais comuns de limitação dos clientes incluem:

* Um grande número de solicitações em todos os aplicativos em um locatário.
* Um grande número de solicitações de um aplicativo específico entre todos os locatários.

## <a name="best-practices-to-handle-throttling"></a>Práticas recomendadas para lidar com a limitação

Estas são as práticas recomendadas para lidar com a limitação:

* Reduza o número de operações por solicitação.
* Reduza a frequência de chamadas.
* Evite novas tentativas imediatas, pois todas as solicitações se acumulam em relação aos seus limites de uso.

Quando você implementa a manipulação de erro, use o código de erro HTTP 429 para detectar a limitação. A resposta com falha inclui o campo *Retry-After* no cabeçalho de resposta. Desativar solicitações usando o atraso *Retry-After* é a forma mais rápida de se recuperar da limitação, já que o Microsoft Graph continua a registrar a utilização de recursos enquanto o cliente continua limitado.

1. Aguarde o número de segundos especificado no campo *Retry-After*.
2. Repita a solicitação.
3. Se a solicitação falhar novamente com um código de erro 429, você ainda estará limitado. Continue a usar o atraso Retry-After recomendado e repita a solicitação até obter êxito.

Atualmente, os seguintes recursos oferecem atualmente um cabeçalho retry-after:
- [Usuário](/graph/api/resources/user?view=graph-rest-1.0)
- [Foto](/graph/api/resources/profilephoto?view=graph-rest-1.0)
- [Email](/graph/api/resources/message?view=graph-rest-1.0)
- [Calendário (usuários e grupos)](/graph/api/resources/event?view=graph-rest-1.0)
- [Contato](/graph/api/resources/contact?view=graph-rest-1.0)
- [Anexo](/graph/api/resources/attachment?view=graph-rest-1.0)
- [Conversas em grupo](/graph/api/resources/conversation?view=graph-rest-1.0)
- [Pessoas e social](/graph/api/resources/social-overview?view=graph-rest-beta)
- [Drive (OneDrive)](/graph/api/resources/drive?view=graph-rest-1.0)

Para ter uma discussão mais ampla sobre a limitação no Microsoft Cloud, veja [Padrão de Limitação](https://msdn.microsoft.com/library/office/dn589798.aspx).
