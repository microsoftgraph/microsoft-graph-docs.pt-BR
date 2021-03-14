---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos com o Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 07ee284f40264c76ec6156235fab651fff77cfe6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/13/2021
ms.locfileid: "50777002"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="ff3e1-103">Problemas conhecidos com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="ff3e1-103">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="ff3e1-104">Este artigo descreve os problemas conhecidos com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-104">This article describes known issues with Microsoft Graph.</span></span> 

<span data-ttu-id="ff3e1-105">Para relatar um problema conhecido, confira a página [Suporte Microsoft Graph](https://developer.microsoft.com/graph/support).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-105">To report a known issue, see the [Microsoft Graph support](https://developer.microsoft.com/graph/support) page.</span></span>

<span data-ttu-id="ff3e1-106">Para saber mais sobre as atualizações mais recentes da API do Microsoft Graph, confira o [changelog do Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-106">For information about the latest updates to the Microsoft Graph API, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="bookings"></a><span data-ttu-id="ff3e1-107">Reservas</span><span class="sxs-lookup"><span data-stu-id="ff3e1-107">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="ff3e1-108">ErrorExceededFindCountLimit ao consultar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="ff3e1-108">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="ff3e1-109">A obtenção da lista de `bookingBusinesses` falha com o seguinte código de erro quando a organização tem várias empresas de Reservas e a conta que está fazendo a solicitação não é um administrador:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-109">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="ff3e1-110">Como alternativa, você pode limitar o conjunto de empresas retornadas pela solicitação, incluindo um parâmetro `query`, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-110">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a><span data-ttu-id="ff3e1-111">Calendários</span><span class="sxs-lookup"><span data-stu-id="ff3e1-111">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="ff3e1-112">Acessar um calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="ff3e1-112">Accessing a shared calendar</span></span>

<span data-ttu-id="ff3e1-113">Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-113">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET /users/{id}/calendars/{id}/events
```

<span data-ttu-id="ff3e1-p101">Você pode receber HTTP 500 com o código de erro `ErrorInternalServerTransientError`. O erro ocorre porque:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p101">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="ff3e1-116">Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-116">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="ff3e1-117">A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-117">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="ff3e1-118">Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-118">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="ff3e1-119">Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-119">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="ff3e1-120">Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-120">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="ff3e1-121">Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-121">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="ff3e1-122">Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-122">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="ff3e1-123">O destinatário remove o calendário previamente compartilhado com ele.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-123">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="ff3e1-124">O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-124">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="ff3e1-p103">O destinatário aceita novamente o calendário compartilhado usando o Outlook na Web. Em breve você poderá usar outros clientes do Outlook.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p103">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="ff3e1-127">O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-127">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="ff3e1-p104">Um calendário compartilhado com você na nova abordagem é exibido como qualquer outro na sua caixa de correio. Você pode usar a API REST de calendário para visualizar e editar eventos no calendário compartilhado, como se fosse seu próprio calendário. Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p104">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="ff3e1-131">Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="ff3e1-131">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="ff3e1-132">Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):</span><span class="sxs-lookup"><span data-stu-id="ff3e1-132">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="ff3e1-133">Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-133">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="ff3e1-p105">[Listar os calendários do usuário](/graph/api/user-list-calendars) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](/graph/api/resources/calendar) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p105">[Listing the user's calendars](/graph/api/user-list-calendars) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="ff3e1-136">Você também pode [listar os eventos](/graph/api/calendar-list-events) de um calendário baseado em ICS.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-136">You can also [list the events](/graph/api/calendar-list-events) of an ICS-based calendar.</span></span>

### <a name="attaching-large-files-to-events"></a><span data-ttu-id="ff3e1-137">Anexar arquivos grandes a eventos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-137">Attaching large files to events</span></span>
<span data-ttu-id="ff3e1-138">Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-138">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="ff3e1-139">Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-139">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="ff3e1-140">Suporte de propriedade onlineMeetingUrl do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ff3e1-140">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="ff3e1-141">Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event) de reunião do Skype indica a URL da reunião online.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-141">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event) would indicate the online meeting URL.</span></span> <span data-ttu-id="ff3e1-142">No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-142">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

<span data-ttu-id="ff3e1-143">A versão beta oferece uma solução alternativa, na qual é possível usar a propriedade **onlineMeetingProvider** de um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)para verificar se o provedor é o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-143">The beta version offers a workaround, where you can use the **onlineMeetingProvider** property of an [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) to verify if the provider is Microsoft Teams.</span></span> <span data-ttu-id="ff3e1-144">Por meio da propriedade **onlineMeeting** do **evento**, você pode acessar o **joinUrl**.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-144">Through the **onlineMeeting** property of the **event**, you can access the **joinUrl**.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="ff3e1-145">Notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="ff3e1-145">Change notifications</span></span>

### <a name="additional-notifications-for-users"></a><span data-ttu-id="ff3e1-146">Notificações adicionais para usuários</span><span class="sxs-lookup"><span data-stu-id="ff3e1-146">Additional notifications for users</span></span>

<span data-ttu-id="ff3e1-147">As [assinaturas](/graph/api/resources/subscription) de alterações para o **usuário** com o **changeType** definido como **atualizado** também receberão notificações de **changeType**: **atualizado** na criação do usuário e exclusão reversível do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-147">[Subscriptions](/graph/api/resources/subscription) to changes for **user** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on user creation and user soft deletion.</span></span>

### <a name="additional-notifications-for-groups"></a><span data-ttu-id="ff3e1-148">Notificações adicionais para grupos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-148">Additional notifications for groups</span></span>

<span data-ttu-id="ff3e1-149">As [assinaturas](/graph/api/resources/subscription) de alterações no **grupo** com o **changeType** definido como **atualizado** também receberão notificações **changeType**: **atualizado** na criação do grupo e exclusão reversível do grupo.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-149">[Subscriptions](/graph/api/resources/subscription) to changes for **group** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on group creation and group soft deletion.</span></span>

## <a name="cloud-communications"></a><span data-ttu-id="ff3e1-150">Comunicações na nuvem</span><span class="sxs-lookup"><span data-stu-id="ff3e1-150">Cloud communications</span></span> 

<span data-ttu-id="ff3e1-151">O cliente do Microsoft Teams não mostra o menu **Exibir detalhes da Reunião** para reuniões de canal criadas por meio da API de comunicações na nuvem.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-151">The Microsoft Teams client does not show the **View Meeting details**  menu for channel meetings created via the cloud communications API.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="ff3e1-152">Aplicativos de Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="ff3e1-152">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="ff3e1-153">Os aplicativos CSP devem usar o ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="ff3e1-153">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="ff3e1-p109">Aplicativos de provedor de solução de nuvem (CSP) devem adquirir tokens de pontos de extremidade do Azure AD (v1) para chamar a Microsoft Graph com êxito em seus clientes gerenciados por parceiros. Atualmente, não há suporte para aquisição de um token pelo ponto de extremidade Azure AD v 2.0 mais recente.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p109">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="ff3e1-156">A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente</span><span class="sxs-lookup"><span data-stu-id="ff3e1-156">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="ff3e1-157">Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-157">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="ff3e1-158">Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-158">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="ff3e1-159">Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-159">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="ff3e1-160">Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-160">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="ff3e1-161">Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-161">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="ff3e1-p110">**OBSERVAÇÃO:** esta não é uma solução permanente e destina-se apenas a desbloquear o desenvolvimento.  Esta solução alternativa não será necessária uma vez que a questão acima mencionada seja corrigida.  Esta solução alternativa não precisa ser desfeita após a correção.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p110">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="ff3e1-p111">Abra uma sessão do Azure AD v2 PowerShell e conecte-se ao locatário do parceiro `customer`digitando suas credenciais de administrador na janela de entrada. Você pode baixar e instalar o Azure AD PowerShell V2 [aqui](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p111">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="ff3e1-167">Crie o servicePrincipal do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-167">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a><span data-ttu-id="ff3e1-168">Contatos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-168">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="ff3e1-169">Contatos de organização disponíveis somente na versão beta</span><span class="sxs-lookup"><span data-stu-id="ff3e1-169">Organization contacts available in only beta</span></span>

<span data-ttu-id="ff3e1-p112">Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p112">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="ff3e1-172">Pasta Contatos padrão</span><span class="sxs-lookup"><span data-stu-id="ff3e1-172">Default contacts folder</span></span>

<span data-ttu-id="ff3e1-173">Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-173">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="ff3e1-p113">Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](/graph/api/user-list-contacts) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p113">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="ff3e1-176">Na consulta acima:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-176">In the above query:</span></span>

1. <span data-ttu-id="ff3e1-177">`/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact) na pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-177">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="ff3e1-178">A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-178">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="ff3e1-179">Acessar contatos por meio de uma pasta de contatos na versão beta</span><span class="sxs-lookup"><span data-stu-id="ff3e1-179">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="ff3e1-180">Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-180">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="ff3e1-181">Acessando um contato a partir de um nível superior do [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-181">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="ff3e1-p114">Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p114">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="ff3e1-184">Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-184">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a><span data-ttu-id="ff3e1-185">Consulta delta</span><span class="sxs-lookup"><span data-stu-id="ff3e1-185">Delta query</span></span>

* <span data-ttu-id="ff3e1-186">O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-186">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="ff3e1-187">As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-187">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="ff3e1-188">Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-188">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="extensions"></a><span data-ttu-id="ff3e1-189">Extensões</span><span class="sxs-lookup"><span data-stu-id="ff3e1-189">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="ff3e1-190">Não há suporte para o controle de alterações</span><span class="sxs-lookup"><span data-stu-id="ff3e1-190">Change tracking is not supported</span></span>

<span data-ttu-id="ff3e1-191">O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-191">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="ff3e1-192">Criar um recurso e uma extensão aberta ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-192">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="ff3e1-p115">Você não pode especificar uma extensão aberta ao mesmo tempo que cria uma instância de **administrativeUnit**, **device**, **group**, **organization** ou **user**. Primeiro você deve criar a instância e, depois, especificar os dados da extensão aberta em uma solicitação ``POST`` subsequente nessa instância.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p115">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="ff3e1-195">Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-195">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="ff3e1-196">Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-196">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="ff3e1-197">Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-197">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="ff3e1-198">Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-198">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="ff3e1-199">Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-199">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a><span data-ttu-id="ff3e1-200">Atualizar uma definição de schemaExtension usando o Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="ff3e1-200">Updating a schemaExtension definition using Microsoft Graph Explorer</span></span>

<span data-ttu-id="ff3e1-201">Ao usar `PATCH` para atualizar uma schemaExtension usando o Graph Explorer, você deve especificar a propriedade de **proprietário** e defini-la com seu valor `appid` atual (que será necessário ser uma `appId` de um aplicativo que você tenha).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-201">When using `PATCH` to update a schemaExtension using Graph Explorer, you must specify the **owner** property and set it to its current `appid` value (which will need to be an `appId` of an application that you own).</span></span> <span data-ttu-id="ff3e1-202">Esse também é o caso de qualquer aplicativo de cliente que `appId` não seja o mesmo que o do **proprietário**.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-202">This is also the case for any client application whose `appId` is not the same as the **owner**.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="ff3e1-203">Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="ff3e1-203">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="ff3e1-204">Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-204">Filtering on schema extension properties (using the `$filter` expression) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="files-onedrive"></a><span data-ttu-id="ff3e1-205">Arquivos (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="ff3e1-205">Files (OneDrive)</span></span>

* <span data-ttu-id="ff3e1-206">O primeiro acesso a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse o próprio site pessoal por um navegador resulta em uma resposta 401.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-206">First time access to a user's personal drive through Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="groups"></a><span data-ttu-id="ff3e1-207">Grupos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-207">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="ff3e1-208">Permissões para grupos e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ff3e1-208">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="ff3e1-209">O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-209">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="ff3e1-210">As permissões do aplicativo devem ser consentidas por um administrador.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-210">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="ff3e1-211">No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-211">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="ff3e1-p119">Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p119">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="ff3e1-214">Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-214">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="ff3e1-215">Criar e excluir grupos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-215">Creating and deleting groups</span></span>
* <span data-ttu-id="ff3e1-216">Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-216">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="ff3e1-217">[Definições do diretório](/graph/api/resources/directoryobject), tipo e sincronização do grupo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-217">Group [directory settings](/graph/api/resources/directoryobject), type, and synchronization</span></span>
* <span data-ttu-id="ff3e1-218">Membros e proprietários de grupo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-218">Group owners and membership</span></span>
* <span data-ttu-id="ff3e1-219">Como obter conversas de grupo e threads</span><span class="sxs-lookup"><span data-stu-id="ff3e1-219">Getting group conversations and threads</span></span>

<span data-ttu-id="ff3e1-220">Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-220">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="ff3e1-221">Eventos de grupo, foto</span><span class="sxs-lookup"><span data-stu-id="ff3e1-221">Group events, photo</span></span>
* <span data-ttu-id="ff3e1-222">Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-222">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="ff3e1-223">Favoritos do usuário e contagem de não vistos</span><span class="sxs-lookup"><span data-stu-id="ff3e1-223">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="ff3e1-224">Política</span><span class="sxs-lookup"><span data-stu-id="ff3e1-224">Policy</span></span>

<span data-ttu-id="ff3e1-225">Usar o Microsoft Graph para criar e nomear um grupo do Microsoft 365 ignora qualquer política de grupo do Microsoft 365 configurada por meio do Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-225">Using Microsoft Graph to create and name a Microsoft 365 group bypasses any Microsoft 365 group policies that are configured through Outlook on the web.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="ff3e1-226">Definir a propriedade allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="ff3e1-226">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="ff3e1-227">Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-227">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="ff3e1-228">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="ff3e1-228">Using delta query</span></span>

<span data-ttu-id="ff3e1-229">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-229">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="identity-and-access--application-and-service-principal-apis"></a><span data-ttu-id="ff3e1-230">Identidade e acesso | APIs da entidade de serviço e aplicativo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-230">Identity and access | Application and service principal APIs</span></span>

<span data-ttu-id="ff3e1-p120">Há alterações para as entidades [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p120">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="ff3e1-233">Limitações atuais:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-233">Current limitations:</span></span>

* <span data-ttu-id="ff3e1-234">Algumas propriedades do aplicativo (como appRoles e addIns) não estarão disponíveis até que todas as alterações sejam concluídas.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-234">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="ff3e1-235">Somente aplicativos multilocatários podem ser registrados.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-235">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="ff3e1-236">Atualizar aplicativos é restrito aos aplicativos registrados após a atualização inicial beta.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-236">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="ff3e1-237">Usuários do Azure Active Directory podem registrar aplicativos e adicionar proprietários adicionais.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-237">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="ff3e1-238">Suporte para protocolos OpenID Connect e OAuth.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-238">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="ff3e1-239">Atribuições de política para uma falha de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-239">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="ff3e1-240">Falha em operações em ownedObjects que exigem appId (por exemplo, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-240">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="ff3e1-241">Em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-241">In development:</span></span>

* <span data-ttu-id="ff3e1-242">Capacidade de registrar aplicativos de um único locatário.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-242">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="ff3e1-243">Atualizações para o servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-243">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="ff3e1-244">Migração de aplicativos Azure AD existentes para um modelo atualizado.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-244">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="ff3e1-245">Suporte para appRoles, clientes pré-autorizados, reivindicações opcionais, reivindicações de associação de grupo e identidade visual.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-245">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="ff3e1-246">Os usuários de conta Microsoft (MSA) podem registrar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-246">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="ff3e1-247">Suporte para protocolos SAML e WsFed.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-247">Support for SAML and WsFed protocols.</span></span>

## <a name="identity-and-access--conditional-access"></a><span data-ttu-id="ff3e1-248">Identidade e acesso | Acesso condicional</span><span class="sxs-lookup"><span data-stu-id="ff3e1-248">Identity and access | Conditional access</span></span>

### <a name="permissions"></a><span data-ttu-id="ff3e1-249">Permissões</span><span class="sxs-lookup"><span data-stu-id="ff3e1-249">Permissions</span></span>

<span data-ttu-id="ff3e1-250">Atualmente, a permissão Policy.Read.All é necessária para chamar as APIs POST e PATCH.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-250">Currently, the Policy.Read.All permission is required to call POST and PATCH APIs.</span></span> <span data-ttu-id="ff3e1-251">No futuro, a permissão Policy.ReadWrite.ConditionalAccess possibilitará que você leia as políticas do diretório.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-251">In the future, the Policy.ReadWrite.ConditionalAccess permission will enable you to read policies from the directory.</span></span>

## <a name="json-batching"></a><span data-ttu-id="ff3e1-252">Envio em lote JSON</span><span class="sxs-lookup"><span data-stu-id="ff3e1-252">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="ff3e1-253">Nenhum lote aninhado</span><span class="sxs-lookup"><span data-stu-id="ff3e1-253">No nested batch</span></span>

<span data-ttu-id="ff3e1-254">Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-254">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="ff3e1-255">Todas as solicitações individuais devem ser síncronas</span><span class="sxs-lookup"><span data-stu-id="ff3e1-255">All individual requests must be synchronous</span></span>

<span data-ttu-id="ff3e1-p122">Todas as solicitações contidas em uma solicitação de lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p122">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="ff3e1-258">Sem transações</span><span class="sxs-lookup"><span data-stu-id="ff3e1-258">No transactions</span></span>

<span data-ttu-id="ff3e1-p123">No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade `atomicityGroup` em solicitações individuais será ignorada.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p123">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="ff3e1-261">URIs devem ser relativas</span><span class="sxs-lookup"><span data-stu-id="ff3e1-261">URIs must be relative</span></span>

<span data-ttu-id="ff3e1-p124">Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p124">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="ff3e1-264">Limite de tamanho de lote</span><span class="sxs-lookup"><span data-stu-id="ff3e1-264">Limit on batch size</span></span>

<span data-ttu-id="ff3e1-265">No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-265">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="ff3e1-266">Dependências simplificadas</span><span class="sxs-lookup"><span data-stu-id="ff3e1-266">Simplified dependencies</span></span>

<span data-ttu-id="ff3e1-p125">Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p125">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="ff3e1-269">Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-269">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="ff3e1-270">Serial – todas as solicitações individuais dependem da solicitação individual anterior.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-270">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="ff3e1-271">Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-271">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="ff3e1-272">Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-272">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="mail-outlook"></a><span data-ttu-id="ff3e1-273">Email (Outlook)</span><span class="sxs-lookup"><span data-stu-id="ff3e1-273">Mail (Outlook)</span></span>

### <a name="attaching-large-files-to-messages"></a><span data-ttu-id="ff3e1-274">Anexando grandes arquivos a mensagens</span><span class="sxs-lookup"><span data-stu-id="ff3e1-274">Attaching large files to messages</span></span>
<span data-ttu-id="ff3e1-275">Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-275">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="ff3e1-276">Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-276">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="ff3e1-277">O parâmetro de comentário para criar um rascunho</span><span class="sxs-lookup"><span data-stu-id="ff3e1-277">The comment parameter for creating a draft</span></span>

<span data-ttu-id="ff3e1-278">O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) não se torna parte do corpo do rascunho de mensagem resultante.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-278">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="ff3e1-279">As mensagens GET retornam chats no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="ff3e1-279">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="ff3e1-280">Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-280">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="ff3e1-281">Essas mensagens de chat tem "IM" como o assunto.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-281">These chat messages have "IM" as their subject.</span></span>

## <a name="teamwork-microsoft-teams"></a><span data-ttu-id="ff3e1-282">Trabalho em equipe (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="ff3e1-282">Teamwork (Microsoft Teams)</span></span>

### <a name="get-teams-is-not-supported"></a><span data-ttu-id="ff3e1-283">GET /teams não tem suporte</span><span class="sxs-lookup"><span data-stu-id="ff3e1-283">GET /teams is not supported</span></span>

<span data-ttu-id="ff3e1-284">Para obter uma lista de equipes, confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-284">To get a list of teams, see [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams).</span></span>

### <a name="unable-to-filter-team-members-by-roles"></a><span data-ttu-id="ff3e1-285">Não é possível filtrar os membros da equipe por funções</span><span class="sxs-lookup"><span data-stu-id="ff3e1-285">Unable to filter team members by roles</span></span>
<span data-ttu-id="ff3e1-286">A consulta de filtro para obter membros de uma equipe com base em suas funções `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')`pode não funcionar.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-286">The filter query to get members of a team based on their roles `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')` might not work.</span></span> <span data-ttu-id="ff3e1-287">O servidor pode responder com uma.`BAD REQUEST`</span><span class="sxs-lookup"><span data-stu-id="ff3e1-287">The server might respond with a `BAD REQUEST`.</span></span>

### <a name="missing-properties-for-chat-members"></a><span data-ttu-id="ff3e1-288">Propriedades ausentes para membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="ff3e1-288">Missing properties for chat members</span></span>
<span data-ttu-id="ff3e1-289">Em certos casos, a `tenantId` / `email` / `displayName` propriedade para os membros individuais de um bate-papo pode não ser preenchida em uma solicitação `GET /chats/chat-id/members` ou `GET /chats/chat-id/members/membership-id`.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-289">In certain instances, the `tenantId` / `email` / `displayName` property for the individual members of a chat might not be populated on a `GET /chats/chat-id/members` or `GET /chats/chat-id/members/membership-id` request.</span></span>

## <a name="users"></a><span data-ttu-id="ff3e1-290">Usuários</span><span class="sxs-lookup"><span data-stu-id="ff3e1-290">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="ff3e1-291">Sem acesso instantâneo após a criação</span><span class="sxs-lookup"><span data-stu-id="ff3e1-291">No instant access after creation</span></span>

<span data-ttu-id="ff3e1-292">Os usuários podem ser criados imediatamente por um POST na entidade do usuário.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-292">Users can be created immediately through a POST on the user entity.</span></span> <span data-ttu-id="ff3e1-293">Uma licença do Microsoft 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-293">A Microsoft 365 license must first be assigned to a user, in order to get access to Microsoft 365 services.</span></span> <span data-ttu-id="ff3e1-294">Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-294">Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API.</span></span> <span data-ttu-id="ff3e1-295">Durante esse período, os aplicativos receberão uma resposta de erro 404 HTTP.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-295">During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="ff3e1-296">Restrições de foto</span><span class="sxs-lookup"><span data-stu-id="ff3e1-296">Photo restrictions</span></span>

<span data-ttu-id="ff3e1-297">A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-297">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span></span> <span data-ttu-id="ff3e1-298">Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis por meio da propriedade **foto** do recurso [usuário](/graph/api/resources/user) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-298">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Azure AD Graph or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user) resource.</span></span>
<span data-ttu-id="ff3e1-299">A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-299">Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a><span data-ttu-id="ff3e1-300">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="ff3e1-300">Using delta query</span></span>

<span data-ttu-id="ff3e1-301">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-301">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a><span data-ttu-id="ff3e1-302">A revogação de sessões de entrada retorna um código HTTP errado</span><span class="sxs-lookup"><span data-stu-id="ff3e1-302">Revoke sign-in sessions returns wrong HTTP code</span></span>

<span data-ttu-id="ff3e1-303">O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-303">The [user: revokeSignInSessions API](/graph/api/user-revokesigninsessions) should return a `204 No content` response for successful revocations, and an HTTP error code (4xx or 5xx) if anything goes wrong with the request.</span></span>  <span data-ttu-id="ff3e1-304">No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre true.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-304">However, due to a service issue, this API returns a `200 OK` and a Boolean parameter that is always true.</span></span>  <span data-ttu-id="ff3e1-305">Até que isso seja corrigido, é recomendado que desenvolvedores simplesmente tratem qualquer código de retorno 2xx como bem-sucedido para esta API.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-305">Until this is fixed, developers are simply advised to treat any 2xx return code as success for this API.</span></span>

### <a name="incomplete-objects-when-using-getbyids-request"></a><span data-ttu-id="ff3e1-306">Objetos incompletos ao usar a solicitação getByIds</span><span class="sxs-lookup"><span data-stu-id="ff3e1-306">Incomplete objects when using getByIds request</span></span>

<span data-ttu-id="ff3e1-307">A solicitação de objetos usando a opção de [Obter objetos de diretório de uma lista de IDs](/graph/api/directoryobject-getbyids) deve retornar objetos completos.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-307">Requesting objects using [Get directory objects from a list of IDs](/graph/api/directoryobject-getbyids) should return full objects.</span></span> <span data-ttu-id="ff3e1-308">No entanto, atualmente, os objetos de [usuário](/graph/api/resources/user) no ponto de extremidade v1.0 são retornados com um conjunto limitado de propriedades.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-308">However, currently [user](/graph/api/resources/user) objects on the v1.0 endpoint are returned with a limited set of properties.</span></span> <span data-ttu-id="ff3e1-309">Como solução temporária, ao usar a operação em combinação com a opção de consulta `$select`, objetos de [usuário](/graph/api/resources/user) mais completos serão retornados.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-309">As a temporary workaround, when you use the operation in combination with the `$select` query option, more complete [user](/graph/api/resources/user) objects will be returned.</span></span> <span data-ttu-id="ff3e1-310">Esse comportamento não está de acordo com as especificações do OData.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-310">This behavior is not in accordance with the OData specifications.</span></span> <span data-ttu-id="ff3e1-311">Como esse comportamento pode ser atualizado no futuro, use esta solução alternativa apenas quando fornecer `$select=` com todas as propriedades de seu interesse e somente se futuras alterações nessa solução alternativa forem aceitáveis.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-311">Because this behavior might be updated in the future, use this workaround only when you provide `$select=` with all the properties you are interested in, and only if future breaking changes to this workaround are acceptable.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="ff3e1-312">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="ff3e1-312">Query parameter limitations</span></span>

* <span data-ttu-id="ff3e1-313">Não há suporte para vários namespaces.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-313">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="ff3e1-314">Não há suporte para GETs no `$ref` e também para transmissão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-314">GETs on `$ref` and casting are not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="ff3e1-p133">`@odata.bind` não é compatível. Isso significa que os desenvolvedores não poderão definir corretamente a propriedade de navegação **acceptedSenders** ou **rejectedSenders** em um grupo.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-p133">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span></span>
* <span data-ttu-id="ff3e1-317">`@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-317">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="ff3e1-318">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-318">`$expand`:</span></span>
  * <span data-ttu-id="ff3e1-319">Não há suporte para `nextLink`</span><span class="sxs-lookup"><span data-stu-id="ff3e1-319">No support for `nextLink`</span></span>
  * <span data-ttu-id="ff3e1-320">Não há suporte para mais de um nível de expansão</span><span class="sxs-lookup"><span data-stu-id="ff3e1-320">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="ff3e1-321">Não há suporte com parâmetros adicionais (`$filter`, `$select`)</span><span class="sxs-lookup"><span data-stu-id="ff3e1-321">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="ff3e1-322">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-322">`$filter`:</span></span>
  * <span data-ttu-id="ff3e1-323">Não há suporte para filtros no ponto de extremidade `/attachments`.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-323">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="ff3e1-324">Se presente, o parâmetro `$filter` é ignorado.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-324">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="ff3e1-325">Não há suporte para filtragem de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-325">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="ff3e1-326">`$search`:</span><span class="sxs-lookup"><span data-stu-id="ff3e1-326">`$search`:</span></span>
  * <span data-ttu-id="ff3e1-327">A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-327">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="ff3e1-328">Não há suporte para pesquisa de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-328">Cross-workload searching is not supported.</span></span>


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="ff3e1-329">Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365</span><span class="sxs-lookup"><span data-stu-id="ff3e1-329">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="ff3e1-330">Alguns recursos ainda não estão disponíveis no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-330">Some functionality is not yet available in Microsoft Graph.</span></span> <span data-ttu-id="ff3e1-331">Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](/previous-versions/office/office-365-api/) específicas do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="ff3e1-331">If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](/previous-versions/office/office-365-api/).</span></span> <span data-ttu-id="ff3e1-332">Para o Azure Active Directory, confira [Migrar aplicativos do Azure AD Graph para o Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="ff3e1-332">For Azure Active Directory, see [Migrate Azure AD Graph apps to Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).</span></span>
