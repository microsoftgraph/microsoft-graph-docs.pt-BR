---
title: Integração do Conexão de Dados do Microsoft Graph com o Privileged Access Management
description: A Conexão de Dados do Microsoft Graph depende do Privileged Access Management para permitir que os administradores do Microsoft 365 aprovem solicitações de movimentação de dados.
author: fercobo-msft
ms.localizationpriority: high
ms.prod: data-connect
ms.openlocfilehash: 8c60df49086ac3b0ebc45475d152e7d7a7d973d9
ms.sourcegitcommit: bfd1ab7e015ef04cb2ca3fb85d308ba2ce830a89
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/19/2022
ms.locfileid: "62072597"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a>Integração do Conexão de Dados do Microsoft Graph com o Privileged Access Management

A Conexão de Dados do Microsoft Graph depende do Privileged Access Management (PAM) para permitir que os administradores do Microsoft 365 aprovem solicitações de movimentação de dados. Os pipelines da Conexão de Dados devem ser aprovados por um membro aprovador de solicitação de acesso a dados especificado pelo administrador do Microsoft 365 durante a ativação. Para configurar o grupo aprovador, consulte [Configurar seu locatário Microsoft 365 e habilitar Conexão de Dados do Microsoft Graph](/graph/data-connect-quickstart?tabs=Microsoft365&tutorial-step=1).

Emails de solicitação de aprovação serão enviados a todos os membros do grupo aprovador para notificá-los quando atividades de cópia solicitam acesso para extrair dados do Microsoft 365. Aprovadores podem aprovar ou negar essas solicitações, especificar um grupo de usuários que deve ser apagado dos dados extraídos ou revogar uma solicitação anteriormente aprovada. As aprovações são válidas por 6 meses, sendo necessária uma aprovação por atividade de cópia no pipeline do Azure Data Factory.

Todas as solicitações sempre incluirão os seguintes detalhes sobre o conjunto de dados e os usuários cujos dados estão sendo extraídos:

* **Solicitante**: O usuário que solicitou o pipeline.
* **Duração**: se aprovado, a validade aprovação. Sempre 4.320 horas (6 meses).
* **Motivo**: motivo para a solicitação, normalmente "um aplicativo instalado para sua organização exige autorização para obter acesso aos dados do Office 365."
* **Solicitado em**: data e hora da solicitação.
* **ID da solicitação**: A ID da solicitação, usada para fins de aprovação.
* **TabelaDados**: O conjunto de dados a ser extraído (por exemplo, itens enviados).
* **Colunas**: A lista de colunas a ser extraída a partir da tabela de dados (por exemplo, DataHorárioEnviado).
* **GruposPermitidos**: o grupo ou grupos de usuários em relação a quem o pipeline está extraindo os dados. Se a lista de grupos estiver vazia, o pipeline está solicitando o acesso aos dados de todos os usuários no locatário.
* **Escopo de Pesquisa de Usuário**: o predicado usado para filtrar os usuários. Somente se aplica se a solicitação for para todos os usuários no locatário. Se esta estiver vazia, nenhum filtro é aplicado.
* **UriSaída**: o caminho de saída no qual os dados extraídos serão armazenados.
* **IdLocatárioOrigem**: a ID do locatário cujos dados são extraídos.
* **IdentidadeInstalador**: a identidade do instalador do aplicativo.

Os seguintes campos na solicitação estarão disponíveis apenas em alguns casos:

* Nome do aplicativo e URI do Marketplace (disponível somente para aplicativos instalados pelo Azure Marketplace).
* Links para a política de privacidade e termos de serviço do aplicativo (disponível somente se o aplicativo fornecer).
* As políticas de conformidade que o aplicativo impõe, como a criptografia de dados inativos no local de armazenamento de saída (disponível somente se o aplicativo fornecer e se o aplicativo foi instalado pelo Azure Marketplace).
* Lista de negações – o grupo de usuários que podem ter sido apagados dos dados extraídos. Esse campo está vazio como parte da solicitação de conjuntos de dados compatíveis com a depuração de privacidade de dados extraídos. Pode ser preenchido por um membro do grupo aprovador que autoriza a solicitação no momento da aprovação.

## <a name="approving-requests"></a>Aprovar solicitações

Os pipelines da Conexão de Dados devem ser aprovados por um membro de um grupo aprovador da solicitação de acesso aos dados. Aprovadores podem aprovar, recusar ou revogar pipelines usando a experiência do usuário PAM ou o módulo do PowerShell do Exchange Online.

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a>Aprovar, negar e revogar solicitações usando o PowerShell

Faça o seguinte para interagir com uma solicitação usando o módulo do PowerShell do Exchange Online:

1. Instalar o módulo do Powershell do Microsoft Exchange Online. Para obter mais informações, confira [Conectar-se ao PowerShell do Exchange Online usando a autenticação de multifator](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).

2. Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator (MFA). Para obter mais informações, confira [Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).
    > [!NOTE]
    > **Observação**: você não precisa habilitar a autenticação multifator para sua organização para usar estas etapas ao se conectar ao PowerShell do Exchange Online. Conexão MFA cria um token OAuth usado pelo PAM para assinar suas solicitações.

3. Entrar com sua conta. Observe que você deve fazer parte do grupo aprovador de acesso aos dados definido para aprovar, recusar ou revogar solicitações. Os usuários convidados não podem aprovar solicitações, mesmo se estiverem no grupo aprovador.

   ```powershell
   Connect-EXOPSSession
   ```

4. Localizar todas as solicitações pendentes.
   > [!NOTE]
   > O valor na propriedade **Identidade** será usado para identificar e aprovar ou recusar a solicitação. Observe que esse valor será usado no parâmetro -RequestId.

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

5. Veja mais detalhes no campo **contexto** da solicitação em que você está interessado.
   >**Observação:** o campo contexto da solicitação de acesso aos dados descreve os parâmetros e as propriedades de atividade de cópia.

   ```powershell
   Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
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

   Você receberá uma resposta semelhante ao seguinte exemplo.

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

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a>Aprovar, negar e revogar solicitações usando a experiência de usuário do PAM

Faça o seguinte para interagir com uma solicitação usando a experiência Web do PAM:

1. Entre no portal de administração do Microsoft 365 usando credenciais de administrador e acesse a página [Experiência do usuário de aprovação do Privileged Access Management](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess). Isso mostra todas as solicitações de acesso (pendentes, aprovada, expiradas, negadas).

2. Na página resultante, escolha a solicitação que você está interessado. Para selecionar uma lista de negação para depuração de privacidade, clique na lista suspensa **ListaNegações**, selecione o grupo que deve ser apagado e selecione **Aprovar**.

3. Para revogar uma solicitação aprovada anteriormente, escolha a solicitação aprovada a ser revogada e clique em **Revogar**. Se a próxima tentativa de mover dados usar essa aprovação, ela irá falhar.

### <a name="approval-behavior"></a>Comportamento de aprovação

Aprovação de solicitações da Conexão de Dados têm características específicas que devem ser consideradas:

* As solicitações de aprovação se baseiam no Azure Data Factory, pipeline e copiam nomes de atividades. Toda execução de atividades de cópia verificará se o administrador do Microsoft 365 aprovou a solicitação de atividade de cópia para acessar dados do Office, e também validará parâmetros importantes de atividades de cópia executadas em relação aos parâmetros de aprovação.
* Em certas condições, uma nova solicitação de aprovação será acionada automaticamente. Um aprovador da Conexão de Dados precisará aprovar a nova solicitação antes que a atividade de cópia acesse dados do Microsoft 365.
* Se os parâmetros de execução da atividade de cópia forem alterados, uma nova solicitação de aprovação será acionada.
* Se o Data Factory, pipeline ou nomes de atividades de cópia forem alterados, uma nova solicitação de aprovação será acionada.
* Por exemplo: uma nova aprovação será necessária se a tabela de dados ou um conjunto de colunas que a atividade de cópia está acessando for alterado.
* As atividades de cópia precisarão de aprovação a cada seis meses. Se a aprovação original foi aprovada há seis meses, uma nova solicitação de aprovação será acionada automaticamente.
* Se o aprovador de acesso aos dados do Microsoft 365 negou uma solicitação de aprovação ou revogou uma aprovada anteriormente, a atividade de cópia irá falhar continuamente. Você deve trabalhar com o aprovador para entender o motivo da negação ou revogação e corrigir os parâmetros da atividade de cópia de acordo com o caso. Será necessário implantar uma nova atividade de cópia ou alterar o nome da atividade de cópia existente para acionar uma nova solicitação de aprovação.
* Se o aprovador de acesso aos dados do Microsoft 365 não der seguimento à solicitação de aprovação em até 24 horas, ela irá expirar. Uma nova solicitação será enviada a cada 24 horas para aprovação. Se você vir suas atividades de cópia aguardando aprovação (no estágio Consentimento Pendente), então trabalhe com os aprovadores de acesso aos dados do Microsoft 365 para que sua solicitação seja aprovada.

## <a name="privacy-scrubbing"></a>A depuração de privacidade

O membro do grupo aprovador que aprova a solicitação pode especificar o nome de um usuário do grupo cujos dados quer que sejam apagados dos dados extraídos. As linhas com os endereços de email correspondentes aos membros do grupo recusado serão apagadas dos dados extraídos. Grupos aninhados dentro do grupo recusado serão expandidos e somente os usuários serão apagados. Consulte a seção deste tópico para saber como aplicar a lista de negação durante a aprovação, por meio do PowerShell ou experiência de usuários do PAM.

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