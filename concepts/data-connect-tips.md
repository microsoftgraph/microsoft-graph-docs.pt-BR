---
title: Dicas para uso do Microsoft Graph Data Connect
description: Veja dicas de como aproveitar o Microsoft Graph Data Connect.
author: tlenig
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 7c887cf6a6407937c49d4e90b0c73800b13bee57
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629877"
---
# <a name="tips-for-using-microsoft-graph-data-connect"></a>Dicas para uso do Microsoft Graph Data Connect

Microsoft Graph Data Connect permite que desenvolvedores criem aplicativos que os clientes podem fornecer acesso gerenciado aos seus conjuntos de dados em escala do Microsoft Graph. Este artigo fornece dicas para ajudar você a aproveitar os recursos do Data Connect. Para obter uma introdução ao Microsoft Graph Data Connect, consulte o artigo [Visão geral](data-connect-concept-overview.md).

## <a name="is-microsoft-graph-data-connect-right-for-you"></a>O Microsoft Graph Data Connect é o certo para você?

Data Connect e as APIs do Microsoft Graph fornecem acesso para os mesmos dados subjacentes, mas de formas muito diferentes. Data Connect foi desenvolvido para extrair grandes quantidades de dados em massa, enquanto as APIs do Microsoft Graph são mais adequadas para acessar conjuntos de dados específicos em tempo real. Em alguns casos, ainda pode fazer sentido combiná-los. Por exemplo, convém usar o Data Connect para fazer uma extração inicial de dados de email do último ano e depois usar as APIs do Microsoft Graph para analisar emails em tempo real em diante. Data Connect e as APIs do Microsoft Graph são ferramentas diferentes para tarefas diferentes. É importante pensar sobre o qual método de acesso melhor se encaixa em seu cenário.

## <a name="expect-an-initial-overhead"></a>Espere uma sobrecarga inicial

Como o Data Connect é projetado para extrair grandes quantidades de dados em massa, alguma sobrecarga é incorrida antes que os dados possam ser extraídos. Essa sobrecarga é de aproximadamente 45 minutos, ou seja, todos os pipelines levarão no mínimo esse tempo, independentemente do tamanho dos dados. Isso pode ser um custo insignificante para grandes quantidades de dados, mas se for inaceitável para seu cenário, as APIs do Microsoft Graph podem fornecer uma melhor abordagem.

## <a name="data-must-stay-within-the-organizations-subscription"></a>Os dados devem ficar dentro da assinatura da organização

