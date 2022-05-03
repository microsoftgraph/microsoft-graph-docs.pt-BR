---
title: Visão geral da A Conexão de Dados do Microsoft Graph
description: A Conexão de Dados do Microsoft Graph traz informações do Microsoft 365 para o Microsoft Azure, que oferece acesso às melhores ferramentas de desenvolvimento e hospedagem para trabalhar com esses dados.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.custom: scenarios:getting-started
ms.openlocfilehash: f2275f5b2163c8b340fb4660d478d07338f11298
ms.sourcegitcommit: 267e3baf545c8dc71ba2ab69497e3ec369379f43
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/03/2022
ms.locfileid: "65176603"
---
# <a name="overview-of-microsoft-graph-data-connect"></a>Visão geral da A Conexão de Dados do Microsoft Graph

A Conexão de Dados do Microsoft Graph aumenta o modelo transacional do Microsoft Graph com uma maneira inteligente de acessar dados avançados em escala. Os dados abordam como os trabalhadores se comunicam, colaboram e gerenciam seu tempo em todos os aplicativos e serviços no Microsoft 365. 

Ideal para big data e aprendizado de máquina, o Data Connect permite que você desenvolva aplicativos para análise, inteligência e otimização de processos de negócios, estendendo os dados do Microsoft 365 para o Azure. Ao integrar desta maneira, você pode aproveitar o vasto conjunto de opções de computação e armazenamento no Azure, mantendo a conformidade com os padrões do setor e mantendo seus dados seguros.

![Uma imagem que mostra os controles de dados aplicados entre os dados do Microsoft 365 na nuvem do Azure, bem como os dados de saída.](images/data-connect-mgdc-capabilities.png)

A Conexão de Dados do Microsoft Graph usa o Azure Data Factory para copiar dados do Microsoft 365 para o armazenamento do seu aplicativo em intervalos configuráveis. Ele também fornece um conjunto de ferramentas para simplificar a entrega desses dados para o Microsoft Azure, permitindo que você acesse as ferramentas de desenvolvimento e hospedagem mais aplicáveis disponíveis. 

A Conexão de Dados também concede um modelo de controle e consentimento mais granular: você pode gerenciar dados, ver quem está acessando e solicitar propriedades específicas de uma entidade. Isso aprimora o modelo do Microsoft Graph, que concede ou nega acesso a aplicativos a entidades inteiras.

Você pode usar o Data Connect para habilitar cenários de aprendizado de máquina para sua organização. Nesses cenários, você pode criar aplicativos que fornecem informações valiosas para os participantes, treinamento de modelos de aprendizado de máquina e até mesmo executar previsões com base em grandes quantidades de dados adquiridos.</br>

<!--<iframe class="video-iframe" style="width: 960px; height: 540px;" frameborder="0" allowfullscreen="true" src="https://www.microsoft.com/en-us/videoplayer/embed/RWEJsy?autoplay=false"> </iframe>-->

> [!VIDEO https://www.microsoft.com/en-us/videoplayer/embed/RWEJsy?autoplay=false]

Você pode aproveitar o Microsoft Graph Data Connect se concordar com os [ Termos de Uso das APIs da Microsoft ](/legal/microsoft-apis/terms-of-use?context=/graph/context) e com a [Política de Privacidade da Microsoft](https://go.microsoft.com/fwlink/p/?LinkId=123161) e você estiver:

- Um ISV criando aplicativos inteligentes para todos os clientes do Microsoft 365.
- Um desenvolvedor corporativo criando aplicativos inteligentes para todos dentro da organização que acessam os dados do Microsoft 365.

## <a name="access-to-data-at-scale"></a>Acesso aos dados em escala

Aplicativos avançados precisam de acesso a grandes quantidades de dados, geralmente de vários usuários em sua organização ao mesmo tempo. Por esse motivo, o modelo de dados transacional padrão do Microsoft Graph tem uma tendência a limitar grandes conjuntos de dados. A entrega de dados requer uma infraestrutura complexa e milhares de chamadas de API, qualquer uma das quais pode ser limitada devido a limitações de recursos. 

O Microsoft Graph Data Connect resolve esse desafio acessando os dados em massa e copiando repetidamente os dados do Microsoft 365 para o seu aplicativo usando o Azure Data Factory. O Data Connect também permite que você escolha entre acessar os dados de todas as pessoas na sua organização ou apenas de grupos específicos de pessoas.

## <a name="granular-data-consent"></a>Consentimento granular de dados

No modelo de consentimento tradicional do Microsoft Graph, um administrador ou usuário só pode conceder ou negar a solicitação de um aplicativo para acessar conjuntos específicos e predefinidos de entidades. Por exemplo, uma solicitação de Mail.Read inclui acesso de leitura a um conjunto fixo de entidades que suportam emails do Outlook, incluindo [mensagens](/graph/api/resources/message) instâncias inteiras com todas as propriedades relevantes. 

A Conexão de Dados do Microsoft Graph permite um consentimento mais granular, permitindo que os aplicativos solicitem acesso a propriedades específicas em uma entidade ou filtre os dados nessas propriedades. Os administradores devem aprovar explicitamente antes que os dados do Microsoft Graph possam ser acessados. A solicitação deve especificar o nível de acesso solicitado, a aplicação da política de dados, o motivo da solicitação e o esquema dos dados solicitados. Como resultado, os aplicativos só podem utilizar dados essenciais para sua função, e qualquer conteúdo não relacionado será excluído. Por exemplo, um aplicativo pode consumir metadados de email, mas excluir o conteúdo do corpo e dos anexos.

## <a name="data-security-and-governance"></a>Segurança e governança de dados

A Microsoft está facilitando uma comunicação avançada e conectada entre a Conexão de Dados do Microsoft Graph e o Azure que respeita os dados do cliente. O Data Connect suporta todos os recursos de serviços nativos do Azure, como criptografia, delimitação geográfica, auditoria e imposição de políticas. 

Para minimizar a sobrecarga de gerenciamento de conformidade de aplicativos criados com o Data Connect, você pode especificar um conjunto de políticas detalhadas que pretende cumprir e que os administradores do Microsoft 365 podem examinar. Após o consentimento dessas políticas, a Microsoft monitora a adesão do aplicativo à política. Se um aplicativo viola (ou tenta violar) uma política estabelecida pela organização, a Microsoft interrompe o fluxo de dados para esse aplicativo.

## <a name="see-also"></a>Confira também

- [Crie seu primeiro aplicativo do Microsoft Graph Data Connect (tutorial)](data-connect-quickstart.yml)
- [Perguntas frequentes sobre a Conexão de Dados](data-connect-faq.md)
- [Conjuntos de dados, regiões e coletores](data-connect-datasets.md)
