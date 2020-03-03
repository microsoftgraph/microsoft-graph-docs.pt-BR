---
title: Visão geral dos registros de chamadas
description: Os registros de chamadas fornecem informações sobre as chamadas e reuniões que ocorrem em sua organização.
author: stephenjust
localization_priority: Normal
ms.prod: cloud-communications
ms.openlocfilehash: 4999f4b0d479b6e618055d39a3fecab340deb650
ms.sourcegitcommit: d3b6e4d11012e6b4c775afcec4fe5444e3a99bd3
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/03/2020
ms.locfileid: "42394635"
---
# <a name="call-records-overview"></a>Visão geral dos registros de chamadas

Os registros de chamadas fornecem informações de uso e diagnóstico sobre as chamadas e reuniões online que ocorrem em sua organização ao usar o Microsoft Teams ou o Skype for Business. Os dados de uso e diagnóstico podem ser consumidos para produzir relatórios personalizados para sua empresa para ajudar a monitorar a adoção ou solucionar problemas de qualidade de chamada.

As organizações podem assinar alterações em registros de chamadas usando o recurso de [assinaturas de webhook](/graph/api/resources/webhooks?view=graph-rest-beta) do Microsoft Graph, permitindo que eles criem relatórios quase em tempo real dos dados ou Alertem em determinados cenários, como chamadas de emergência.

> **Importante:** Use o critério ao conceder a permissão CallRecords. Read. All para aplicativos. Os registros de chamadas podem fornecer informações sobre a operação de sua empresa e, portanto, podem ser um alvo de atores mal-intencionados. Conceda essa permissão somente aos aplicativos em que você confia para atender aos seus requisitos de proteção de dados.

## <a name="subscribe-to-call-records"></a>Inscrever-se em registros de chamadas

As organizações e parceiros geralmente têm suas próprias ferramentas para gerar relatórios sobre chamadas e reuniões online. Usando WebHooks, eles podem receber um feed contínuo de registros de chamadas à medida que são criados. Esse modelo de push permite que as organizações e parceiros criem suas próprias soluções de relatórios em tempo real.

## <a name="look-up-a-call-record-by-its-call-id"></a>Pesquisar um registro de chamadas por ID de chamada

Os aplicativos podem recuperar um [registro de chamada](/graph/api/resources/callrecords-callrecord?view=graph-rest-beta) por sua ID. Essa ID pode ser determinada de uma notificação de webhook ou recuperada das ferramentas administrativas.

## <a name="see-also"></a>Confira também

- [Permissões de registros de chamadas](/graph/permissions-reference#call-records-permissions)