Os pipelines do Data Connect são organizados pelo Azure Data Factory, um serviço de integração de dados executado em uma assinatura do Azure. A assinatura do Azure está [associada a exatamente um locatário do Office 365](https://docs.microsoft.com/pt-BR/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory). Dessa forma, os dados devem ter o fluxo associado inicialmente a uma assinatura do Azure. Depois de mais minimalização e agregação, os dados podem ser usados em outro lugar.

Se você quiser desenvolver um aplicativo para outras pessoas usarem para extrair os dados do Office 365, você pode compactar o aplicativo como um [aplicativo gerenciado do Azure](https://docs.microsoft.com/pt-BR/azure/managed-applications/overview) e publicar no Azure Marketplace. Em seguida, alguém pode implantar o aplicativo em sua própria assinatura do Azure, e o aplicativo pode acessar dados em seu locatário. 

## <a name="use-of-service-principals"></a>Uso de entidades de serviço

Ao criar o pipeline do Data Factory, você terá que fornecer uma entidade de serviço para o serviço vinculado do Office 365. No Azure, uma entidade de serviço é uma identidade de segurança que representa um aplicativo ou serviço (e não um usuário). O Data Connect usa essa entidade de serviço como sua identidade ao receber acesso autorizado aos seus dados do Office 365.
Se você criar um Aplicativo Gerenciado do Azure para que outras pessoas usem em seus locatários, você ainda irá fornecer uma entidade de serviço para uso do aplicativo. A entidade de serviço ficará armazenado em seu locatário (do fornecedor). No entanto, se o aplicativo precisa de outras entidades de serviço, seu cliente (instalador) irá criá-las em seu próprio locatário. Por exemplo, seu pipeline do Data Factory provavelmente precisará de acesso a um recurso de armazenamento no Azure. O cliente criaria a entidade de serviço com permissões para a conta de armazenamento para uso do pipeline.

## <a name="check-for-pending-privileged-access-management-requests"></a>Procure por solicitações pendentes do Privileged Access Management

Antes que o Data Connect possa copiar seus dados, um administrador deve aprovar uma solicitação de Privileged Access Management (PAM). PAM é o mecanismo que autorizava seu acesso a dados de pipeline aos dados no Office 365. Na primeira vez que acionar um pipeline, irá esperar a aprovação da solicitação de acesso de um administrador do Office 365 (ou representante indicado). Embora o status do pipeline mostra **Em andamento**, a atividade de cópia subjacente terá o status **ConsentimentoPendente** até que o acesso seja aprovado, conforme mostrado na captura de tela a seguir.

![Captura de tela do painel de status da execução de pipeline com um status ConsentimentoPendente](images/data-connect-tips.png)

Durante o desenvolvimento, é uma boa ideia para garantir que a execução do seu pipeline não fique preso em **ConsentimentoPendente**, especialmente após alterar seu pipeline. Por exemplo, se você inserir um campo adicional no esquema, a próxima execução de pipeline emitirá uma nova solicitação de PAM que precisa ser aprovada. Não desperdice tempo esperando um pipeline que aguarda sua aprovação.

## <a name="approve-pam-requests-via-office-365-admin-portal"></a>Aprove solicitações PAM através do portal de administração do Office 365

A documentação do Data Connect mostra como usar o PowerShell e UX do PAM para aprovar solicitações PAM. Para aprovar usando UX do PAM, acesse a interface PAM no [portal de administração do Office 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/Settings/PrivilegedAccess). O portal fornece uma maneira simples e fácil para exibir, aprovar, negar, revogar solicitações PAM. Você encontra um link para ele no suplemento do Microsoft Graph Data Connect em **Configurações** > **Serviços e Suplementos** > **Microsoft Graph Data Connect**.

## <a name="use-a-second-user-to-approve-pam-requests"></a>Usar um segundo usuário para aprovar as solicitações PAM

Quando você executa um pipeline e aciona uma solicitação PAM, a solicitação é anexada à conta de usuário que é o proprietário de entidade de serviço usada pelo pipeline. Mas mesmo se essa conta for parte do grupo aprovador que você definiu, você não pode usá-la para aprovar a solicitação PAM porque autoaprovações não são permitidas. Se você tentar, receberá uma mensagem de erro no portal PAM: "Solicitante e aprovador são iguais. Não é permitida autoaprovação.” Para o desenvolvimento, convém ter uma segunda conta, além da de administrador que aprova as solicitações. O solicitante e o aprovador devem ter contas ativas do Exchange Online.

## <a name="deduplicate-emails-when-needed"></a>Elimine a duplicação de emails quando necessário

Quando você extrair emails do conjunto de dados `Message`, geralmente haverá vários objetos JSON para o mesmo email. Essas duplicatas existem quando um email é enviado para várias pessoas, há uma cópia do email na caixa de correio de cada destinatário. Como o conjunto de dados é extraído de cada caixa de correio, haverá todas as cópias entre os usuários. Em alguns cenários, talvez seja necessário manter cada cópia, mas em outros talvez você queira remover as duplicatas.
Você pode eliminar as duplicatas dos objetos JSON exportados baseados em `internetMessageId` das mensagens: duas mensagens com o mesmo `internetMessageId` são cópias duplicadas da mesma instância. Como as duplicatas podem existir em diferentes blobs, você deve eliminar as duplicatas em todos os blobs em vez de fazer isso em cada blob separadamente.

## <a name="use-puser-field-to-determine-the-relevant-user"></a>Use o campo puser para determinar o usuário relevante

Os dados extraídos incluem algumas propriedades meta que não existem se forem usadas as APIs correspondentes do Microsoft Graph. Especificamente, o campo `puser` pode ser útil para determinar de quais usuários os dados foram extraídos. No cenário em que você tem duas cópias do mesmo email em caixas de correio diferentes, você pode usar o campo `puser` para determinar as caixas de correio de origem das cópias.
O campo  também é útil para conjuntos de dados, como o conjunto de dados `Manager`. JSON exportado inclui informações sobre um gerenciador, mas isso é útil apenas se você souber o que gerenciam. O campo `puser` indicará qual gerenciador corresponde ao objeto JSON.

## <a name="next-steps"></a>Próximos passos

Consulte [UserVoice](https://microsoftgraph.uservoice.com/forums/920506-microsoft-graph-feature-requests?category_id=359581) para solicitações de recursos. 
