---
title: Integração do Microsoft Graph Data Connect com o PAM
description: A Conexão de Dados do Microsoft Graph depende do Privileged Access Management (PAM) para permitir que os administradores do Microsoft 365 aprovem solicitações de movimentação de dados.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 7326580a1fa5516c516ff949dace93c20a5930d2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094036"
---
# <a name="microsoft-graph-data-connect-integration-with-pam"></a>Integração do Microsoft Graph Data Connect com o PAM

A Conexão de Dados do Microsoft Graph depende do Privileged Access Management (PAM) para permitir que os administradores do Microsoft 365 aprovem solicitações de movimentação de dados. Os pipelines da Conexão de Dados devem ser aprovados por um membro do grupo aprovador de solicitação de acesso a dados especificado pelo administrador do Microsoft 365 durante a ativação. Para configurar o grupo aprovador, consulte [Configurar seu locatário Microsoft 365 e habilitar Conexão de Dados do Microsoft Graph](/graph/data-connect-quickstart?tabs=Microsoft365&tutorial-step=1).

Emails de solicitação de aprovação são enviados a todos os membros do grupo aprovador para notificá-los quando atividades de cópia solicitam acesso para extrair dados do Microsoft 365. Aprovadores podem aprovar ou negar essas solicitações, especificar um grupo de usuários que deve ser apagado dos dados extraídos ou revogar uma solicitação anteriormente aprovada. As aprovações são válidas por seis meses, sendo necessária uma aprovação por atividade de cópia no pipeline do Azure Data Factory.

Cada solicitação sempre inclui os seguintes detalhes sobre o conjunto de dados e os usuários sobre os quais os dados estão sendo extraídos:

* **Solicitante**: O usuário que solicitou o pipeline.
* **Duração**: se aprovada, por quanto tempo a aprovação persiste, que é sempre 4320 horas (6 meses).
* **Motivo**: motivo para a solicitação, normalmente "um aplicativo instalado para sua organização exige autorização para obter acesso aos dados do Office 365."
* **Solicitado em**: data e hora da solicitação.
* **ID da solicitação**: A ID da solicitação, usada para fins de aprovação.
* **TabelaDados**: O conjunto de dados a ser extraído (por exemplo, itens enviados).
* **Colunas**: A lista de colunas a ser extraída a partir da tabela de dados (por exemplo, DataHorárioEnviado).
* **GruposPermitidos**: o grupo ou grupos de usuários em relação a quem o pipeline está extraindo os dados. Se a lista de grupos estiver vazia, o pipeline está solicitando o acesso aos dados de todos os usuários no locatário.
* **Escopo de Pesquisa de Usuário**: o predicado usado para filtrar os usuários. Isso só se aplica se a solicitação for para todos os usuários no locatário. Se esta estiver vazia, nenhum filtro é aplicado.
* **UriSaída**: o caminho de saída no qual os dados extraídos serão armazenados.
* **IdLocatárioOrigem**: a ID do locatário cujos dados são extraídos.
* **IdentidadeInstalador**: a identidade do instalador do aplicativo.

Os campos a seguir na solicitação estão disponíveis apenas em alguns casos:

* **Nome do aplicativo** e **URI do Marketplace** (disponível somente para aplicativos instalados pelo Azure Marketplace).
* Links para a política de privacidade e termos de serviço do aplicativo (disponível somente se o aplicativo fornecer).
* As políticas de conformidade que o aplicativo impõe, como a criptografia de dados inativos no local de armazenamento de saída (disponível somente se o aplicativo fornecer e se o aplicativo foi instalado pelo Azure Marketplace).
* **Lista de negações** – o grupo de usuários que podem ter sido apagados dos dados extraídos. Esse campo está vazio como parte da solicitação de conjuntos de dados compatíveis com a depuração de privacidade de dados extraídos. Pode ser preenchido por um membro do grupo aprovador que autoriza a solicitação no momento da aprovação.

## <a name="approving-requests"></a>Aprovar solicitações

Os pipelines do Conector de Dados do Microsoft Graph devem ser aprovados por um membro de um grupo aprovador de solicitação de acesso a dados. Aprovadores podem aprovar, recusar ou revogar pipelines usando a experiência do usuário PAM ou o módulo do PowerShell do Exchange Online.

### <a name="approve-deny-and-revoke-requests-by-using-powershell"></a>Aprovar, negar e revogar solicitações usando o PowerShell

Faça o seguinte para interagir com uma solicitação usando o módulo do PowerShell do Exchange Online:

1. Instalar o módulo do Powershell do Microsoft Exchange Online. Para obter mais informações, confira [Conectar-se ao PowerShell do Exchange Online usando a autenticação de multifator](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).

