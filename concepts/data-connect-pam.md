---
title: Integração do Conexão de Dados do Microsoft Graph com o Privileged Access Management
description: A Conexão de Dados do Microsoft Graph depende do Privileged Access Management para permitir que os administradores do Microsoft 365 aprovem solicitações de movimentação de dados.
author: fercobo-msft
localization_priority: Priority
ms.prod: data-connect
ms.openlocfilehash: 3631b652c5e17c333548662b429a56ce3015f55b
ms.sourcegitcommit: 276a13a37c3772689dfc71f7cd47586c9581f27d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/24/2021
ms.locfileid: "52629319"
---
# <a name="microsoft-graph-data-connect-integration-with-privileged-access-management"></a><span data-ttu-id="82d96-103">Integração do Conexão de Dados do Microsoft Graph com o Privileged Access Management</span><span class="sxs-lookup"><span data-stu-id="82d96-103">Microsoft Graph Data Connect integration with Privileged Access Management</span></span>

<span data-ttu-id="82d96-104">A Conexão de Dados do Microsoft Graph depende do Privileged Access Management (PAM) para permitir que os administradores do Microsoft 365 aprovem solicitações de movimentação de dados.</span><span class="sxs-lookup"><span data-stu-id="82d96-104">Microsoft Graph Data Connect relies on Privileged Access Management (PAM) to allow Microsoft 365 administrators to approve data movement requests.</span></span> <span data-ttu-id="82d96-105">Os pipelines da Conexão de Dados devem ser aprovados por um membro aprovador de solicitação de acesso a dados especificado pelo administrador do Microsoft 365 durante a ativação.</span><span class="sxs-lookup"><span data-stu-id="82d96-105">Data Connect pipelines must be approved by a member of the data access request approver specified by the Microsoft 365 administrator during enablement.</span></span> <span data-ttu-id="82d96-106">Para configurar o grupo aprovador, confira [Introdução](data-connect-get-started.md).</span><span class="sxs-lookup"><span data-stu-id="82d96-106">To set up the approver group, see [Get started](data-connect-get-started.md).</span></span>

<span data-ttu-id="82d96-107">Emails de solicitação de aprovação serão enviados a todos os membros do grupo aprovador para notificá-los quando atividades de cópia solicitam acesso para extrair dados do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="82d96-107">Approval request emails will be sent to each member of the approver group to notify them when copy activities request access to extract Microsoft 365 data.</span></span> <span data-ttu-id="82d96-108">Aprovadores podem aprovar ou negar essas solicitações, especificar um grupo de usuários que deve ser apagado dos dados extraídos ou revogar uma solicitação anteriormente aprovada.</span><span class="sxs-lookup"><span data-stu-id="82d96-108">Approvers can approve or deny these requests, specify a user group that should be scrubbed out of extracted data, or revoke a previously approved request.</span></span> <span data-ttu-id="82d96-109">As aprovações são válidas por 6 meses, sendo necessária uma aprovação por atividade de cópia no pipeline do Azure Data Factory.</span><span class="sxs-lookup"><span data-stu-id="82d96-109">Approvals persist for 6 months, and one approval is needed per copy activity in the Azure Data Factory pipeline.</span></span>

<span data-ttu-id="82d96-110">Todas as solicitações sempre incluirão os seguintes detalhes sobre o conjunto de dados e os usuários cujos dados estão sendo extraídos:</span><span class="sxs-lookup"><span data-stu-id="82d96-110">Every request will always include the following details about the dataset and the users about whom data is being extracted:</span></span>

