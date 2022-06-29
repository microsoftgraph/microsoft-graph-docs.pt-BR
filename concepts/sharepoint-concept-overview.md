---
title: Visão geral da API de conteúdo e sites do SharePoint
description: Use a API REST do SharePoint no Microsoft Graph para integrar soluções com sites e conteúdo do SharePoint nos quais os usuários colaboram e compartilham em uma organização.
ms.localizationpriority: high
ms.prod: sharepoint
ms.custom: scenarios:getting-started
ms.openlocfilehash: 90b8095505ea82f4874c2910fe98eacdd5065481
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66437566"
---
# <a name="sharepoint-sites-and-content-api-overview"></a>Visão geral da API de conteúdo e sites do SharePoint

O SharePoint é sua Intranet móvel e inteligente. Com o SharePoint, os usuários podem compartilhar e gerenciar conteúdo, conhecimentos e aplicativos para capacitar o trabalho em equipe, encontrar informações e colaborar em uma organização. Você pode usar a API REST do SharePoint no Microsoft Graph para integrar suas soluções a conteúdo e sites do SharePoint.

## <a name="why-integrate-with-sharepoint-sites-and-content"></a>Por que integrar com conteúdo e sites do SharePoint?

Sites do SharePoint possibilitam a comunicação e a colaboração em equipe. Os Grupos do Microsoft 365, o Microsoft Teams e os portais são baseados no SharePoint, portanto, você pode usar o Microsoft Graph para acessar dados onde quer que eles sejam mantidos. Use a API do SharePoint no Microsoft Graph para acessar:

- Sites de equipe que armazenam o conteúdo no qual os usuários colaboraram com seus colegas de trabalho.
- Sites e portais de comunicação em que os usuários publicam páginas de conteúdo avançado para compartilhar em toda a organização.

### <a name="unleash-your-data-with-sharepoint-lists"></a>Potencialize seus dados com listas do SharePoint

As [Listas][lista] são a base do armazenamento de dados no SharePoint.
[Criar listas][criar] para armazenar uma variedade de dados corporativos, desde uma simples lista de contatos de clientes até um aplicativo corporativo personalizado com o PowerApps.
Quando você usa [colunas][] para definir o esquema, o SharePoint pode proteger a integridade de seus dados e habilitar recursos avançados de indexação, consulta e pesquisa.

### <a name="bring-the-power-of-lists-to-your-teams-files"></a>Leve o poder de listas para os arquivos da sua equipe

O SharePoint armazena arquivos em um [tipo de lista][] especial chamado biblioteca de documentos.
Você pode usar a [API do OneDrive][] para trabalhar com uma biblioteca como uma [unidade][], ou a API do SharePoint para trabalhar com ela como uma [lista][].
Assim como com uma lista normal, você pode ampliar o esquema de uma Biblioteca de documentos para atender às suas necessidades de negócios com colunas personalizadas.

### <a name="light-up-your-app-with-your-users-sharepoint-intranet-data"></a>Aprimore seu aplicativo com os dados da Intranet do SharePoint de seus usuários

Com o Microsoft Graph, você pode exibir os dados mais importantes dos seus usuários no seu aplicativo.
Mantenha os dados atualizados ao [consultar][] a lista que armazena os dados dos seus usuários.
[Crie][] suas próprias listas para os usuários do seu aplicativo e permita que eles acessem seus dados em outras experiências do SharePoint ou mantenha os dados ocultos.

### <a name="use-microsoft-graph-to-extend-sharepoint"></a>Use o Microsoft Graph para aprimorar o SharePoint

Como uma plataforma, o SharePoint oferece vários modelos de extensão e integração:

- A [Estrutura do SharePoint][] fornece uma maneira de compilar Web Parts usando tecnologias do lado do cliente e ferramentas de código aberto que podem ser hospedadas em páginas do SharePoint.
- [Suplementos do SharePoint][] são extensões autônomas que podem ser adicionadas a um site do SharePoint sem a necessidade de um código personalizado em execução no servidor.

Quando seu aplicativo é executado em uma página do SharePoint, você pode usar o Microsoft Graph facilmente para acessar dados no Microsoft 365.

Para saber mais sobre esses modelos, acesse o [Centro de Desenvolvedores do SharePoint][] ou os [Documentos para Desenvolvedores do SharePoint][].

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [API do SharePoint no Microsoft Graph v1.0](/graph/api/resources/sharepoint)
- [API do SharePoint no Microsoft Graph beta](/graph/api/resources/sharepoint?view=graph-rest-beta&preserve-view=true)

## <a name="next-steps"></a>Próximas etapas

Comece a usar o SharePoint no Microsoft Graph aprendendo mais sobre como [trabalhar com sites](/graph/api/resources/sharepoint).

[list]: /graph/api/resources/list
[colunas]: /graph/api/resources/columndefinition
[tipo de lista]: /graph/api/resources/listinfo
[criar]: /graph/api/list-create
[consultar]: /graph/api/listitem-get
[unidade]: /graph/api/resources/drive
[API do OneDrive]: /graph/api/resources/onedrive
[Estrutura do SharePoint]: /sharepoint/dev/spfx/sharepoint-framework-overview
[Suplementos do SharePoint]: /sharepoint/dev/sp-add-ins/sharepoint-add-ins
[Centro de Desenvolvedores do SharePoint]: https://developer.microsoft.com/sharepoint
[Documentos para Desenvolvedores do SharePoint]: /sharepoint/dev/
[SharePoint]: /graph/api/resources/sharepoint
