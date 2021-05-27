---
title: Perguntas frequentes sobre a Conexão de Dados do Microsoft Graph
description: Obtenha dicas que o ajudarão a aproveitar as vantagens da Conexão de Dados do Microsoft Graph.
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: dbc0b7776d769ee694d9022b1e7f5b838f014da6
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/27/2021
ms.locfileid: "52680077"
---
# <a name="microsoft-graph-data-connect-frequently-asked-questions"></a>Perguntas frequentes sobre a Conexão de Dados do Microsoft Graph

A Conexão de Dados do Microsoft Graph permite que os desenvolvedores criem aplicativos que os clientes podem fornecer acesso gerenciado a seus conjuntos de dados em escala do Microsoft Graph. Este artigo fornece dicas que o ajudarão a tirar proveito dos recurso da Conexão de Dados. Para obter uma introdução a Conexão de Dados do Microsoft Graph, consulte o artigo [Visão geral](data-connect-concept-overview.md).

## <a name="is-microsoft-graph-data-connect-right-for-me"></a>A Conexão de Dados do Microsoft Graph é adequada para mim?

A Conexão de Dados e as APIs do Microsoft Graph fornecem acesso aos mesmos dados subjacentes, mas de formas muito diferentes. A Conexão de Dados foi projetada para extrair grandes quantidades de dados em massa, enquanto as APIs do Microsoft Graph são mais adequadas para acessar conjuntos específicos de dados em tempo real. Em alguns casos, ainda pode fazer sentido combiná-los. Por exemplo, você pode querer usar a Conexão de Dados para fazer uma extração inicial dos dados de email do último ano e, em seguida, usar as APIs do Microsoft Graph para analisar emails em tempo real daqui para frente. A Conexão de Dados e as APIs do Microsoft Graph são ferramentas diferentes para trabalhos diferentes. É importante pensar sobre o qual método de acesso melhor se encaixa em seu cenário.

## <a name="will-there-be-any-initial-overhead"></a>Haverá alguma sobrecarga inicial?

Como o Data Connect foi projetado para extrair grandes quantidades de dados em massa, ocorre alguma sobrecarga antes que os dados possam ser extraídos. Essa sobrecarga é de aproximadamente 45 minutos, ou seja, todos os pipelines levarão no mínimo esse tempo, independentemente do tamanho dos dados. Isso pode ser um custo insignificante para grandes quantidades de dados, mas se for inaceitável para seu cenário, as APIs do Microsoft Graph podem fornecer uma melhor abordagem.

## <a name="how-much-do-i-have-to-pay-for-microsoft-graph-data-connect"></a>Quanto devo pagar pela Conexão de Dados do Microsoft Graph?

Os encargos de consumo da Conexão de Dados do Microsoft Graph são cobrados mensalmente com base no pagamento por uso. A unidade de faturamento da Conexão de Dados do Microsoft Graph está em vários de 1000 objetos, onde 1 objeto é mapeado para 1 instância individual de uma entidade no Microsoft 365. Por exemplo, 1 email == 1 objeto, 1 arquivo == 1 objeto, 1 Mensagem de chat do Teams == 1 objeto, e assim por diante. Os encargos são calculados usando uma taxa fixa com base na contagem de 1.000 objetos extraídos por meio do conector. Não há cobrança de extração de objetos dos seguintes conjuntos de dados:

- BasicDataSet_v0.User
- BasicDataSet_v0.MailboxSettings
- BasicDataSet_v0.Manager
- BasicDataSet_v0.DirectReport.

## <a name="is-it-possible-for-my-data-to-stay-within-the-organizations-subscription-with-microsoft-graph-data-connect"></a>É possível que meus dados permaneçam dentro da assinatura da organização com a Conexão de Dados do Microsoft Graph?

Os pipelines do Data Connect são organizados pelo Azure Data Factory, um serviço de integração de dados executado em uma assinatura do Azure. A assinatura do Azure está [associada a exatamente um locatário do Microsoft 365](/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory). Dessa forma, os dados devem ter o fluxo associado inicialmente a uma assinatura do Azure. Depois de mais minimalização e agregação, os dados podem ser usados em outro lugar.

Se você quiser desenvolver um aplicativo para outras pessoas usarem para extrair os dados do Microsoft 365, você pode compactar o aplicativo como um [aplicativo gerenciado do Azure](/azure/managed-applications/overview) e publicar no Azure Marketplace. Em seguida, alguém pode implantar o aplicativo em sua própria assinatura do Azure, e o aplicativo pode acessar dados em seu locatário.

