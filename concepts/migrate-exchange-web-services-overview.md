---
title: Migrar Exchange aplicativos EWS (Serviços Web) para o Microsoft Graph
description: Descreve como migrar aplicativos Exchange EWS (Serviços Web) para o Microsoft Graph.
author: sumithra-maran
ms.localizationpriority: medium
ms.prod: exchange
doc_type: conceptualPageType
ms.openlocfilehash: dcc9d75e82fa2a6b09298a8b5068f2c55e2a8be4
ms.sourcegitcommit: 562dc670cea411de0ecc232840ce1c650abbe34c
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/19/2022
ms.locfileid: "65549600"
---
# <a name="migrate-exchange-web-services-ews-apps-to-microsoft-graph"></a>Migrar Exchange aplicativos EWS (Serviços Web) para o Microsoft Graph

[Exchange Serviços Web (EWS)](/exchange/client-developer/exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange) é um protocolo herdado que está em uso desde Exchange Server 2007. Em agosto de 2018, a [Microsoft](https://techcommunity.microsoft.com/t5/exchange-team-blog/upcoming-changes-to-exchange-web-services-ews-api-for-office-365/ba-p/608055) anunciou que não haverá nenhum investimento ativo em APIs do EWS para Exchange Online. É altamente recomendável migrar seus aplicativos EWS que acessam Exchange Online para o Microsoft Graph.

## <a name="why-use-microsoft-graph"></a>Por que usar o Microsoft Graph?

O Microsoft Graph oferece melhorias em relação ao EWS em termos de segurança, simplicidade e eficiência. Alterne para o Microsoft Graph para aproveitar essas melhorias, tudo por meio de um único ponto de extremidade.

### <a name="security"></a>Segurança

O Microsoft Graph tem políticas de segurança e governança mais estritas com o OAuth e escopo [granular](/graph/permissions-reference) para limitar o acesso a dados em uma caixa de correio em vez do modelo de acesso todo ou nenhum no EWS.

### <a name="developer-simplicity"></a>Simplicidade do desenvolvedor

O Microsoft Graph oferece [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para descobrir e testar APIs de maneira fácil e rápida, [SDKs](/graph/sdks/sdks-overview) em diferentes linguagens de programação e uma comunidade de desenvolvedores ativa.

### <a name="rest-efficiency"></a>Eficiência rest

As APIs Graph Microsoft são baseadas em REST, em que as APIs do EWS são baseadas em SOAP. A vantagem de usar protocolos baseados em REST incluem serialização JSON mais rápida e menor uso de rede.

## <a name="next-steps"></a>Próximas etapas

- Saiba mais [sobre as diferenças de](migrate-exchange-web-services-authentication.md) autenticação no Microsoft Graph e no EWS.
- Examine [os mapeamentos de](migrate-exchange-web-services-api-mapping.md) API para localizar Graph Microsoft para as APIs do EWS que você usa no momento.
- Explore [os conceitos e](/graph/overview) as práticas Graph Microsoft.
- Use [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) para experimentar com o Microsoft Graph.
