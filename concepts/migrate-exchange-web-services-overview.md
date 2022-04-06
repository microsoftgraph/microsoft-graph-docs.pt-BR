---
title: Migrar Exchange aplicativos do Web Services (EWS) para o Microsoft Graph
description: Descreve como migrar aplicativos Exchange Web Services (EWS) para o Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: 029c27940ee98b9f6b9d9077e79dc704df143e9e
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/16/2022
ms.locfileid: "63516541"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>Migrar Exchange aplicativos do Web Services (EWS) para o Microsoft Graph

[Exchange Web Services (EWS)](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange) é um protocolo herdado que está em uso desde Exchange Server 2007. Em agosto de 2018, a [Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055) anunciava que não haverá nenhum investimento ativo em APIs EWS para Exchange Online. Recomendamos que você migre seus aplicativos EWS que acessam Exchange Online para o Microsoft Graph.

## <a name="why-use-microsoft-graph"></a>Por que usar o Microsoft Graph?

O Microsoft Graph oferece melhorias sobre o EWS em termos de segurança, simplicidade e eficiência. Alternar para a Microsoft Graph aproveitar essas melhorias, tudo por meio de um único ponto de extremidade.

### <a name="security"></a>Segurança

A Microsoft Graph tem políticas mais estritas de segurança e governança com o OAuth e o escoamento granular para limitar o acesso a dados em uma caixa de correio, em vez do modelo de acesso todo ou nenhum no EWS.

### <a name="developer-simplicity"></a>Simplicidade do desenvolvedor

O Microsoft Graph oferece [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para descobrir e testar APIs de forma fácil e rápida, SDKs em diferentes linguagens de programação e uma comunidade ativa de desenvolvedores.

### <a name="rest-efficiency"></a>Eficiência REST

As APIs Graph Microsoft são baseadas em REST, onde as APIs EWS são baseadas em SOAP. A vantagem de usar protocolos baseados em REST incluem serialização JSON mais rápida e menor uso de rede.

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de](migrate-exchange-web-services-authentication.md) autenticação no Microsoft Graph e EWS.
- Revise [mapeamentos de API](migrate-exchange-web-services-api-mapping.md) para encontrar Graph da Microsoft para as APIs EWS que você usa no momento.
- Explore [os Graph](/graph/overview) e práticas da Microsoft.
- Use [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para experimentar com o Microsoft Graph.