## <a name="are-service-principals-required-with-microsoft-graph-data-connect"></a>As entidades de serviços são requeridas com a Conexão de Dados do Microsoft Graph?

Ao criar o pipeline do Data Factory, você terá que fornecer uma entidade de serviço para o serviço vinculado do Microsoft 365. No Azure, uma entidade de serviço é uma identidade de segurança que representa um aplicativo ou serviço (e não um usuário). O Data Connect usa essa entidade de serviço como sua identidade ao obter acesso autorizado aos dados do Microsoft 365.

Se você criar um Aplicativo Gerenciado do Azure para que outras pessoas usem em seus locatários, você ainda irá fornecer uma entidade de serviço para uso do aplicativo. A entidade de serviço ficará armazenado em seu locatário (do fornecedor). No entanto, se o aplicativo precisa de outras entidades de serviço, seu cliente (instalador) irá criá-las em seu próprio locatário. Por exemplo, seu pipeline do Data Factory provavelmente precisará de acesso a um recurso de armazenamento no Azure. O cliente criaria a entidade de serviço com permissões para a conta de armazenamento para uso do pipeline.

## <a name="how-can-i-check-for-pending-privileged-access-management-requests"></a>Como posso verificar se há solicitações pendentes de Gerenciamento de Acesso Privilegiado?

Antes que o Data Connect possa copiar seus dados, um administrador deve aprovar uma solicitação de Gerenciamento de Acesso Privilegiado (PAM). PAM é o mecanismo usado para autorizar seu acesso a dados de pipeline aos dados no Microsoft 365. Na primeira vez que acionar um pipeline, irá esperar a aprovação da solicitação de acesso de um administrador do Microsoft 365 (ou representante indicado). Embora o status do pipeline mostra **Em andamento**, a atividade de cópia subjacente terá o status **ConsentimentoPendente** até que o acesso seja aprovado, conforme mostrado na captura de tela a seguir.

![Captura de tela do painel de status da execução de pipeline com um status ConsentimentoPendente](images/data-connect-tips.png)

Durante o desenvolvimento, é uma boa ideia para garantir que a execução do seu pipeline não fique preso em **ConsentimentoPendente**, especialmente após alterar seu pipeline. Por exemplo, se você inserir um campo adicional no esquema, a próxima execução de pipeline emitirá uma nova solicitação de PAM que precisa ser aprovada. Não desperdice tempo esperando um pipeline que aguarda sua aprovação.

## <a name="how-can-i-approve-pam-requests-via-microsoft-365-admin-portal"></a>Como posso aprovar solicitações de PAM por meio do portal de administração do Microsoft 365?

A documentação da Conexão de Dados mostra como usar o PowerShell e o PAM UX para aprovar solicitações de PAM. Para aprovar usando a UX do PAM, acesse a interface PAM no [portal de administração do Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/Settings/PrivilegedAccess). O portal fornece uma maneira simples e fácil para exibir, aprovar, negar, revogar solicitações PAM. Você encontra um link para ele no suplemento de Conexão de Dados do Microsoft Graph em **Configurações** > **Serviços e Suplementos** > **Conexão de Dados do Microsoft Graph**.

## <a name="can-i-have-a-second-user-to-approve-pam-requests"></a>Posso ter um segundo usuário para aprovar solicitações de PAM?

Quando você executa um pipeline e aciona uma solicitação PAM, a solicitação é anexada à conta de usuário que é o proprietário de entidade de serviço usada pelo pipeline. Mas mesmo se essa conta for parte do grupo aprovador que você definiu, você não pode usá-la para aprovar a solicitação PAM porque autoaprovações não são permitidas. Se você tentar, receberá uma mensagem de erro no portal PAM: "Solicitante e aprovador são iguais. Não é permitida autoaprovação.” Para o desenvolvimento, convém ter uma segunda conta, além da de administrador que aprova as solicitações. O solicitante e o aprovador devem ter contas ativas do Exchange Online.

## <a name="can-i-deduplicate-emails-when-needed"></a>Posso eliminar a duplicação de emails quando necessário?

Quando você extrair emails do conjunto de dados `Message`, geralmente haverá vários objetos JSON para o mesmo email. Essas duplicatas existem quando um email é enviado para várias pessoas, há uma cópia do email na caixa de correio de cada destinatário. Como o conjunto de dados é extraído de cada caixa de correio, haverá todas as cópias entre os usuários. Em alguns cenários, talvez seja necessário manter cada cópia, mas em outros talvez você queira remover as duplicatas.
Você pode eliminar as duplicatas dos objetos JSON exportados baseados em `internetMessageId` das mensagens: duas mensagens com o mesmo `internetMessageId` são cópias duplicadas da mesma instância. Como as duplicatas podem existir em diferentes blobs, você deve eliminar as duplicatas em todos os blobs em vez de fazer isso em cada blob separadamente.

