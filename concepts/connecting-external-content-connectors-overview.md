---
title: Visão geral dos conectores do Microsoft Graph
description: Visão geral dos conectores do Microsoft Graph
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: d17c187ed45194c3f99572202d50c7339e70f730
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139307"
---
# <a name="microsoft-graph-connectors-overview"></a>Visão geral dos conectores do Microsoft Graph

O[Microsoft 365](https://www.microsoft.com/microsoft-365) é uma solução completa e inteligente que capacita usuários e organizações com experiências inovadoras de produtividade e abordagens enriquecedoras para aumentar a eficiência e gerar o crescimento dos negócios. O Microsoft Graph é o núcleo de dados que permite essas experiências inteligentes, e a API do Microsoft Graph fornece acesso a esses dados e inteligência.

Embora a maioria dos profissionais de informação gaste grande parte do seu tempo de trabalho em aplicativos de produtividade, como o [Microsoft 365](https://www.microsoft.com/microsoft-365), eles também precisam de uma maneira de integrar esse ambiente com os aplicativos corporativos e outros softwares e serviços de nuvem SaaS locais utilizados. Por exemplo, aplicativos de ERP (planejamento de recursos empresariais), CRM (gerenciamento de recursos do cliente), aplicativos de intranet, wikis, blogs e sites de redes sociais.

Os conectores do Microsoft Graph oferecem uma maneira simples e intuitiva de trazer conteúdo de serviços externos para o Microsoft Graph, habilitando dados externos para experiências inteligentes do Microsoft 365 como a Pesquisa da Microsoft (atualmente GA) e muitos outros em breve como Viva Topics.

Hoje, com os conectores do Microsoft Graph, os dados obtidos de sua organização podem aparecer nos resultados da Pesquisa da Microsoft. Esse recurso expande os tipos de fontes de conteúdo que podem ser pesquisadas nos aplicativos de produtividade do Microsoft 365 e no ecossistema da Microsoft mais amplo. Em breve, os conectores terão muitas outras experiências inteligentes do Microsoft 365.
O diagrama a seguir fornece uma visão geral de alto nível dos conectores do Microsoft Graph.

<!---Insert image reference here --->
<!---       ![Select the Microsoft Graph permissions](./images/application-saml-sso-configure-api/set-permissions.png) --->
![Imagem mostrando conectores sendo usados para trazer dados para o Microsoft Graph](./images/connectors-images/overview.png)

## <a name="build-your-own-custom-connector"></a>Criar seu próprio conector personalizado

Os mais de 100 conectores atualmente disponíveis na Microsoft e nos parceiros permitem que você se conecte aos serviços Microsoft e não-Microsoft populares. Exemplos de conectores existentes incluem os serviços Azure, Box, ServiceNow, Salesforce, serviços Google, MediaWiki, e muito mais.

Para saber mais sobre os conectores existentes do Microsoft Graph, visite a [galeria de conectores do Microsoft Graph](/microsoftsearch/connectors-gallery).

Embora esses conectores ajudem a se conectar aos serviços populares, talvez você queira integrar com serviços que não estão disponíveis na [galeria de conectores](/microsoftsearch/connectors-gallery) existente. Você pode usar a API de conectores do Microsoft Graph para criar conectores personalizados para trazer seus dados externos para experiências do Microsoft 365, incluindo a Pesquisa da Microsoft, Viva Topics e muito mais (em breve), dentro de sua organização.

## <a name="get-started-with-custom-graph-connectors"></a>Começar a trabalhar com conectores Graph personalizados:
* [Trabalhando com a API de conectores](connecting-external-content-connectors-api-overview.md)
* [Use o Postman com a API de conectores do Microsoft Graph](connecting-external-content-connectors-api-postman.md)
<!---**(Articles coming next)**
* [Build your first custom connector with Microsoft Graph]()
--->

