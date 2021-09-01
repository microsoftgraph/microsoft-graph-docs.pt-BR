---
title: Trabalhar com a API de registros de chamadas no Microsoft Graph
description: A API de registros de chamadas do Microsoft Graph permite recuperar dados de uso e de diagnóstico das chamadas e reuniões on-line dentro da organização.
author: williamlooney
doc_type: conceptualPageType
ms.prod: cloud-communications
localization_priority: Priority
ms.openlocfilehash: 6af5d297c7a04b8c28321fed4cc106d2981ac0e4
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58799441"
---
# <a name="working-with-the-call-records-api-in-microsoft-graph"></a>Trabalhar com a API de registros de chamadas no Microsoft Graph

Os registros das chamadas fornecem informações de uso e diagnóstico das chamadas e reuniões on-line que ocorrem na sua organização ao usar o Microsoft Teams ou o Skype for Business. Você pode usar as APIs de registros de chamadas para se inscrever nos registros de chamadas e procurar registros de chamadas por IDs.

A API de registros de chamadas é definida no subnamespace OData, `microsoft.graph.callRecords`.

## <a name="key-resource-types"></a>Principais tipos de recursos

| Resource | Métodos |
| :-- | :-- |
| [callRecord](callrecords-callrecord.md) | [Obter callRecord](../api/callrecords-callrecord-get.md) |
| [sessão](callrecords-session.md) | [Obter callRecord](../api/callrecords-callrecord-get.md)<br />[Listar sessões](../api/callrecords-session-list.md) |
| [segmento](callrecords-segment.md) | [Obter callRecord](../api/callrecords-callrecord-get.md)<br />[Listar sessões](../api/callrecords-session-list.md) |
| [pstnCallLogRow](callrecords-pstncalllogrow.md)|[getPstnCalls](../api/callrecords-callrecord-getpstncalls.md) |
| [directRoutingLogRow](callrecords-directroutinglogrow.md) | [getDirectRoutingCalls](../api/callrecords-callrecord-getdirectroutingcalls.md)|

## <a name="call-record-structure"></a>Estrutura do registro de chamadas

A entidade [callRecord](callrecords-callrecord.md) representa uma única chamada ponto a ponto ou uma chamada de grupo entre vários participantes, às vezes chamada de reunião on-line.

Uma chamada ponto a ponto contém uma única [sessão](callrecords-session.md) entre os dois participantes da chamada. As chamadas de grupo contêm uma ou mais entidades de **sessão**. Em uma chamada de grupo, cada **sessão** fica entre o participante e um ponto de extremidade do serviço.

Cada **sessão** contém uma ou mais entidades do [segmento](callrecords-segment.md). Um **segmento** representa um link de mídia entre dois [pontos de extremidade](callrecords-endpoint.md). Para a maioria das chamadas, apenas um **segmento** estará presente em cada **sessão**. Entretanto, às vezes, poderá haver um ou mais **pontos de extremidade** intermediários.

![Imagem de uma estrutura de dados que representa um registro de chamada concluída](/graph/images/callrecords-structure.png)

No diagrama acima, o número denota quantas crianças de cada tipo podem estar presentes. Por exemplo: uma relação 1..N entre um **callRecord** e uma **sessão** significa que uma instância **callRecord** pode conter uma ou mais instâncias da **sessão**. Da mesma forma, uma relação 1..N entre um **segmento** e uma **mídia** significa que uma instância do **segmento** pode conter um ou mais fluxos de [mídia](callrecords-media.md).

## <a name="see-also"></a>Também consulte

- [Assinaturas do Webhook](/graph/api/resources/webhooks?view=graph-rest-1.0&preserve-view=true)