## <a name="can-i-use-puser-field-to-determine-the-relevant-user"></a>Posso usar o campo puser para determinar a relevância do usuário?

Os dados extraídos incluem algumas propriedades meta que não existem se forem usadas as APIs correspondentes do Microsoft Graph. Especificamente, o campo `puser` pode ser útil para determinar de quais usuários os dados foram extraídos. No cenário em que você tem duas cópias do mesmo email em caixas de correio diferentes, você pode usar o campo `puser` para determinar as caixas de correio de origem das cópias. O campo `puser` também é útil para conjuntos de dados, como o conjunto de dados `Manager`. JSON exportado inclui informações sobre um gerenciador, mas isso é útil apenas se você souber o que gerenciam. O campo `puser` indicará qual gerenciador corresponde ao objeto JSON.

## <a name="is-a-mix-of-users-with-and-without-workplace-analytics-licenses-supported"></a>Existe suporte para uma combinação de usuários com e sem licenças do Workplace Analytics?

Hoje, exigimos que todos os usuários na lista de usuários tenham a licença do Workplace Analytics ou que todos os usuários na lista de usuários não tenham licença do Workplace Analytics. Infelizmente, não temos suporte para listas mistas de usuários, ou seja, alguns usuários têm licença de análise do local de trabalho e outros não. Isto porque se os usuários na lista de usuários têm licença do Workplace Analytics, então não são necessários custos adicionais para a Conexão de Dados, enquanto que se os clientes não têm licença do Workplace Analytics, então os clientes são cobrados usando o faturamento de consumo detalhado aqui. Se isso está quebrando seu caso de uso hoje, informe-nos e podemos ver se há oportunidades para ajudar em seu cenário aqui.

## <a name="is-hybrid-mode-tenant-setup-supported"></a>A configuração do locatário no modo híbrido é compatível?

Se sua configuração do Microsoft 365 tiver alguns usuários no Exchange Online e alguns usuários no Exchange local, não haverá suporte para os usuários que estão no Exchange local. Infelizmente, hoje não há suporte para a Conexão de Dados para usuários locais do Exchange.

## <a name="are-resource-accounts-supported"></a>Há suporte para contas de recursos?

Atualmente não apoiamos o acesso a mensagens ou eventos a partir de contas de recursos. No futuro, teremos suporte para isso.

## <a name="i-am-seeing-multiple-files-per-adf-pipeline-run-but-sometimes-just-1-file-per-run-why-is-this-happening"></a>Estou vendo vários arquivos por execução de pipeline ADF, mas às vezes apenas 1 arquivo por execução. Por que isso está acontecendo?

A Conexão de Dados do Microsoft Graph leva a lista de usuários para cada execução de pipeline e, em seguida, distribui a extração e curadoria do conjunto de dados em vários trabalhos executados em paralelo. Para cada execução paralela, 1 arquivo de saída é gerado no coletor de dados definido por você. Para alguns casos, se a lista de usuários for pequena, eles podem ser mapeados em 1 trabalho de extração e curadoria e, nesses casos, apenas 1 arquivo de saída seria gerado no coletor de dados.

## <a name="how-is-billing-computed-with-the-count-of-objects-is-not-a-round-number"></a>Como a cobrança é calculada quando a contagem de objetos não é um número redondo?

Para fins de cobrança, a Conexão de Dados do Microsoft Graph arredonda para cima a contagem de objetos extraídos para o 1000 mais próximo. Por exemplo, se você extrair 125 objetos ou eles extraírem 999 objetos, serão cobrados 1000 objetos. Da mesma forma, se você extrair entre 1.001 a 2.000 objetos, será cobrado por 2.000 objetos.

## <a name="my-microsoft-365-copy-data-activity-is-always-failing-when-initialized-via-azure-synapse-why-is-this-happening"></a>Minha atividade de dados de cópia do Microsoft 365 está sempre falhando quando inicializada por meio do Azure Synapse. Por que isso está acontecendo?

Hoje, não temos suporte para atividade de cópia de dados do Microsoft 365 para ser inicializada pelo Azure Synapse. Estamos trabalhando para acrescentar a integração para a atividade Inicializada do Azure Synapse e atualizaremos nossa documentação quando esta for concluída.
