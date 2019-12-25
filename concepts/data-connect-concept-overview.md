---
title: Visão geral do Microsoft Graph Data Connect
description: O Microsoft Graph Data Connect traz os dados do Office 365 para o Microsoft Azure, que lhe oferece acesso às melhores ferramentas de desenvolvimento e hospedagem para trabalhar com esses dados.
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.custom: scenarios:getting-started
ms.openlocfilehash: adbc84b0d032c4c2cfb32d0c448bac5bfcae607f
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/25/2019
ms.locfileid: "40868020"
---
# <a name="overview-of-microsoft-graph-data-connect"></a>Visão geral do Microsoft Graph Data Connect
O Microsoft Graph contém dados avançados sobre funcionários e o seu local de trabalho, incluindo informações sobre como as pessoas trabalham e como elas se comunicam, colaboram e gerenciam seu tempo. O Microsoft Graph Data Connect oferece um conjunto de ferramentas para simplificar a entrega desses dados para o Microsoft Azure, que lhe oferece acesso às melhores ferramentas de desenvolvimento e hospedagem para trabalhar com esses dados. Isso permite que os clientes, enquanto mantêm total controle sobre seus dados do Microsoft Graph, se beneficiem de aplicativos inovadores ou específicos do setor que melhoram sua produtividade. A Microsoft está trazendo o controle mais seguro os clientes esperam.

## <a name="why-use-microsoft-graph-data-connect"></a>Por que usar o Microsoft Graph Data Connect?
Administradores do Office 365 precisam considerar cuidadosamente os desafios inerentes a migrar e gerenciar uma quantidade significativa de seus dados organizacionais. O Microsoft Graph Data Connect é projetado para proporcionar aos administradores novos controles sobre seus dados. Você pode usar esses dados para criar aplicativos que criam insights controlados por dados. 

### <a name="enable-granular-consent"></a>Habilitar o consentimento granular

No modelo de autorização do Microsoft Graph, um administrador ou usuário pode apenas conceder ou recusar uma solicitação de aplicativo para acessar conjuntos de entidades específicos e predefinidos. Por exemplo, uma solicitação de Mail.Read inclui acesso de leitura a um conjunto de entidades fixo que dá suporte ao Email do Outlook, incluindo instâncias de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) inteiras com todas as suas propriedades. Por outro lado, o Microsoft Graph Data Connect permite consentimento mais preciso, permitindo que os aplicativos solicitem acesso a propriedades específicas em uma entidade ou que filtrem os dados nessas propriedades. Os administradores precisam fornecer aprovação explícita para acessar dados do Microsoft Graph antes que o acesso seja permitido. A solicitação precisa especificar o nível de acesso solicitado e descrever a imposição da política de dados, o motivo da solicitação e o esquema dos dados solicitados. Como resultado, os aplicativos podem usar apenas os dados essenciais para a função desempenhada por eles, enquanto o conteúdo não relacionado é excluído. Por exemplo, um aplicativo pode consumir metadados de email, mas excluir o conteúdo do corpo e de anexos. 

### <a name="provide-data-governance"></a>Fornecer governança de dados
A Microsoft está facilitando comunicação avançada e conectada entre o Microsoft Graph e o Azure, com relação ao status dos dados dos clientes. Quando cria aplicativos por meio de dados do Microsoft Graph Data Connect, você pode especificar um conjunto de políticas detalhadas com as quais pretende manter a conformidade. Os administradores do Office 365 podem, em seguida, revisar e concordar com essas políticas. Essa prática minimiza sobrecarga de gerenciamento de conformidade. Quando o consentimento é fornecido, a Microsoft monitora a adesão do aplicativo à política. Se um aplicativo viola (ou tenta violar) uma política estabelecida pela organização, a Microsoft interrompe o fluxo de dados para esse aplicativo. 

### <a name="get-access-to-data-at-scale"></a>Obter acesso a dados em escala
Aplicativos avançados precisam de acesso a grandes quantidades de dados, geralmente de vários usuários em sua organização ao mesmo tempo. Com o modelo de dados transacionais tradicional, você precisa criar uma infraestrutura complexa e fazer milhares de chamadas à API para coordenar essa entrega de dados. Com apenas algumas etapas simples, o Microsoft Graph Data Connect usa a força do Azure Data Factory para entregar dados do Office 365 da sua organização para o aplicativo, em um cronograma que pode ser repetido.

## <a name="next-steps"></a>Próximas etapas
Para começar, veja [Introdução ao Microsoft Graph Data Connect](data-connect-get-started.md).