* <span data-ttu-id="82d96-111">**Solicitante**: O usuário que solicitou o pipeline.</span><span class="sxs-lookup"><span data-stu-id="82d96-111">**Requestor**: The user who requested the pipeline.</span></span>
* <span data-ttu-id="82d96-112">**Duração**: se aprovado, a validade aprovação.</span><span class="sxs-lookup"><span data-stu-id="82d96-112">**Duration**: If approved, how long the approval will persist.</span></span> <span data-ttu-id="82d96-113">Sempre 4.320 horas (6 meses).</span><span class="sxs-lookup"><span data-stu-id="82d96-113">Always 4320 hours (6 months).</span></span>
* <span data-ttu-id="82d96-114">**Motivo**: motivo para a solicitação, normalmente "um aplicativo instalado para sua organização exige autorização para obter acesso aos dados do Office 365."</span><span class="sxs-lookup"><span data-stu-id="82d96-114">**Reason**: Reason for the request, typically "An app installed for your organization requires approval for access to Office 365 Data."</span></span>
* <span data-ttu-id="82d96-115">**Solicitado em**: data e hora da solicitação.</span><span class="sxs-lookup"><span data-stu-id="82d96-115">**Requested at**: The DateTime of the request.</span></span>
* <span data-ttu-id="82d96-116">**ID da solicitação**: A ID da solicitação, usada para fins de aprovação.</span><span class="sxs-lookup"><span data-stu-id="82d96-116">**Request id**: The ID of the request, used for approval purposes.</span></span>
* <span data-ttu-id="82d96-117">**TabelaDados**: O conjunto de dados a ser extraído (por exemplo, itens enviados).</span><span class="sxs-lookup"><span data-stu-id="82d96-117">**DataTable**: The data set being extracted (for example, Sent Items).</span></span>
* <span data-ttu-id="82d96-118">**Colunas**: A lista de colunas a ser extraída a partir da tabela de dados (por exemplo, DataHorárioEnviado).</span><span class="sxs-lookup"><span data-stu-id="82d96-118">**Columns**: The list of columns being extracted from the data table (for example, SentDateTime).</span></span>
* <span data-ttu-id="82d96-119">**GruposPermitidos**: o grupo ou grupos de usuários em relação a quem o pipeline está extraindo os dados.</span><span class="sxs-lookup"><span data-stu-id="82d96-119">**AllowedGroups**: The group or groups of users against whom the pipeline is extracting data.</span></span> <span data-ttu-id="82d96-120">Se a lista de grupos estiver vazia, o pipeline está solicitando o acesso aos dados de todos os usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="82d96-120">If the list of groups is empty, the pipeline is requesting access to data from all users in the tenant.</span></span>
* <span data-ttu-id="82d96-121">**Escopo de Pesquisa de Usuário**: o predicado usado para filtrar os usuários.</span><span class="sxs-lookup"><span data-stu-id="82d96-121">**User Scope Query**: The predicate used to filter out users.</span></span> <span data-ttu-id="82d96-122">Somente se aplica se a solicitação for para todos os usuários no locatário.</span><span class="sxs-lookup"><span data-stu-id="82d96-122">Only applies if the request is for all users in the tenant.</span></span> <span data-ttu-id="82d96-123">Se esta estiver vazia, nenhum filtro é aplicado.</span><span class="sxs-lookup"><span data-stu-id="82d96-123">If this is empty, no filter is applied.</span></span>
* <span data-ttu-id="82d96-124">**UriSaída**: o caminho de saída no qual os dados extraídos serão armazenados.</span><span class="sxs-lookup"><span data-stu-id="82d96-124">**OutputUri**: The output path in which the extracted data will be stored.</span></span>
* <span data-ttu-id="82d96-125">**IdLocatárioOrigem**: a ID do locatário cujos dados são extraídos.</span><span class="sxs-lookup"><span data-stu-id="82d96-125">**SourceTenantId**: The tenant ID from which data is being extracted.</span></span>
* <span data-ttu-id="82d96-126">**IdentidadeInstalador**: a identidade do instalador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="82d96-126">**InstallerIdentity**: The identity of the app installer.</span></span>

<span data-ttu-id="82d96-127">Os seguintes campos na solicitação estarão disponíveis apenas em alguns casos:</span><span class="sxs-lookup"><span data-stu-id="82d96-127">The following fields in the request will be available only in some cases:</span></span>

