---
title: Visão geral da conexão de dados do Microsoft Graph
description: A conexão de dados do Microsoft Graph traz informações do Microsoft 365 para o Microsoft Azure, que oferece acesso às melhores ferramentas de desenvolvimento e hospedagem para trabalhar com esses dados.
author: ajacks-msft
localization_priority: Priority
ms.prod: data-connect
ms.custom: scenarios:getting-started
ms.openlocfilehash: 9f93d895213c37858cf19db2b36c1f467e92fda5
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897299"
---
# <a name="overview-of-microsoft-graph-data-connect"></a>Visão geral da conexão de dados do Microsoft Graph
O Microsoft Graph contém dados avançados sobre funcionários e o seu local de trabalho, incluindo informações sobre como as pessoas trabalham e como elas se comunicam, colaboram e gerenciam seu tempo. O Microsoft Graph Data Connect oferece um conjunto de ferramentas para simplificar a entrega desses dados para o Microsoft Azure, que lhe oferece acesso às melhores ferramentas de desenvolvimento e hospedagem para trabalhar com esses dados. Isso permite que os clientes, enquanto mantêm total controle sobre seus dados do Microsoft Graph, se beneficiem de aplicativos inovadores ou específicos do setor que melhoram sua produtividade. A Microsoft está trazendo o controle mais seguro os clientes esperam.

## <a name="why-use-microsoft-graph-data-connect"></a>Por que usar a conexão de dados do Microsoft Graph?
Os administradores do Microsoft 365 devem considerar cuidadosamente os desafios inerentes à movimentação e gerenciamento de quantidades significativas de seus dados organizacionais. A conexão de dados do Microsoft Graph é projetada para proporcionar aos administradores novos controles sobre seus dados. Você pode usar esses dados para criar aplicativos que criam insights controlados por dados. 

### <a name="enable-granular-consent"></a>Habilitar o consentimento granular

No modelo de autorização do Microsoft Graph, um administrador ou usuário pode apenas conceder ou recusar uma solicitação de aplicativo para acessar conjuntos de entidades específicos e predefinidos. Por exemplo, uma solicitação de Mail.Read inclui acesso de leitura a um conjunto de entidades fixo que dá suporte ao Email do Outlook, incluindo instâncias de [mensagem](/graph/api/resources/message?view=graph-rest-1.0) inteiras com todas as suas propriedades. Por outro lado, o Microsoft Graph Data Connect permite consentimento mais preciso, permitindo que os aplicativos solicitem acesso a propriedades específicas em uma entidade ou que filtrem os dados nessas propriedades. Os administradores precisam fornecer aprovação explícita para acessar dados do Microsoft Graph antes que o acesso seja permitido. A solicitação precisa especificar o nível de acesso solicitado e descrever a imposição da política de dados, o motivo da solicitação e o esquema dos dados solicitados. Como resultado, os aplicativos podem usar apenas os dados essenciais para a função desempenhada por eles, enquanto o conteúdo não relacionado é excluído. Por exemplo, um aplicativo pode consumir metadados de email, mas excluir o conteúdo do corpo e de anexos. 

### <a name="provide-data-governance"></a>Fornecer governança de dados
A Microsoft está facilitando comunicação avançada e conectada entre o Microsoft Graph e o Azure, com relação ao status dos dados dos clientes. Quando cria aplicativos por meio de dados da conexão de dados do Microsoft Graph, você pode especificar um conjunto de políticas detalhadas com as quais pretende manter a conformidade. Os administradores do Microsoft 365 podem então revisar e consentir com essas políticas. Essa prática minimiza sobrecarga de gerenciamento de conformidade. Quando o consentimento é fornecido, a Microsoft monitora a adesão do aplicativo à política. Se um aplicativo viola (ou tenta violar) uma política estabelecida pela organização, a Microsoft interrompe o fluxo de dados para esse aplicativo. 

### <a name="get-access-to-data-at-scale"></a>Obter acesso a dados em escala
Aplicativos avançados precisam de acesso a grandes quantidades de dados, geralmente de vários usuários em sua organização ao mesmo tempo. Com o modelo de dados transacionais tradicional, você precisa criar uma infraestrutura complexa e fazer milhares de chamadas à API para coordenar essa entrega de dados. A conexão de dados do Microsoft Graph usa o poder do Azure Data Factory para fornecer dados do Microsoft 365 da sua organização para o seu aplicativo, em uma programação repetível, com apenas algumas etapas simples.

## <a name="next-steps"></a>Próximos passos
Para começar, veja [Introdução ao Microsoft Graph Data Connect](data-connect-get-started.md).
