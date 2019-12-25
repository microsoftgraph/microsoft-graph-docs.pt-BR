---
title: Limites de API de comunicação em nuvem no Microsoft Graph
description: Contém informações sobre os limites das APIs de comunicação em nuvem
author: ananmishr
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 0338c7b37a58da66aac75430234a4b1df56b07b1
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40871552"
---
# <a name="cloud-communication-api-limits-in-microsoft-graph"></a>Limites de API de comunicação em nuvem no Microsoft Graph

Este artigo descreve as limitações das APIs de comunicação em nuvem. Esses limites ajudam a garantir que a plataforma seja estável, confiável e segura. Observe que essas limitações estão sujeitas a alterações no futuro. 

>**Observação:** Quando o limite é atingido, tentar fazer mais solicitações de API resultará em um HTTP `429 Error`.

| API      | Limitações    |
| :------------- | :----------: |
|  Chamadas | 10.000 chamadas/mês e 100 chamadas simultâneas   |
| Reuniões   | 2000 reuniões/usuários por mês |
| Presença (visualização)   | 2 solicitações/segundo |

## <a name="see-also"></a>Confira também

- [Trabalhar com a API de comunicação](/graph/api/resources/communications-api-overview?view=graph-rest-beta)