* <span data-ttu-id="82d96-128">Nome do aplicativo e URI do Marketplace (disponível somente para aplicativos instalados pelo Azure Marketplace).</span><span class="sxs-lookup"><span data-stu-id="82d96-128">Application Name and the Marketplace URI (available only for applications installed from the Azure marketplace).</span></span>
* <span data-ttu-id="82d96-129">Links para a política de privacidade e termos de serviço do aplicativo (disponível somente se o aplicativo fornecer).</span><span class="sxs-lookup"><span data-stu-id="82d96-129">Links to the application's privacy policy and terms of service (available only if the application provides it).</span></span>
* <span data-ttu-id="82d96-130">As políticas de conformidade que o aplicativo impõe, como a criptografia de dados inativos no local de armazenamento de saída (disponível somente se o aplicativo fornecer e se o aplicativo foi instalado pelo Azure Marketplace).</span><span class="sxs-lookup"><span data-stu-id="82d96-130">The compliance policies that the application enforces, such as data encryption at rest in the output storage location (available only if the application provides it and if the application is installed from the Azure marketplace).</span></span>
* <span data-ttu-id="82d96-131">Lista de negações – o grupo de usuários que podem ter sido apagados dos dados extraídos.</span><span class="sxs-lookup"><span data-stu-id="82d96-131">Deny List - The user group that can be scrubbed out of the extracted data.</span></span> <span data-ttu-id="82d96-132">Esse campo está vazio como parte da solicitação de conjuntos de dados compatíveis com a depuração de privacidade de dados extraídos.</span><span class="sxs-lookup"><span data-stu-id="82d96-132">This field is empty as a part of the request for datasets that support privacy scrubbing of extracted data.</span></span> <span data-ttu-id="82d96-133">Pode ser preenchido por um membro do grupo aprovador que autoriza a solicitação no momento da aprovação.</span><span class="sxs-lookup"><span data-stu-id="82d96-133">It can be populated by the member of the approver group who approves the request at approval time.</span></span>

## <a name="approving-requests"></a><span data-ttu-id="82d96-134">Aprovar solicitações</span><span class="sxs-lookup"><span data-stu-id="82d96-134">Approving requests</span></span>

<span data-ttu-id="82d96-135">Os pipelines da Conexão de Dados devem ser aprovados por um membro de um grupo aprovador da solicitação de acesso aos dados.</span><span class="sxs-lookup"><span data-stu-id="82d96-135">Data Connect pipelines must be approved by a member of a data access request approver group.</span></span> <span data-ttu-id="82d96-136">Aprovadores podem aprovar, recusar ou revogar pipelines usando a experiência do usuário PAM ou o módulo do PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="82d96-136">Approvers can approve, deny, or revoke pipelines by using the Exchange Online PowerShell module or the PAM user experience.</span></span>

### <a name="approving-denying-and-revoking-requests-by-using-powershell"></a><span data-ttu-id="82d96-137">Aprovar, negar e revogar solicitações usando o PowerShell</span><span class="sxs-lookup"><span data-stu-id="82d96-137">Approving, denying, and revoking requests by using PowerShell</span></span>

<span data-ttu-id="82d96-138">Faça o seguinte para interagir com uma solicitação usando o módulo do PowerShell do Exchange Online:</span><span class="sxs-lookup"><span data-stu-id="82d96-138">Use the following steps to interact with a request using the Exchange Online PowerShell module:</span></span>

