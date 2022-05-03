---
title: Visão geral dos conectores do Microsoft Graph
description: Os conectores do Microsoft Graph trazem conteúdos de serviços externos para o Microsoft Graph, permitindo que dados externos potencializem as experiências inteligentes do Microsoft 365.
author: mecampos
ms.localizationpriority: high
doc_type: conceptualPageType
ms.prod: search
ms.openlocfilehash: 0ca7c660a0c2db5ad83bda3253c2d330e390320e
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176630"
---
# <a name="microsoft-graph-connectors-overview"></a>Visão geral dos conectores do Microsoft Graph

O[Microsoft 365](https://www.microsoft.com/microsoft-365) é uma solução completa e inteligente que capacita usuários e organizações com experiências inovadoras de produtividade e abordagens enriquecedoras para aumentar a eficiência e gerar o crescimento dos negócios. O Microsoft Graph é o núcleo de dados que permite essas experiências inteligentes, e a API do Microsoft Graph fornece acesso a esses dados e inteligência.

Embora a maioria dos profissionais de informações passe grande parte do seu tempo de trabalho em aplicativos de produtividade, como o Microsoft 365, eles também precisam de uma maneira de integrar esse ambiente com os aplicativos empresariais e outros softwares e serviços de nuvem SaaS e locais que usam. Exemplos incluem aplicativos de planejamento de recursos da empresariais (ERP), aplicativos de gerenciamento de recursos do cliente (CRM), aplicativos de intranet, wikis, blogs e sites de redes sociais.

Os conectores do Microsoft Graph oferecem uma maneira intuitiva de trazer conteúdos de serviços externos para o Microsoft Graph, permitindo que dados externos potencializem experiências inteligentes do Microsoft 365, como a Pesquisa Microsoft (atualmente GA).

Hoje, com os conectores do Microsoft Graph, os dados obtidos de sua organização podem aparecer nos resultados da Pesquisa da Microsoft. Esse recurso expande os tipos de fontes de conteúdo que podem ser pesquisadas nos aplicativos de produtividade do Microsoft 365 e no ecossistema da Microsoft mais amplo. Em breve, os conectores irão potencializar muitas outras experiências inteligentes do Microsoft 365, como o Viva Topics.

O diagrama a seguir fornece uma visão geral de alto nível dos conectores do Microsoft Graph.

<!---Insert image reference here --->
<!---       ![Select the Microsoft Graph permissions](./images/application-saml-sso-configure-api/set-permissions.png) --->
![Imagem mostrando conectores sendo usados para trazer dados para o Microsoft Graph](./images/connectors-images/overview.png)

## <a name="get-started-with-custom-connectors"></a>Introdução aos conectores personalizados

Os mais de 100 conectores atualmente disponíveis na Microsoft e nos parceiros permitem que você se conecte aos serviços Microsoft e não-Microsoft populares. Exemplos de conectores existentes incluem os serviços do Azure, Box, ServiceNow, Salesforce, serviços do Google e MediaWiki.

Para saber mais sobre os conectores existentes do Microsoft Graph, visite a [galeria de conectores do Microsoft Graph](https://www.microsoft.com/microsoft-search/connectors/).

## <a name="build-a-custom-connector"></a>Criar um conector personalizado

Embora os conectores existentes ajudem a se conectar a serviços populares, convém se integrar a serviços que não estão disponíveis na galeria de conectores. Você pode usar a API de conectores do Microsoft Graph para criar conectores personalizados para trazer seus dados externos para as experiências do Microsoft 365 em sua organização.

Para começar, confira [Criar seu primeiro conector personalizado do Microsoft Graph ](connecting-external-content-build-quickstart.yml).

## <a name="next-steps"></a>Próximas etapas

* [Trabalhar com a API de conectores do Microsoft Graph ](connecting-external-content-connectors-api-overview.md)
* [Use o Postman com a API de conectores do Microsoft Graph](connecting-external-content-connectors-api-postman.md)