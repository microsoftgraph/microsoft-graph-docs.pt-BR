---
title: Visão geral dos dados do Microsoft Graph conectar (preview)
description: O Microsoft Graph contém dados avançados sobre trabalhadores e seu local de trabalho, incluindo informações sobre como as pessoas funcionam e como eles se comunicam, colaborar e gerenciar dedicação de tempo. Conexão de dados do Microsoft Graph traz esses dados para o Microsoft Azure, que fornece acesso para o desenvolvimento de práticas e ferramentas para trabalhar com esses dados de hospedagem. Isso permite que os clientes se beneficiam de aplicativos inovadores ou específico do setor que melhoram a sua produtividade, enquanto que elas mantenham controle total sobre seus dados do Microsoft Graph. Microsoft está trazendo ao longo de controle mais protegido que os clientes esperam.
ms.openlocfilehash: cce6046c9ed9b57171e998b1cb17c4e92fa0fcb5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091630"
---
# <a name="overview-of-microsoft-graph-data-connect-preview"></a>Visão geral dos dados do Microsoft Graph conectar (preview)
O Microsoft Graph contém dados avançados sobre trabalhadores e seu local de trabalho, incluindo informações sobre como as pessoas funcionam e como eles se comunicam, colaborar e gerenciar dedicação de tempo. Conexão de dados do Microsoft Graph traz esses dados para o Microsoft Azure, que fornece acesso para o desenvolvimento de práticas e ferramentas para trabalhar com esses dados de hospedagem. Isso permite que os clientes se beneficiam de aplicativos inovadores ou específico do setor que melhoram a sua produtividade, enquanto que elas mantenham controle total sobre seus dados do Microsoft Graph. Microsoft está trazendo ao longo de controle mais protegido que os clientes esperam.

## <a name="why-use-microsoft-graph-data-connect"></a>Por que o uso de dados do Microsoft Graph conectar?
Administradores do Office 365 devem considerar cuidadosamente os desafios inerentes movendo e gerenciando quantidades significativas de seus dados organizacionais. Conectar dados do Microsoft Graph foi projetado para proporcionar aos administradores novos controles sobre seus dados; Você pode usar esses dados para criar aplicativos que criam insights orientadas a dados. 

### <a name="enable-granular-consent"></a>Habilitar o consentimento granular

No modelo de consentimento do Microsoft Graph, um administrador ou usuário pode apenas conceder ou negar a solicitação de um aplicativo para acessar conjuntos específicos predefinidos de entidades. Por exemplo, uma solicitação para Mail.Read inclui o acesso de leitura para um conjunto fixo de entidades que oferecem suporte a email do Outlook, incluindo instâncias de toda a [mensagem](/graph/api/resources/message?view=graph-rest-1.0) com todas as suas propriedades. Por outro lado, conecte-se de dados do Microsoft Graph permite consentimento mais granular, permitindo que os aplicativos solicitar acesso a propriedades específicas em uma entidade ou filtrar os dados nessas propriedades. Os administradores devem dar a aprovação explícita para acessar dados do Microsoft Graph antes que o acesso seja concedido. A solicitação deve especificar o nível de acesso solicitado e descrevem a aplicação da política de dados, o motivo para a solicitação e o esquema dos dados solicitados. Como resultado, aplicativos podem usar somente os dados que é essenciais para as suas funções, e não relacionado conteúdo é excluído. Por exemplo, um aplicativo pode consumir cabeçalhos de email, mas excluir o conteúdo do corpo e anexos. 

### <a name="provide-data-governance"></a>Fornecer um governança de dados
A Microsoft está facilitando rica e conectada a comunicação entre Microsoft Graph e o Azure com relação o status dos dados dos clientes. Quando você crie aplicativos por meio de dados do Microsoft Graph se conectar, você pode especificar um conjunto de diretivas detalhadas que você pretende cumprirá. Administradores do Office 365 podem examinar e concorda com essas políticas. Essa prática minimiza a sobrecarga de gerenciamento de conformidade. Quando o consentimento for fornecido, o Microsoft monitora adesão do aplicativo à diretiva. Se um aplicativo viola (ou tentativas de violar) uma política estabelecida pela organização, o Microsoft interrompe o fluxo de dados ao aplicativo. 

### <a name="get-access-to-data-at-scale"></a>Obter acesso aos dados em escala
Aplicativos de rich exigem acesso a uma grande quantidade de dados, com frequência de muitos usuários em sua organização ao mesmo tempo. Com o modelo de dados transacionais tradicional, você precisa criar uma infra-estrutura complexa e tornar milhares de chamadas da API para orquestram este fornecimento de dados. Conexão de dados do Microsoft Graph usa o poder do alocador de dados do Windows Azure para enviar dados do Office 365 da sua organização para seu aplicativo, em um agendamento repetitivo, com apenas algumas etapas simples.

## <a name="api-reference"></a>Referência da API
Procurando a referência de API para esse serviço?

[Configurar](data-connect-get-started.md) Dados do Microsoft Graph conecte e consulte a [análise de uso Azure e dados do Office 365 para criar aplicativos inteligentes](https://github.com/OfficeDev/MS-Graph-Data-Connect/wiki).


## <a name="next-steps"></a>Próximas etapas
Para começar, consulte [Introdução ao conectar dados do Microsoft Graph](data-connect-get-started.md).