2. Conectar-se ao PowerShell do Exchange Online usando a MFA (autenticação multifator). Para obter mais informações, confira [Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    > [!NOTE]
    > **Observação**: você não precisa habilitar a autenticação multifator para sua organização para usar estas etapas ao se conectar ao PowerShell do Exchange Online. Conexão MFA cria um token OAuth usado pelo PAM para assinar suas solicitações.

3. Entrar com sua conta. Você deve fazer parte do grupo aprovador de acesso a dados configurado para poder aprovar, negar ou revogar solicitações. Os usuários convidados não podem aprovar solicitações, mesmo se estiverem no grupo aprovador.

   ```powershell
   Connect-EXOPSSession
   ```

4. Localizar todas as solicitações pendentes.
   > [!NOTE]
   > O valor na propriedade **Identidade** é usado para identificar e aprovar ou recusar a solicitação. Observe que esse valor será usado no parâmetro -RequestId.

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

5. Veja mais detalhes no campo **contexto** da solicitação em que você está interessado.
   > [!NOTE]
   > O campo contexto da solicitação de acesso aos dados descreve os parâmetros e as propriedades de atividade de cópia.

   ```powershell
   Get-ElevatedAccessRequest -RequestId ($requestId).Context | ConvertFrom-Json
   ```

   Você recebe uma resposta semelhante ao seguinte exemplo.

   ```powershell
   Key                          Value
   ---                          -----
   ApplicationName
   ComplianceStatus             [{"Timestamp":"2018-05-02T18:29:21.5705664Z","RequirementName":"adlsEncryption","PolicyComplianceState":"Compliant","Violations":0},{"Timestamp":"2018-05-02T...
   ApplicationMarketPlaceUri
   OutputUri                    adl://myadlserumvrroyspmq.azuredatalakestore.net/targetFolder/Event
   ApplicationPrivacyPolicyUri  http://www.wkw.com/privacy
   ApplicationTermsOfServiceUri http://www.wkw.com/tos
   InstallerIdentity            a89885c3-4b0e-499e-86ed-14d7ed9147c2@942229f8-4656-4fb0-828b-e938dad4019a
   SourceTenantId               942229f8-4656-4fb0-828b-e938dad4019a
   UserScopeQuery               tenant in (942229f8-4656-4fb0-828b-e938dad4019a)
   ApplicationId
   DataTable                    Calendar Events
   DestinationTenantId          942229f8-4656-4fb0-828b-e938dad4019a
   Columns                      Subject:string, HasAttachments:bool, End:DateTime, Start:DateTime, ResponseStatus:string, Organizer:Object, Attendees:string, Importance:string, Sensitivity:...
   ```

6. Aprovar/rejeitar a solicitação usando o valor de **identidade** para o parâmetro -RequestId.

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

Você também pode aprovar a solicitação com uma lista de negações para garantir que dados de certos usuários não sejam incluídos. Para fazer isso, você precisa modificar contexto da solicitação para adicionar o `object Id` do grupo que você deseja omitir e depois aprovar a solicitação.

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

Também é possível revogar as solicitações já aprovadas anteriormente. Semelhante à aprovação de solicitações, o valor de **identidade** é o requerido no parâmetro -RequestId.

   ```powershell
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```

   Você recebe uma resposta semelhante ao seguinte exemplo:

   ```powershell
   AuthorizedBy          : user@tenant.onmicrosoft.com
   Type                  : Task
   AuthorizedAccess      : Data Access Request
   StartTimeUtc          : 7/24/2018 6:02:42 PM
   EndTimeUtc            : 10/22/2018 6:02:42 PM
   Revoked               : True
   RevocationDateTimeUtc : 7/24/2018 9:12:55 PM
   RevokedBy             : NAMPR00A001.prod.outlook.com/Microsoft Exchange Hosted  Organizations/tenant.onmicrosoft.com/user
   RevocationComment     : Revoking this request!
   Identity              : bda75607-0d87-43cb-bdf1-284b18446b34
   DateCreatedUtc        : 1/1/0001 12:00:00 AM
   DateUpdatedUtc        : 7/24/2018 9:12:55 PM
   ```

### <a name="approve-deny-and-revoke-requests-by-using-the-pam-user-experience"></a>Aprovar, negar e revogar solicitações usando a experiência do usuário do PAM

Use as etapas a seguir para interagir com uma solicitação usando a experiência do usuário do PAM:

1. Entre no portal de administração do Microsoft 365 usando credenciais de administrador e, em seguida, vá para a página [Experiência do usuário de aprovação do Gerenciamento de acesso Privilegiado](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess). Esta página mostrará todas as solicitações de acesso (pendentes/aprovadas/expiradas/negadas).

2. Na página resultante, escolha a solicitação que você está interessado. Para selecionar uma lista de negação para depuração de privacidade, selecione a lista suspensa **DenyList**, selecione o grupo que precisa ser depurado e, em seguida, selecione **Aprovar**.

3. Para revogar uma solicitação aprovada anteriormente, escolha a solicitação aprovada a ser revogada e clique em **Revogar**. A próxima tentativa de mover dados usando essa aprovação falha.

### <a name="approval-behavior"></a>Comportamento de aprovação

Aprovação de solicitações da Conexão de Dados do Microsoft Graph têm características específicas das quais você deve estar ciente:

* As solicitações de aprovação são baseadas no Azure Data Factory, pipeline e nomes de atividade de cópia. Cada execução da atividade de cópia verifica se o administrador do Microsoft 365 aprovou a solicitação da atividade de cópia para acessar dados do Office e valida os parâmetros importantes da atividade de cópia executados nos parâmetros da aprovação.
* Em determinadas condições, uma nova solicitação de aprovação é disparada automaticamente. Um aprovador da Conexão de Dados deve aprovar a nova solicitação antes que a atividade de cópia acesse dados do Microsoft 365.
* Se os parâmetros de execução da atividade de cópia forem alterados, uma nova solicitação de aprovação é acionada.
* Se os nomes Azure Data Factory, pipeline ou atividade de cópia forem alterados, uma nova solicitação de aprovação é disparada. Por exemplo: uma nova aprovação é necessária se a tabela de dados ou um conjunto de colunas que a atividade de cópia está acessando for alterado.
* As atividades de cópia devem ser aprovadas uma vez a cada seis meses. Se a aprovação original tiver sido aprovada há seis meses, uma nova solicitação de aprovação será disparada automaticamente.
* Se um Microsoft 365 de acesso a dados tiver negado uma solicitação de aprovação ou revogado uma solicitação aprovada anteriormente, a atividade de cópia falhará continuamente. Trabalhe com o aprovador para entender o motivo da negação ou revogação e corrija os parâmetros da atividade de cópia adequadamente. Para disparar uma nova solicitação de aprovação, uma nova atividade de cópia deve ser implantada ou o nome da atividade de cópia existente deve ser alterado.
* Uma solicitação de aprovação expira em 24 horas, a menos que um aprovador de acesso a dados do Microsoft 365 atue na solicitação. Uma nova solicitação é enviada a cada 24 horas para aprovação. Se você vir suas atividades de cópia aguardando aprovação (no estágio Consentimento Pendente), então trabalhe com os aprovadores de acesso aos dados do Microsoft 365 para que sua solicitação seja aprovada.

## <a name="privacy-scrubbing"></a>A depuração de privacidade

O membro do grupo aprovador que aprova a solicitação pode especificar o nome de um usuário do grupo cujos dados quer que sejam apagados dos dados extraídos. As linhas com os endereços de email correspondentes aos membros do grupo recusado são apagadas dos dados extraídos. Os grupos aninhados dentro do grupo negado são expandidos e somente os usuários são removidos. Consulte a seção de solicitações de aprovação deste artigo para obter detalhes sobre como aplicar a lista de negações durante a aprovação por meio do PowerShell ou da experiência do usuário do PAM.

A tabela a seguir mostra os nomes dos conjuntos de dados e das colunas cujos conteúdos estão marcados para depuração de privacidade.

| Nome do conjunto de dados                                                       | Colunas usadas para depuração baseada na lista de negações              |
| ------------------------------------------------------------------ | ------------------------------------------------------- |
| **BasicDataSet_v0.Message_v0**<br>**BasicDataSet_v0.Message_v1**   | Remetente, De, ParaDestinatário, DestinatáriosCc, DestinatáriosCco |
| **BasicDataSet_v0.SentItem_v0**<br>**BasicDataSet_v0.SentItem_v1** | Remetente, De, ParaDestinatário, DestinatáriosCc, DestinatáriosCco |
| **BasicDataSet_v0.Event_v0**<br>**BasicDataSet_v0.Event_v1**       | Organizador, Participantes                                    |
| **BasicDataSet_v0.Contact_v0**<br>**BasicDataSet_v0.Contact_v1**   | EndereçosEmail                                          |
| **BasicDataSet_v0.CalendarView_v0**                                | Organizador, Participantes                                    |

## <a name="see-also"></a>Confira também

- [Perguntas frequentes sobre a Conexão de Dados](data-connect-faq.md)