1. <span data-ttu-id="82d96-139">Instalar o módulo do Powershell do Microsoft Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="82d96-139">Install the Exchange Online Powershell module.</span></span> <span data-ttu-id="82d96-140">Para obter mais informações, confira [Conectar-se ao PowerShell do Exchange Online usando a autenticação de multifator](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="82d96-140">For installation instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>

2. <span data-ttu-id="82d96-141">Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator (MFA).</span><span class="sxs-lookup"><span data-stu-id="82d96-141">Connect to Exchange Online Powershell using multi-factor authentication (MFA).</span></span> <span data-ttu-id="82d96-142">Para obter mais informações, confira [Conectar-se ao PowerShell do Exchange Online usando a autenticação multifator](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="82d96-142">For instructions, see [Connect to Exchange Online PowerShell using multi-factor authentication](/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell?view=exchange-ps).</span></span>
    > [!NOTE]
    > <span data-ttu-id="82d96-143">**Observação**: você não precisa habilitar a autenticação multifator para sua organização para usar estas etapas ao se conectar ao PowerShell do Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="82d96-143">**Note**: You do not need to enable multi-factor authentication for your organization to use these steps while connecting to Exchange Online PowerShell.</span></span> <span data-ttu-id="82d96-144">Conexão MFA cria um token OAuth usado pelo PAM para assinar suas solicitações.</span><span class="sxs-lookup"><span data-stu-id="82d96-144">Connecting with MFA creates an OAuth token that is used by PAM for signing your requests.</span></span>

3. <span data-ttu-id="82d96-145">Entrar com sua conta.</span><span class="sxs-lookup"><span data-stu-id="82d96-145">Sign in with your account.</span></span> <span data-ttu-id="82d96-146">Observe que você deve fazer parte do grupo aprovador de acesso aos dados definido para aprovar, recusar ou revogar solicitações.</span><span class="sxs-lookup"><span data-stu-id="82d96-146">Note that you must be part of the configured data access approver group in order to be able to approve, deny, or revoke requests.</span></span> <span data-ttu-id="82d96-147">Os usuários convidados não podem aprovar solicitações, mesmo se estiverem no grupo aprovador.</span><span class="sxs-lookup"><span data-stu-id="82d96-147">Guest users cannot approve requests, even if they are in the approver group.</span></span>

   ```powershell
   Connect-EXOPSSession
   ```

4. <span data-ttu-id="82d96-148">Localizar todas as solicitações pendentes.</span><span class="sxs-lookup"><span data-stu-id="82d96-148">Find all pending requests.</span></span>
   > [!NOTE]
   > <span data-ttu-id="82d96-149">O valor na propriedade **Identidade** será usado para identificar e aprovar ou recusar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="82d96-149">The value in the **Identity** property will be used to identify and approve or deny the request.</span></span> <span data-ttu-id="82d96-150">Observe que esse valor será usado no parâmetro -RequestId.</span><span class="sxs-lookup"><span data-stu-id="82d96-150">Note this value and use it in the -RequestId parameter.</span></span>

   ```powershell
   Get-ElevatedAccessRequest | ?{$_.RequestStatus -eq 'Pending'}
   ```

5. <span data-ttu-id="82d96-151">Veja mais detalhes no campo **contexto** da solicitação em que você está interessado.</span><span class="sxs-lookup"><span data-stu-id="82d96-151">Take a closer look at the **context** field of the request you are interested in.</span></span>
   ><span data-ttu-id="82d96-152">**Observação:** o campo contexto da solicitação de acesso aos dados descreve os parâmetros e as propriedades de atividade de cópia.</span><span class="sxs-lookup"><span data-stu-id="82d96-152">**Note:** The context field of the data access request describes the parameters and properties of the copy activity.</span></span>

   ```powershell
   Get-ElevatedAccessRequest -RequestId $requestId).Context | ConvertFrom-Json
   ```

   <span data-ttu-id="82d96-153">Você recebe uma resposta semelhante ao seguinte exemplo.</span><span class="sxs-lookup"><span data-stu-id="82d96-153">You'll get a response that looks like the following.</span></span>

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

6. <span data-ttu-id="82d96-154">Aprovar/rejeitar a solicitação usando o valor de **identidade** para o parâmetro -RequestId.</span><span class="sxs-lookup"><span data-stu-id="82d96-154">Approve/deny the request using the value for **Identity** for the -RequestId parameter.</span></span>

   ```powershell
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!"
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="82d96-155">Você também pode aprovar a solicitação com uma lista de negações para garantir que dados de certos usuários não sejam incluídos.</span><span class="sxs-lookup"><span data-stu-id="82d96-155">You can also approve the request with a deny list to ensure data from certain users is not included.</span></span> <span data-ttu-id="82d96-156">Para fazer isso, você precisa modificar contexto da solicitação para adicionar o `object Id` do grupo que você deseja omitir e depois aprovar a solicitação.</span><span class="sxs-lookup"><span data-stu-id="82d96-156">To do so, you need to modify the context of the request to add the `object Id` of the group that you want to omit and then approve the request.</span></span>

   ```powershell
   $request = Get-ElevatedAccessRequest -RequestId
   $hash = $request.Context
   $hash["DenyList"] = <Object ID of denied user group>;
   Approve-ElevatedAccessRequest -RequestId $requestId -Comment "Yay!!" -RequestContext $hash
   Deny-ElevatedAccessRequest -RequestId $requestId -Comment "Nay!!"
   ```

<span data-ttu-id="82d96-157">Também é possível revogar as solicitações já aprovadas anteriormente.</span><span class="sxs-lookup"><span data-stu-id="82d96-157">You can also revoke requests that were previously approved.</span></span> <span data-ttu-id="82d96-158">Semelhante à aprovação de solicitações, o valor de **identidade** é o requerido no parâmetro -RequestId.</span><span class="sxs-lookup"><span data-stu-id="82d96-158">Similar to approving requests, the value for **Identity** is what is required in the -RequestId parameter.</span></span>

   ```powershell
   Revoke-ElevatedAccessAuthorization -Comment "Revoking this request!" -RequestId $requestId
   ```

   <span data-ttu-id="82d96-159">Você receberá uma resposta semelhante ao seguinte exemplo.</span><span class="sxs-lookup"><span data-stu-id="82d96-159">You'll see a response similar to the following.</span></span>

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

### <a name="approving-denying-and-revoking-requests-by-using-the-pam-user-experience"></a><span data-ttu-id="82d96-160">Aprovar, negar e revogar solicitações usando a experiência de usuário do PAM</span><span class="sxs-lookup"><span data-stu-id="82d96-160">Approving, denying, and revoking requests by using the PAM user experience</span></span>

<span data-ttu-id="82d96-161">Faça o seguinte para interagir com uma solicitação usando a experiência Web do PAM:</span><span class="sxs-lookup"><span data-stu-id="82d96-161">Use the following steps to interact with a request using the PAM web experience:</span></span>

1. <span data-ttu-id="82d96-162">Entre no portal de administração do Microsoft 365 usando credenciais de administrador e acesse a página [Experiência do usuário de aprovação do Privileged Access Management](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess).</span><span class="sxs-lookup"><span data-stu-id="82d96-162">Sign in to the Microsoft 365 admin portal using admin credentials and go to the [Privileged Access Managment approval user experience](https://admin.microsoft.com/AdminPortal/Home#/Settings/PrivilegedAccess) page.</span></span> <span data-ttu-id="82d96-163">Isso mostra todas as solicitações de acesso (pendentes, aprovada, expiradas, negadas).</span><span class="sxs-lookup"><span data-stu-id="82d96-163">This will show you all the access requests (pending/approved/expired/denied).</span></span>

2. <span data-ttu-id="82d96-164">Na página resultante, escolha a solicitação que você está interessado.</span><span class="sxs-lookup"><span data-stu-id="82d96-164">On the resulting page, select the request that you're interested in.</span></span> <span data-ttu-id="82d96-165">Para selecionar uma lista de negação para depuração de privacidade, clique na lista suspensa **ListaNegações**, selecione o grupo que deve ser apagado e selecione **Aprovar**.</span><span class="sxs-lookup"><span data-stu-id="82d96-165">To select a deny list for privacy scrubbing, click the **DenyList** dropdown, select the group that needs to be scrubbed, and then select **Approve**.</span></span>

3. <span data-ttu-id="82d96-166">Para revogar uma solicitação aprovada anteriormente, escolha a solicitação aprovada a ser revogada e clique em **Revogar**.</span><span class="sxs-lookup"><span data-stu-id="82d96-166">To revoke a previously approved request, select the approved request that needs to be revoked, and choose **Revoke**.</span></span> <span data-ttu-id="82d96-167">Se a próxima tentativa de mover dados usar essa aprovação, ela irá falhar.</span><span class="sxs-lookup"><span data-stu-id="82d96-167">The next attempt to move data using that approval will fail.</span></span>

### <a name="approval-behavior"></a><span data-ttu-id="82d96-168">Comportamento de aprovação</span><span class="sxs-lookup"><span data-stu-id="82d96-168">Approval behavior</span></span>

<span data-ttu-id="82d96-169">Aprovação de solicitações da Conexão de Dados têm características específicas que devem ser consideradas:</span><span class="sxs-lookup"><span data-stu-id="82d96-169">Data Connect approval requests have particular characteristics that are important to be aware of:</span></span>

* <span data-ttu-id="82d96-p118">As solicitações de aprovação se baseiam no Azure Data Factory, pipeline e copiam nomes de atividades. Toda execução de atividades de cópia verificará se o administrador do Microsoft 365 aprovou a solicitação de atividade de cópia para acessar dados do Office, e também validará parâmetros importantes de atividades de cópia executadas em relação aos parâmetros de aprovação.</span><span class="sxs-lookup"><span data-stu-id="82d96-p118">Approval requests are based on the Azure Data Factory, pipeline and copy activity names. Every copy activity run will verify that the Microsoft 365 admin has approved the copy activity's request to access Office data, and will validate the important parameters of the copy activity run against the parameters of the approval.</span></span>
* <span data-ttu-id="82d96-172">Em certas condições, uma nova solicitação de aprovação será acionada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="82d96-172">Under certain conditions, a new approval request will automatically be triggered.</span></span> <span data-ttu-id="82d96-173">Um aprovador da Conexão de Dados precisará aprovar a nova solicitação antes que a atividade de cópia acesse dados do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="82d96-173">A Data Connect approver will have to approve the new request before the copy activity can access Microsoft 365 data.</span></span>
* <span data-ttu-id="82d96-174">Se os parâmetros de execução da atividade de cópia forem alterados, uma nova solicitação de aprovação será acionada.</span><span class="sxs-lookup"><span data-stu-id="82d96-174">If the parameters of the copy activity run changes, a new approval request will be triggered.</span></span>
* <span data-ttu-id="82d96-175">Se o Data Factory, pipeline ou nomes de atividades de cópia forem alterados, uma nova solicitação de aprovação será acionada.</span><span class="sxs-lookup"><span data-stu-id="82d96-175">If the Data Factory, pipeline or copy activity names change, a new approval request will be triggered.</span></span>
* <span data-ttu-id="82d96-176">Por exemplo: uma nova aprovação será necessária se a tabela de dados ou um conjunto de colunas que a atividade de cópia está acessando for alterado.</span><span class="sxs-lookup"><span data-stu-id="82d96-176">For example: A new approval will be required if the data table or set of columns that the copy activity is accessing changes.</span></span>
* <span data-ttu-id="82d96-177">As atividades de cópia precisarão de aprovação a cada seis meses.</span><span class="sxs-lookup"><span data-stu-id="82d96-177">Copy activities will have to be approved once every 6 months.</span></span> <span data-ttu-id="82d96-178">Se a aprovação original foi aprovada há seis meses, uma nova solicitação de aprovação será acionada automaticamente.</span><span class="sxs-lookup"><span data-stu-id="82d96-178">If the original approval was approved 6 months ago, a new approval request will automatically be triggered.</span></span>
* <span data-ttu-id="82d96-179">Se o aprovador de acesso aos dados do Microsoft 365 negou uma solicitação de aprovação ou revogou uma aprovada anteriormente, a atividade de cópia irá falhar continuamente.</span><span class="sxs-lookup"><span data-stu-id="82d96-179">If a Microsoft 365 Data Access approver has denied an approval request or revoked a previously approved request, the copy activity will fail continually.</span></span> <span data-ttu-id="82d96-180">Você deve trabalhar com o aprovador para entender o motivo da negação ou revogação e corrigir os parâmetros da atividade de cópia de acordo com o caso.</span><span class="sxs-lookup"><span data-stu-id="82d96-180">You should work with the approver to understand the reason for the denial or revocation and fix the parameters of the copy activity accordingly.</span></span> <span data-ttu-id="82d96-181">Será necessário implantar uma nova atividade de cópia ou alterar o nome da atividade de cópia existente para acionar uma nova solicitação de aprovação.</span><span class="sxs-lookup"><span data-stu-id="82d96-181">A new copy activity will have to deployed, or the name of the existing copy activity will have to be changed in order to trigger a new approval request for approval.</span></span>
* <span data-ttu-id="82d96-182">Se o aprovador de acesso aos dados do Microsoft 365 não der seguimento à solicitação de aprovação em até 24 horas, ela irá expirar.</span><span class="sxs-lookup"><span data-stu-id="82d96-182">An approval request will expire in 24 hours unless a Microsoft 365 data access approver acts on the request.</span></span> <span data-ttu-id="82d96-183">Uma nova solicitação será enviada a cada 24 horas para aprovação.</span><span class="sxs-lookup"><span data-stu-id="82d96-183">A new request will be submitted once every 24 hours for approval.</span></span> <span data-ttu-id="82d96-184">Se você vir suas atividades de cópia aguardando aprovação (no estágio Consentimento Pendente), então trabalhe com os aprovadores de acesso aos dados do Microsoft 365 para que sua solicitação seja aprovada.</span><span class="sxs-lookup"><span data-stu-id="82d96-184">If you see your copy activity waiting for approval (in the Consent Pending stage), then work with Microsoft 365 data access approvers to get your request approved.</span></span>

## <a name="privacy-scrubbing"></a><span data-ttu-id="82d96-185">A depuração de privacidade</span><span class="sxs-lookup"><span data-stu-id="82d96-185">Privacy scrubbing</span></span>

<span data-ttu-id="82d96-186">O membro do grupo aprovador que aprova a solicitação pode especificar o nome de um usuário do grupo cujos dados quer que sejam apagados dos dados extraídos.</span><span class="sxs-lookup"><span data-stu-id="82d96-186">The member of the approver group who approves the request can specify the name of one user group whose data would be scrubbed out of extracted data.</span></span> <span data-ttu-id="82d96-187">As linhas com os endereços de email correspondentes aos membros do grupo recusado serão apagadas dos dados extraídos.</span><span class="sxs-lookup"><span data-stu-id="82d96-187">The rows containing email addresses corresponding to the members of the denied group will be scrubbed out of extracted data.</span></span> <span data-ttu-id="82d96-188">Grupos aninhados dentro do grupo recusado serão expandidos e somente os usuários serão apagados. Consulte a seção deste tópico para saber como aplicar a lista de negação durante a aprovação, por meio do PowerShell ou experiência de usuários do PAM.</span><span class="sxs-lookup"><span data-stu-id="82d96-188">Groups nested within the denied group will be expanded and only users will be scrubbed out. Refer to the approving requests section of this topic for details on how to apply the deny list during approval, through either PowerShell or the PAM UX.</span></span>

<span data-ttu-id="82d96-189">A tabela a seguir mostra os nomes dos conjuntos de dados e das colunas cujos conteúdos estão marcados para depuração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="82d96-189">The following table shows the names of the datasets and the columns for which the contents are checked for privacy scrubbing.</span></span>

| <span data-ttu-id="82d96-190">Nome do conjunto de dados</span><span class="sxs-lookup"><span data-stu-id="82d96-190">Dataset name</span></span>                                                       | <span data-ttu-id="82d96-191">Colunas usadas para depuração baseada na lista de negações</span><span class="sxs-lookup"><span data-stu-id="82d96-191">Columns used for deny list-based scrubbing</span></span>              |
| ------------------------------------------------------------------ | ------------------------------------------------------- |
| <span data-ttu-id="82d96-192">**BasicDataSet_v0.Message_v0**</span><span class="sxs-lookup"><span data-stu-id="82d96-192">**BasicDataSet_v0.Message_v0**</span></span><br><span data-ttu-id="82d96-193">**BasicDataSet_v0.Message_v1**</span><span class="sxs-lookup"><span data-stu-id="82d96-193">**BasicDataSet_v0.Message_v1**</span></span>   | <span data-ttu-id="82d96-194">Remetente, De, ParaDestinatário, DestinatáriosCc, DestinatáriosCco</span><span class="sxs-lookup"><span data-stu-id="82d96-194">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span> |
| <span data-ttu-id="82d96-195">**BasicDataSet_v0.SentItem_v0**</span><span class="sxs-lookup"><span data-stu-id="82d96-195">**BasicDataSet_v0.SentItem_v0**</span></span><br><span data-ttu-id="82d96-196">**BasicDataSet_v0.SentItem_v1**</span><span class="sxs-lookup"><span data-stu-id="82d96-196">**BasicDataSet_v0.SentItem_v1**</span></span> | <span data-ttu-id="82d96-197">Remetente, De, ParaDestinatário, DestinatáriosCc, DestinatáriosCco</span><span class="sxs-lookup"><span data-stu-id="82d96-197">Sender, From, ToRecipients, CcRecipients, BccRecipients</span></span> |
| <span data-ttu-id="82d96-198">**BasicDataSet_v0.Event_v0**</span><span class="sxs-lookup"><span data-stu-id="82d96-198">**BasicDataSet_v0.Event_v0**</span></span><br><span data-ttu-id="82d96-199">**BasicDataSet_v0.Event_v1**</span><span class="sxs-lookup"><span data-stu-id="82d96-199">**BasicDataSet_v0.Event_v1**</span></span>       | <span data-ttu-id="82d96-200">Organizador, Participantes</span><span class="sxs-lookup"><span data-stu-id="82d96-200">Organizer, Attendees</span></span>                                    |
| <span data-ttu-id="82d96-201">**BasicDataSet_v0.Contact_v0**</span><span class="sxs-lookup"><span data-stu-id="82d96-201">**BasicDataSet_v0.Contact_v0**</span></span><br><span data-ttu-id="82d96-202">**BasicDataSet_v0.Contact_v1**</span><span class="sxs-lookup"><span data-stu-id="82d96-202">**BasicDataSet_v0.Contact_v1**</span></span>   | <span data-ttu-id="82d96-203">EndereçosEmail</span><span class="sxs-lookup"><span data-stu-id="82d96-203">EmailAddresses</span></span>                                          |
| <span data-ttu-id="82d96-204">**BasicDataSet_v0.CalendarView_v0**</span><span class="sxs-lookup"><span data-stu-id="82d96-204">**BasicDataSet_v0.CalendarView_v0**</span></span>                                | <span data-ttu-id="82d96-205">Organizador, Participantes</span><span class="sxs-lookup"><span data-stu-id="82d96-205">Organizer, Attendees</span></span>                                    |

## <a name="see-also"></a><span data-ttu-id="82d96-206">Confira também</span><span class="sxs-lookup"><span data-stu-id="82d96-206">See also</span></span>

- [<span data-ttu-id="82d96-207">Perguntas frequentes sobre a Conexão de Dados</span><span class="sxs-lookup"><span data-stu-id="82d96-207">Data Connect frequently asked questions</span></span>](data-connect-faq.md)
