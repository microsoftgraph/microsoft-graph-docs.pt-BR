---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos com o Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 257d8966eabe2428072f470f290816a1c9c2e35d
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351105"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="2ce82-103">Problemas conhecidos com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2ce82-103">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="2ce82-104">Este artigo descreve os problemas conhecidos com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ce82-104">This article describes known issues with Microsoft Graph.</span></span> 

<span data-ttu-id="2ce82-105">Para relatar um problema conhecido, confira a página [Suporte Microsoft Graph](https://developer.microsoft.com/graph/support).</span><span class="sxs-lookup"><span data-stu-id="2ce82-105">To report a known issue, see the [Microsoft Graph support](https://developer.microsoft.com/graph/support) page.</span></span>

<span data-ttu-id="2ce82-106">Para saber mais sobre as atualizações mais recentes da API do Microsoft Graph, confira o [changelog do Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="2ce82-106">For information about the latest updates to the Microsoft Graph API, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="bookings"></a><span data-ttu-id="2ce82-107">Reservas</span><span class="sxs-lookup"><span data-stu-id="2ce82-107">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="2ce82-108">ErrorExceededFindCountLimit ao consultar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="2ce82-108">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="2ce82-109">A obtenção da lista de `bookingBusinesses` falha com o seguinte código de erro quando a organização tem várias empresas de Reservas e a conta que está fazendo a solicitação não é um administrador:</span><span class="sxs-lookup"><span data-stu-id="2ce82-109">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="2ce82-110">Como alternativa, você pode limitar o conjunto de empresas retornadas pela solicitação, incluindo um parâmetro `query`, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="2ce82-110">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```http
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a><span data-ttu-id="2ce82-111">Calendários</span><span class="sxs-lookup"><span data-stu-id="2ce82-111">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="2ce82-112">Acessar um calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="2ce82-112">Accessing a shared calendar</span></span>

<span data-ttu-id="2ce82-113">Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:</span><span class="sxs-lookup"><span data-stu-id="2ce82-113">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET /users/{id}/calendars/{id}/events
```

<span data-ttu-id="2ce82-p101">Você pode receber HTTP 500 com o código de erro `ErrorInternalServerTransientError`. O erro ocorre porque:</span><span class="sxs-lookup"><span data-stu-id="2ce82-p101">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`. The error occurs because:</span></span>

- <span data-ttu-id="2ce82-116">Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.</span><span class="sxs-lookup"><span data-stu-id="2ce82-116">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="2ce82-117">A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.</span><span class="sxs-lookup"><span data-stu-id="2ce82-117">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="2ce82-118">Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.</span><span class="sxs-lookup"><span data-stu-id="2ce82-118">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="2ce82-119">Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.</span><span class="sxs-lookup"><span data-stu-id="2ce82-119">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="2ce82-120">Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.</span><span class="sxs-lookup"><span data-stu-id="2ce82-120">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="2ce82-121">Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="2ce82-121">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="2ce82-122">Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="2ce82-122">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="2ce82-123">O destinatário remove o calendário previamente compartilhado com ele.</span><span class="sxs-lookup"><span data-stu-id="2ce82-123">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="2ce82-124">O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="2ce82-124">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="2ce82-p103">O destinatário aceita novamente o calendário compartilhado usando o Outlook na Web. Em breve você poderá usar outros clientes do Outlook.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p103">The recipient re-accepts the shared calendar using Outlook on the web. (It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="2ce82-127">O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="2ce82-127">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="2ce82-p104">Um calendário compartilhado com você na nova abordagem é exibido como qualquer outro na sua caixa de correio. Você pode usar a API REST de calendário para visualizar e editar eventos no calendário compartilhado, como se fosse seu próprio calendário. Como exemplo:</span><span class="sxs-lookup"><span data-stu-id="2ce82-p104">A calendar shared with you in the new approach appears as just another calendar in your mailbox. You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar. As an example:</span></span>

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="2ce82-131">Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="2ce82-131">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="2ce82-132">Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):</span><span class="sxs-lookup"><span data-stu-id="2ce82-132">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="2ce82-133">Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ce82-133">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="2ce82-p105">[Listar os calendários do usuário](/graph/api/user-list-calendars) permite que você obtenha as propriedades **name**, **color** e **id** de cada [calendar](/graph/api/resources/calendar) no grupo de calendários padrão do usuário ou em um grupo de calendários especificado, inclusive todos os calendários com base em ICS. Não é possível armazenar ou acessar a URL da ICS no recurso de calendário.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p105">[Listing the user's calendars](/graph/api/user-list-calendars) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars. You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="2ce82-136">Você também pode [listar os eventos](/graph/api/calendar-list-events) de um calendário baseado em ICS.</span><span class="sxs-lookup"><span data-stu-id="2ce82-136">You can also [list the events](/graph/api/calendar-list-events) of an ICS-based calendar.</span></span>

### <a name="attaching-large-files-to-events"></a><span data-ttu-id="2ce82-137">Anexar arquivos grandes a eventos</span><span class="sxs-lookup"><span data-stu-id="2ce82-137">Attaching large files to events</span></span>
<span data-ttu-id="2ce82-138">Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-138">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="2ce82-139">Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2ce82-139">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="2ce82-140">Suporte de propriedade onlineMeetingUrl do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2ce82-140">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="2ce82-141">Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event) de reunião do Skype indica a URL da reunião online.</span><span class="sxs-lookup"><span data-stu-id="2ce82-141">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event) would indicate the online meeting URL.</span></span> <span data-ttu-id="2ce82-142">No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.</span><span class="sxs-lookup"><span data-stu-id="2ce82-142">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

<span data-ttu-id="2ce82-143">A versão beta oferece uma solução alternativa, na qual é possível usar a propriedade **onlineMeetingProvider** de um [evento](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true)para verificar se o provedor é o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2ce82-143">The beta version offers a workaround, where you can use the **onlineMeetingProvider** property of an [event](/graph/api/resources/event?view=graph-rest-beta&preserve-view=true) to verify if the provider is Microsoft Teams.</span></span> <span data-ttu-id="2ce82-144">Por meio da propriedade **onlineMeeting** do **evento**, você pode acessar o **joinUrl**.</span><span class="sxs-lookup"><span data-stu-id="2ce82-144">Through the **onlineMeeting** property of the **event**, you can access the **joinUrl**.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="2ce82-145">Notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="2ce82-145">Change notifications</span></span>

### <a name="additional-notifications-for-users"></a><span data-ttu-id="2ce82-146">Notificações adicionais para usuários</span><span class="sxs-lookup"><span data-stu-id="2ce82-146">Additional notifications for users</span></span>

<span data-ttu-id="2ce82-147">As [assinaturas](/graph/api/resources/subscription) de alterações para o **usuário** com o **changeType** definido como **atualizado** também receberão notificações de **changeType**: **atualizado** na criação do usuário e exclusão reversível do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ce82-147">[Subscriptions](/graph/api/resources/subscription) to changes for **user** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on user creation and user soft deletion.</span></span>

### <a name="additional-notifications-for-groups"></a><span data-ttu-id="2ce82-148">Notificações adicionais para grupos</span><span class="sxs-lookup"><span data-stu-id="2ce82-148">Additional notifications for groups</span></span>

<span data-ttu-id="2ce82-149">As [assinaturas](/graph/api/resources/subscription) de alterações no **grupo** com o **changeType** definido como **atualizado** também receberão notificações **changeType**: **atualizado** na criação do grupo e exclusão reversível do grupo.</span><span class="sxs-lookup"><span data-stu-id="2ce82-149">[Subscriptions](/graph/api/resources/subscription) to changes for **group** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on group creation and group soft deletion.</span></span>

## <a name="cloud-communications"></a><span data-ttu-id="2ce82-150">Comunicações na nuvem</span><span class="sxs-lookup"><span data-stu-id="2ce82-150">Cloud communications</span></span> 

<span data-ttu-id="2ce82-151">O cliente do Microsoft Teams não mostra o menu **Exibir detalhes da Reunião** para reuniões de canal criadas por meio da API de comunicações na nuvem.</span><span class="sxs-lookup"><span data-stu-id="2ce82-151">The Microsoft Teams client does not show the **View Meeting details**  menu for channel meetings created via the cloud communications API.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="2ce82-152">Aplicativos de Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="2ce82-152">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="2ce82-153">Os aplicativos CSP devem usar o ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="2ce82-153">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="2ce82-p109">Aplicativos de provedor de solução de nuvem (CSP) devem adquirir tokens de pontos de extremidade do Azure AD (v1) para chamar a Microsoft Graph com êxito em seus clientes gerenciados por parceiros. Atualmente, não há suporte para aquisição de um token pelo ponto de extremidade Azure AD v 2.0 mais recente.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p109">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers. Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="2ce82-156">A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente</span><span class="sxs-lookup"><span data-stu-id="2ce82-156">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="2ce82-157">Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="2ce82-157">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="2ce82-158">Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-158">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="2ce82-159">Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ce82-159">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="2ce82-160">Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="2ce82-160">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="2ce82-161">Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="2ce82-161">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="2ce82-p110">**OBSERVAÇÃO:** esta não é uma solução permanente e destina-se apenas a desbloquear o desenvolvimento.  Esta solução alternativa não será necessária uma vez que a questão acima mencionada seja corrigida.  Esta solução alternativa não precisa ser desfeita após a correção.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p110">**NOTE:** This is not a permanent solution and is only intended to unblock development.  This workaround will not be required once the aforementioned issue is fixed.  This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="2ce82-p111">Abra uma sessão do Azure AD v2 PowerShell e conecte-se ao locatário do parceiro `customer`digitando suas credenciais de administrador na janela de entrada. Você pode baixar e instalar o Azure AD PowerShell V2 [aqui](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="2ce82-p111">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window. You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="2ce82-167">Crie o servicePrincipal do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ce82-167">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a><span data-ttu-id="2ce82-168">Contatos</span><span class="sxs-lookup"><span data-stu-id="2ce82-168">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="2ce82-169">Contatos de organização disponíveis somente na versão beta</span><span class="sxs-lookup"><span data-stu-id="2ce82-169">Organization contacts available in only beta</span></span>

<span data-ttu-id="2ce82-p112">Somente os contatos pessoais têm suporte no momento. Os contatos organizacionais atualmente não têm suporte na `/v1.0`, mas podem ser encontrados na versão `/beta`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p112">Only personal contacts are currently supported. Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="2ce82-172">Pasta Contatos padrão</span><span class="sxs-lookup"><span data-stu-id="2ce82-172">Default contacts folder</span></span>

<span data-ttu-id="2ce82-173">Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="2ce82-173">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="2ce82-p113">Uma correção será disponibilizada. Enquanto isso, você pode usar a seguinte consulta [list contacts](/graph/api/user-list-contacts) e a propriedade **parentFolderId** como uma solução alternativa para obter a ID da pasta de contatos padrão:</span><span class="sxs-lookup"><span data-stu-id="2ce82-p113">A fix will be made available. Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="2ce82-176">Na consulta acima:</span><span class="sxs-lookup"><span data-stu-id="2ce82-176">In the above query:</span></span>

1. <span data-ttu-id="2ce82-177">`/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact) na pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="2ce82-177">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact) in the default contacts folder.</span></span>
2. <span data-ttu-id="2ce82-178">A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="2ce82-178">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="2ce82-179">Acessar contatos por meio de uma pasta de contatos na versão beta</span><span class="sxs-lookup"><span data-stu-id="2ce82-179">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="2ce82-180">Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.</span><span class="sxs-lookup"><span data-stu-id="2ce82-180">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta&preserve-view=true) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="2ce82-181">Acessando um contato a partir de um nível superior do [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) do usuário.</span><span class="sxs-lookup"><span data-stu-id="2ce82-181">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta&preserve-view=true) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="2ce82-p114">Acessando um contato contido em uma pasta filha de um **contactFolder**.  O exemplo a seguir mostra um nível de aninhamento, mas um contato pode estar localizado em um filho de um filho e assim por diante.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p114">Accessing a contact contained in a child folder of a **contactFolder**.  The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolders/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="2ce82-184">Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="2ce82-184">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta&preserve-view=true) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a><span data-ttu-id="2ce82-185">Consulta delta</span><span class="sxs-lookup"><span data-stu-id="2ce82-185">Delta query</span></span>

* <span data-ttu-id="2ce82-186">O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.</span><span class="sxs-lookup"><span data-stu-id="2ce82-186">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="2ce82-187">As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.</span><span class="sxs-lookup"><span data-stu-id="2ce82-187">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="2ce82-188">Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.</span><span class="sxs-lookup"><span data-stu-id="2ce82-188">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="devices-and-apps--device-updates-windows-updates"></a><span data-ttu-id="2ce82-189">Dispositivos e aplicativos | Atualizações do dispositivo (atualizações do Windows)</span><span class="sxs-lookup"><span data-stu-id="2ce82-189">Devices and apps | Device updates (Windows updates)</span></span>

### <a name="accessing-and-updating-deployment-audiences"></a><span data-ttu-id="2ce82-190">Acessando e atualizando audiências de implantação</span><span class="sxs-lookup"><span data-stu-id="2ce82-190">Accessing and updating deployment audiences</span></span>

<span data-ttu-id="2ce82-191">Acessando e atualizando audiências de implantação em recursos de **implantação** criados por meio do Intune não são suportados atualmente.</span><span class="sxs-lookup"><span data-stu-id="2ce82-191">Accessing and updating deployment audiences on **deployment** resources created via Intune is not currently supported.</span></span>

* <span data-ttu-id="2ce82-192">[Listando membros da audiência de implantação](/graph/api/windowsupdates-deploymentaudience-list-members) e [listando exclusões da audiência de implantação](/graph/api/windowsupdates-deploymentaudience-list-exclusions) retornos `404 Not Found`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-192">[Listing deployment audience members](/graph/api/windowsupdates-deploymentaudience-list-members) and [listing deployment audience exclusions](/graph/api/windowsupdates-deploymentaudience-list-exclusions) returns `404 Not Found`.</span></span>
* <span data-ttu-id="2ce82-193">[Atualizar membros da audiência de implantação e exclusões](/graph/api/windowsupdates-deploymentaudience-updateaudience) ou [atualizar por ID](/graph/api/windowsupdates-deploymentaudience-updateaudiencebyid) retorna `202 Accepted`, mas a audiência não é atualizada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-193">[Updating deployment audience members and exclusions](/graph/api/windowsupdates-deploymentaudience-updateaudience) or [updating by ID](/graph/api/windowsupdates-deploymentaudience-updateaudiencebyid) returns `202 Accepted` but the audience is not updated.</span></span>

## <a name="extensions"></a><span data-ttu-id="2ce82-194">Extensões</span><span class="sxs-lookup"><span data-stu-id="2ce82-194">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="2ce82-195">Não há suporte para o controle de alterações</span><span class="sxs-lookup"><span data-stu-id="2ce82-195">Change tracking is not supported</span></span>

<span data-ttu-id="2ce82-196">O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.</span><span class="sxs-lookup"><span data-stu-id="2ce82-196">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="2ce82-197">Criar um recurso e uma extensão aberta ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="2ce82-197">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="2ce82-p115">Você não pode especificar uma extensão aberta ao mesmo tempo que cria uma instância de **administrativeUnit**, **device**, **group**, **organization** ou **user**. Primeiro você deve criar a instância e, depois, especificar os dados da extensão aberta em uma solicitação ``POST`` subsequente nessa instância.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p115">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**. You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="2ce82-200">Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="2ce82-200">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="2ce82-201">Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="2ce82-201">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="2ce82-202">Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="2ce82-202">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="2ce82-203">Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos</span><span class="sxs-lookup"><span data-stu-id="2ce82-203">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="2ce82-204">Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.</span><span class="sxs-lookup"><span data-stu-id="2ce82-204">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="updating-a-schemaextension-definition-using-microsoft-graph-explorer"></a><span data-ttu-id="2ce82-205">Atualizar uma definição de schemaExtension usando o Microsoft Graph Explorer</span><span class="sxs-lookup"><span data-stu-id="2ce82-205">Updating a schemaExtension definition using Microsoft Graph Explorer</span></span>

<span data-ttu-id="2ce82-206">Ao usar `PATCH` para atualizar uma schemaExtension usando o Graph Explorer, você deve especificar a propriedade de **proprietário** e defini-la com seu valor `appid` atual (que será necessário ser uma `appId` de um aplicativo que você tenha).</span><span class="sxs-lookup"><span data-stu-id="2ce82-206">When using `PATCH` to update a schemaExtension using Graph Explorer, you must specify the **owner** property and set it to its current `appid` value (which will need to be an `appId` of an application that you own).</span></span> <span data-ttu-id="2ce82-207">Esse também é o caso de qualquer aplicativo de cliente que `appId` não seja o mesmo que o do **proprietário**.</span><span class="sxs-lookup"><span data-stu-id="2ce82-207">This is also the case for any client application whose `appId` is not the same as the **owner**.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="2ce82-208">Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="2ce82-208">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="2ce82-209">Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="2ce82-209">Filtering on schema extension properties (using the `$filter` expression) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="files-onedrive"></a><span data-ttu-id="2ce82-210">Arquivos (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="2ce82-210">Files (OneDrive)</span></span>

* <span data-ttu-id="2ce82-211">O primeiro acesso a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse o próprio site pessoal por um navegador resulta em uma resposta 401.</span><span class="sxs-lookup"><span data-stu-id="2ce82-211">First time access to a user's personal drive through Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="groups"></a><span data-ttu-id="2ce82-212">Grupos</span><span class="sxs-lookup"><span data-stu-id="2ce82-212">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="2ce82-213">Permissões para grupos e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2ce82-213">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="2ce82-214">O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2ce82-214">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="2ce82-215">As permissões do aplicativo devem ser consentidas por um administrador.</span><span class="sxs-lookup"><span data-stu-id="2ce82-215">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="2ce82-216">No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="2ce82-216">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="2ce82-p119">Além disso, somente a API para administração de grupo principal e gerenciamento suporta acesso usando permissões delegadas ou somente para aplicativos. Todos os outros recursos da API do grupo dão suporte apenas a permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p119">Also, only the API for core group administration and management supports access using delegated or app-only permissions. All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="2ce82-219">Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="2ce82-219">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="2ce82-220">Criar e excluir grupos</span><span class="sxs-lookup"><span data-stu-id="2ce82-220">Creating and deleting groups</span></span>
* <span data-ttu-id="2ce82-221">Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo</span><span class="sxs-lookup"><span data-stu-id="2ce82-221">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="2ce82-222">[Definições do diretório](/graph/api/resources/directoryobject), tipo e sincronização do grupo</span><span class="sxs-lookup"><span data-stu-id="2ce82-222">Group [directory settings](/graph/api/resources/directoryobject), type, and synchronization</span></span>
* <span data-ttu-id="2ce82-223">Membros e proprietários de grupo</span><span class="sxs-lookup"><span data-stu-id="2ce82-223">Group owners and membership</span></span>
* <span data-ttu-id="2ce82-224">Como obter conversas de grupo e threads</span><span class="sxs-lookup"><span data-stu-id="2ce82-224">Getting group conversations and threads</span></span>

<span data-ttu-id="2ce82-225">Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:</span><span class="sxs-lookup"><span data-stu-id="2ce82-225">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="2ce82-226">Eventos de grupo, foto</span><span class="sxs-lookup"><span data-stu-id="2ce82-226">Group events, photo</span></span>
* <span data-ttu-id="2ce82-227">Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo</span><span class="sxs-lookup"><span data-stu-id="2ce82-227">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="2ce82-228">Favoritos do usuário e contagem de não vistos</span><span class="sxs-lookup"><span data-stu-id="2ce82-228">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="2ce82-229">Política</span><span class="sxs-lookup"><span data-stu-id="2ce82-229">Policy</span></span>

<span data-ttu-id="2ce82-230">Usar o Microsoft Graph para criar e nomear um grupo do Microsoft 365 ignora qualquer política de grupo do Microsoft 365 configurada por meio do Outlook na Web.</span><span class="sxs-lookup"><span data-stu-id="2ce82-230">Using Microsoft Graph to create and name a Microsoft 365 group bypasses any Microsoft 365 group policies that are configured through Outlook on the web.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="2ce82-231">Definir a propriedade allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="2ce82-231">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="2ce82-232">Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-232">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="2ce82-233">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="2ce82-233">Using delta query</span></span>

<span data-ttu-id="2ce82-234">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="2ce82-234">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="identity-and-access--application-and-service-principal-apis"></a><span data-ttu-id="2ce82-235">Identidade e acesso | APIs da entidade de serviço e aplicativo</span><span class="sxs-lookup"><span data-stu-id="2ce82-235">Identity and access | Application and service principal APIs</span></span>

<span data-ttu-id="2ce82-p120">Há alterações para as entidades [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) e [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) atualmente em desenvolvimento. A seguir, encontra-se um resumo das limitações atuais e os recursos da API em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="2ce82-p120">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta&preserve-view=true) entities currently in development. The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="2ce82-238">Limitações atuais:</span><span class="sxs-lookup"><span data-stu-id="2ce82-238">Current limitations:</span></span>

* <span data-ttu-id="2ce82-239">Algumas propriedades do aplicativo (como appRoles e addIns) não estarão disponíveis até que todas as alterações sejam concluídas.</span><span class="sxs-lookup"><span data-stu-id="2ce82-239">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="2ce82-240">Somente aplicativos multilocatários podem ser registrados.</span><span class="sxs-lookup"><span data-stu-id="2ce82-240">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="2ce82-241">Atualizar aplicativos é restrito aos aplicativos registrados após a atualização inicial beta.</span><span class="sxs-lookup"><span data-stu-id="2ce82-241">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="2ce82-242">Usuários do Azure Active Directory podem registrar aplicativos e adicionar proprietários adicionais.</span><span class="sxs-lookup"><span data-stu-id="2ce82-242">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="2ce82-243">Suporte para protocolos OpenID Connect e OAuth.</span><span class="sxs-lookup"><span data-stu-id="2ce82-243">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="2ce82-244">Atribuições de política para uma falha de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="2ce82-244">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="2ce82-245">Falha em operações em ownedObjects que exigem appId (por exemplo, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="2ce82-245">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="2ce82-246">Em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="2ce82-246">In development:</span></span>

* <span data-ttu-id="2ce82-247">Capacidade de registrar aplicativos de um único locatário.</span><span class="sxs-lookup"><span data-stu-id="2ce82-247">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="2ce82-248">Atualizações para o servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="2ce82-248">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="2ce82-249">Migração de aplicativos Azure AD existentes para um modelo atualizado.</span><span class="sxs-lookup"><span data-stu-id="2ce82-249">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="2ce82-250">Suporte para appRoles, clientes pré-autorizados, reivindicações opcionais, reivindicações de associação de grupo e identidade visual.</span><span class="sxs-lookup"><span data-stu-id="2ce82-250">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="2ce82-251">Os usuários de conta Microsoft (MSA) podem registrar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="2ce82-251">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="2ce82-252">Suporte para protocolos SAML e WsFed.</span><span class="sxs-lookup"><span data-stu-id="2ce82-252">Support for SAML and WsFed protocols.</span></span>

## <a name="identity-and-access--conditional-access"></a><span data-ttu-id="2ce82-253">Identidade e acesso | Acesso condicional</span><span class="sxs-lookup"><span data-stu-id="2ce82-253">Identity and access | Conditional access</span></span>

### <a name="permissions"></a><span data-ttu-id="2ce82-254">Permissões</span><span class="sxs-lookup"><span data-stu-id="2ce82-254">Permissions</span></span>

<span data-ttu-id="2ce82-255">Atualmente, a permissão Policy.Read.All é necessária para chamar as APIs POST e PATCH.</span><span class="sxs-lookup"><span data-stu-id="2ce82-255">Currently, the Policy.Read.All permission is required to call POST and PATCH APIs.</span></span> <span data-ttu-id="2ce82-256">No futuro, a permissão Policy.ReadWrite.ConditionalAccess possibilitará que você leia as políticas do diretório.</span><span class="sxs-lookup"><span data-stu-id="2ce82-256">In the future, the Policy.ReadWrite.ConditionalAccess permission will enable you to read policies from the directory.</span></span>

## <a name="json-batching"></a><span data-ttu-id="2ce82-257">Envio em lote JSON</span><span class="sxs-lookup"><span data-stu-id="2ce82-257">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="2ce82-258">Nenhum lote aninhado</span><span class="sxs-lookup"><span data-stu-id="2ce82-258">No nested batch</span></span>

<span data-ttu-id="2ce82-259">Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.</span><span class="sxs-lookup"><span data-stu-id="2ce82-259">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="2ce82-260">Todas as solicitações individuais devem ser síncronas</span><span class="sxs-lookup"><span data-stu-id="2ce82-260">All individual requests must be synchronous</span></span>

<span data-ttu-id="2ce82-p122">Todas as solicitações contidas em uma solicitação de lote devem ser executadas de forma síncrona. Se estiver presente, a preferência `respond-async` será ignorada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p122">All requests contained in a batch request must be executed synchronously. If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="2ce82-263">Sem transações</span><span class="sxs-lookup"><span data-stu-id="2ce82-263">No transactions</span></span>

<span data-ttu-id="2ce82-p123">No momento o Microsoft Graph não oferece suporte a processamento transacional de solicitações individuais. A propriedade `atomicityGroup` em solicitações individuais será ignorada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p123">Microsoft Graph does not currently support transactional processing of individual requests. The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="2ce82-266">URIs devem ser relativas</span><span class="sxs-lookup"><span data-stu-id="2ce82-266">URIs must be relative</span></span>

<span data-ttu-id="2ce82-p124">Sempre especifique URIs relativas em solicitações de lote. O Microsoft Graph então torna essas URLs absolutas usando o ponto de extremidade de versão incluído na URL de lote.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p124">Always specify relative URIs in batch requests. Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="2ce82-269">Limite de tamanho de lote</span><span class="sxs-lookup"><span data-stu-id="2ce82-269">Limit on batch size</span></span>

<span data-ttu-id="2ce82-270">No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.</span><span class="sxs-lookup"><span data-stu-id="2ce82-270">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="2ce82-271">Dependências simplificadas</span><span class="sxs-lookup"><span data-stu-id="2ce82-271">Simplified dependencies</span></span>

<span data-ttu-id="2ce82-p125">Solicitações individuais podem depender de outras solicitações individuais. Atualmente, solicitações só podem depender de uma única outra solicitação e devem seguir um destes três padrões:</span><span class="sxs-lookup"><span data-stu-id="2ce82-p125">Individual requests can depend on other individual requests. Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="2ce82-274">Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-274">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="2ce82-275">Serial – todas as solicitações individuais dependem da solicitação individual anterior.</span><span class="sxs-lookup"><span data-stu-id="2ce82-275">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="2ce82-276">Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.</span><span class="sxs-lookup"><span data-stu-id="2ce82-276">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="2ce82-277">Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.</span><span class="sxs-lookup"><span data-stu-id="2ce82-277">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="mail-outlook"></a><span data-ttu-id="2ce82-278">Email (Outlook)</span><span class="sxs-lookup"><span data-stu-id="2ce82-278">Mail (Outlook)</span></span>

### <a name="attaching-large-files-to-messages"></a><span data-ttu-id="2ce82-279">Anexando grandes arquivos a mensagens</span><span class="sxs-lookup"><span data-stu-id="2ce82-279">Attaching large files to messages</span></span>
<span data-ttu-id="2ce82-280">Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-280">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="2ce82-281">Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="2ce82-281">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="2ce82-282">O parâmetro de comentário para criar um rascunho</span><span class="sxs-lookup"><span data-stu-id="2ce82-282">The comment parameter for creating a draft</span></span>

<span data-ttu-id="2ce82-283">O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) não se torna parte do corpo do rascunho de mensagem resultante.</span><span class="sxs-lookup"><span data-stu-id="2ce82-283">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply), [createReplyAll](/graph/api/message-createreplyall), [createForward](/graph/api/message-createforward)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="2ce82-284">As mensagens GET retornam chats no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="2ce82-284">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="2ce82-285">Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal.</span><span class="sxs-lookup"><span data-stu-id="2ce82-285">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="2ce82-286">Essas mensagens de chat tem "IM" como o assunto.</span><span class="sxs-lookup"><span data-stu-id="2ce82-286">These chat messages have "IM" as their subject.</span></span>

## <a name="teamwork-microsoft-teams"></a><span data-ttu-id="2ce82-287">Trabalho em equipe (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="2ce82-287">Teamwork (Microsoft Teams)</span></span>

### <a name="get-teams-is-not-supported"></a><span data-ttu-id="2ce82-288">GET /teams não tem suporte</span><span class="sxs-lookup"><span data-stu-id="2ce82-288">GET /teams is not supported</span></span>

<span data-ttu-id="2ce82-289">Para obter uma lista de equipes, confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams).</span><span class="sxs-lookup"><span data-stu-id="2ce82-289">To get a list of teams, see [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams).</span></span>

### <a name="unable-to-filter-team-members-by-roles"></a><span data-ttu-id="2ce82-290">Não é possível filtrar os membros da equipe por funções</span><span class="sxs-lookup"><span data-stu-id="2ce82-290">Unable to filter team members by roles</span></span>
<span data-ttu-id="2ce82-291">A consulta de filtro para obter membros de uma equipe com base em suas funções `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')`pode não funcionar.</span><span class="sxs-lookup"><span data-stu-id="2ce82-291">The filter query to get members of a team based on their roles `GET /teams/team-id/members?$filter=roles/any(r:r eq 'owner')` might not work.</span></span> <span data-ttu-id="2ce82-292">O servidor pode responder com uma.`BAD REQUEST`</span><span class="sxs-lookup"><span data-stu-id="2ce82-292">The server might respond with a `BAD REQUEST`.</span></span>

### <a name="missing-properties-for-chat-members"></a><span data-ttu-id="2ce82-293">Propriedades ausentes para membros do bate-papo</span><span class="sxs-lookup"><span data-stu-id="2ce82-293">Missing properties for chat members</span></span>
<span data-ttu-id="2ce82-294">Em certos casos, a `tenantId` / `email` / `displayName` propriedade para os membros individuais de um bate-papo pode não ser preenchida em uma solicitação `GET /chats/chat-id/members` ou `GET /chats/chat-id/members/membership-id`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-294">In certain instances, the `tenantId` / `email` / `displayName` property for the individual members of a chat might not be populated on a `GET /chats/chat-id/members` or `GET /chats/chat-id/members/membership-id` request.</span></span>

## <a name="users"></a><span data-ttu-id="2ce82-295">Usuários</span><span class="sxs-lookup"><span data-stu-id="2ce82-295">Users</span></span>

### <a name="use-the-dollar--symbol-in-the-userprincipalname"></a><span data-ttu-id="2ce82-296">Usar o símbolo de cifrão ($) no userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2ce82-296">Use the dollar ($) symbol in the userPrincipalName</span></span>

<span data-ttu-id="2ce82-297">O Microsoft Graph permite que o **userPrincipalName** comece com um caractere de cifrão (`$`).</span><span class="sxs-lookup"><span data-stu-id="2ce82-297">Microsoft Graph allows the **userPrincipalName** to begin with a dollar (`$`) character.</span></span> <span data-ttu-id="2ce82-298">No entanto, ao consultar usuários por userPrincipalName, a url de solicitação `/users/$x@y.com` falha.</span><span class="sxs-lookup"><span data-stu-id="2ce82-298">However, when querying users by userPrincipalName, the request URL `/users/$x@y.com` fails.</span></span> <span data-ttu-id="2ce82-299">Isso porque essa URL de solicitação viola as convenções de URL OData que espera que apenas as opções de consulta do sistema sejam prefixadas com um caractere `$`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-299">This is because this request URL violates the OData URL conventions which expects only system query options to be prefixed with a `$` character.</span></span> <span data-ttu-id="2ce82-300">Como alternativa, remova a barra (/) após `/users` e coloque o **userPrincipalName** entre parênteses e aspas simples como a seguir: `/users('$x@y.com')`</span><span class="sxs-lookup"><span data-stu-id="2ce82-300">As a workaround, remove the slash (/) after `/users` and enclose the **userPrincipalName** in parentheses and single quotes as follows: `/users('$x@y.com')`.</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="2ce82-301">Sem acesso instantâneo após a criação</span><span class="sxs-lookup"><span data-stu-id="2ce82-301">No instant access after creation</span></span>

<span data-ttu-id="2ce82-p130">Os usuários podem ser criados imediatamente por um POST na entidade do usuário. Uma licença do Office 365 deve ser atribuída a um usuário primeiro para que ele possa ter acesso aos serviços do Microsoft 365. Mesmo assim, devido à natureza distribuída do serviço, pode demorar 15 minutos antes que os arquivos, as mensagens e as entidades de eventos fiquem disponíveis para uso por esse usuário na API do Microsoft Graph. Durante esse período, os aplicativos receberão uma resposta de erro HTTP 404.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p130">Users can be created immediately through a POST on the user entity. A Microsoft 365 license must first be assigned to a user, in order to get access to Microsoft 365 services. Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API. During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="2ce82-306">Restrições de foto</span><span class="sxs-lookup"><span data-stu-id="2ce82-306">Photo restrictions</span></span>

<span data-ttu-id="2ce82-307">A leitura e a atualização da foto do perfil do usuário só serão possíveis se o usuário tiver uma caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="2ce82-307">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span></span> <span data-ttu-id="2ce82-308">Além disso, as fotos que *possam* ter sido previamente armazenadas usando a propriedade **thumbnailPhoto** (usando o Azure AD Graph ou por meio da sincronização do AD Connect) deixarão de estar acessíveis por meio da propriedade **foto** do recurso [usuário](/graph/api/resources/user) do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ce82-308">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Azure AD Graph or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user) resource.</span></span>
<span data-ttu-id="2ce82-309">A falha na leitura ou na atualização de uma foto, nesse caso, resultaria no seguinte erro:</span><span class="sxs-lookup"><span data-stu-id="2ce82-309">Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a><span data-ttu-id="2ce82-310">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="2ce82-310">Using delta query</span></span>

<span data-ttu-id="2ce82-311">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="2ce82-311">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a><span data-ttu-id="2ce82-312">A revogação de sessões de entrada retorna um código HTTP errado</span><span class="sxs-lookup"><span data-stu-id="2ce82-312">Revoke sign-in sessions returns wrong HTTP code</span></span>

<span data-ttu-id="2ce82-313">O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.</span><span class="sxs-lookup"><span data-stu-id="2ce82-313">The [user: revokeSignInSessions API](/graph/api/user-revokesigninsessions) should return a `204 No content` response for successful revocations, and an HTTP error code (4xx or 5xx) if anything goes wrong with the request.</span></span>  <span data-ttu-id="2ce82-314">No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre true.</span><span class="sxs-lookup"><span data-stu-id="2ce82-314">However, due to a service issue, this API returns a `200 OK` and a Boolean parameter that is always true.</span></span>  <span data-ttu-id="2ce82-315">Até que isso seja corrigido, é recomendado que desenvolvedores simplesmente tratem qualquer código de retorno 2xx como bem-sucedido para esta API.</span><span class="sxs-lookup"><span data-stu-id="2ce82-315">Until this is fixed, developers are simply advised to treat any 2xx return code as success for this API.</span></span>

### <a name="incomplete-objects-when-using-getbyids-request"></a><span data-ttu-id="2ce82-316">Objetos incompletos ao usar a solicitação getByIds</span><span class="sxs-lookup"><span data-stu-id="2ce82-316">Incomplete objects when using getByIds request</span></span>

<span data-ttu-id="2ce82-317">A solicitação de objetos usando a opção de [Obter objetos de diretório de uma lista de IDs](/graph/api/directoryobject-getbyids) deve retornar objetos completos.</span><span class="sxs-lookup"><span data-stu-id="2ce82-317">Requesting objects using [Get directory objects from a list of IDs](/graph/api/directoryobject-getbyids) should return full objects.</span></span> <span data-ttu-id="2ce82-318">No entanto, atualmente, os objetos de [usuário](/graph/api/resources/user) no ponto de extremidade v1.0 são retornados com um conjunto limitado de propriedades.</span><span class="sxs-lookup"><span data-stu-id="2ce82-318">However, currently [user](/graph/api/resources/user) objects on the v1.0 endpoint are returned with a limited set of properties.</span></span> <span data-ttu-id="2ce82-319">Como solução temporária, ao usar a operação em combinação com a opção de consulta `$select`, objetos de [usuário](/graph/api/resources/user) mais completos serão retornados.</span><span class="sxs-lookup"><span data-stu-id="2ce82-319">As a temporary workaround, when you use the operation in combination with the `$select` query option, more complete [user](/graph/api/resources/user) objects will be returned.</span></span> <span data-ttu-id="2ce82-320">Esse comportamento não está de acordo com as especificações do OData.</span><span class="sxs-lookup"><span data-stu-id="2ce82-320">This behavior is not in accordance with the OData specifications.</span></span> <span data-ttu-id="2ce82-321">Como esse comportamento pode ser atualizado no futuro, use esta solução alternativa apenas quando fornecer `$select=` com todas as propriedades de seu interesse e somente se futuras alterações nessa solução alternativa forem aceitáveis.</span><span class="sxs-lookup"><span data-stu-id="2ce82-321">Because this behavior might be updated in the future, use this workaround only when you provide `$select=` with all the properties you are interested in, and only if future breaking changes to this workaround are acceptable.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="2ce82-322">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="2ce82-322">Query parameter limitations</span></span>

* <span data-ttu-id="2ce82-323">Não há suporte para vários namespaces.</span><span class="sxs-lookup"><span data-stu-id="2ce82-323">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="2ce82-324">Não há suporte para GETs no `$ref` e também para transmissão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="2ce82-324">GETs on `$ref` and casting are not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="2ce82-p134">`@odata.bind` não é compatível. Isso significa que os desenvolvedores não poderão definir corretamente a propriedade de navegação **acceptedSenders** ou **rejectedSenders** em um grupo.</span><span class="sxs-lookup"><span data-stu-id="2ce82-p134">`@odata.bind` is not supported.  This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span></span>
* <span data-ttu-id="2ce82-327">`@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.</span><span class="sxs-lookup"><span data-stu-id="2ce82-327">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="2ce82-328">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="2ce82-328">`$expand`:</span></span>
  * <span data-ttu-id="2ce82-329">Retorna um máximo de 20 objetos.</span><span class="sxs-lookup"><span data-stu-id="2ce82-329">Returns a maximum of 20 objects.</span></span>
  * <span data-ttu-id="2ce82-330">Sem suporte para `@odata.nextLink`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-330">No support for `@odata.nextLink`.</span></span>
  * <span data-ttu-id="2ce82-331">Sem suporte para mais de 1 nível de expansão.</span><span class="sxs-lookup"><span data-stu-id="2ce82-331">No support for more than 1 level of expand.</span></span>
  * <span data-ttu-id="2ce82-332">Sem suporte com parâmetros extras (`$filter`, `$select`).</span><span class="sxs-lookup"><span data-stu-id="2ce82-332">No support with extra parameters (`$filter`, `$select`).</span></span>
* <span data-ttu-id="2ce82-333">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="2ce82-333">`$filter`:</span></span>
  * <span data-ttu-id="2ce82-334">Não há suporte para filtros no ponto de extremidade `/attachments`.</span><span class="sxs-lookup"><span data-stu-id="2ce82-334">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="2ce82-335">Se presente, o parâmetro `$filter` é ignorado.</span><span class="sxs-lookup"><span data-stu-id="2ce82-335">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="2ce82-336">Não há suporte para filtragem de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-336">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="2ce82-337">`$search`:</span><span class="sxs-lookup"><span data-stu-id="2ce82-337">`$search`:</span></span>
  * <span data-ttu-id="2ce82-338">A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.</span><span class="sxs-lookup"><span data-stu-id="2ce82-338">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="2ce82-339">Não há suporte para pesquisa de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="2ce82-339">Cross-workload searching is not supported.</span></span>
  * <span data-ttu-id="2ce82-340">A pesquisa não é suportada nos locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="2ce82-340">Searching is not supported on Azure AD B2C tenants.</span></span>
* <span data-ttu-id="2ce82-341">`$count`:</span><span class="sxs-lookup"><span data-stu-id="2ce82-341">`$count`:</span></span>
  * <span data-ttu-id="2ce82-342">Não é apoiado em locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="2ce82-342">Not supported on Azure AD B2C tenants.</span></span>
  * <span data-ttu-id="2ce82-343">Ao usar a cadeia de consulta `$count=true` ao consultar recursos de diretório, a propriedade `@odata.count` estará presente apenas na primeira página dos dados paginados.</span><span class="sxs-lookup"><span data-stu-id="2ce82-343">When using the `$count=true` query string when querying against directory resources, the `@odata.count` property will be present only in the first page of the paged data.</span></span>
* <span data-ttu-id="2ce82-344">Os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="2ce82-344">Query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="2ce82-345">Isto pode ser verdade tanto para parâmetros de consulta não suportados quanto para combinações não suportadas de parâmetros de consulta..</span><span class="sxs-lookup"><span data-stu-id="2ce82-345">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span>


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="2ce82-346">Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365</span><span class="sxs-lookup"><span data-stu-id="2ce82-346">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="2ce82-347">Alguns recursos ainda não estão disponíveis no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2ce82-347">Some functionality is not yet available in Microsoft Graph.</span></span> <span data-ttu-id="2ce82-348">Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](/previous-versions/office/office-365-api/) específicas do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="2ce82-348">If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](/previous-versions/office/office-365-api/).</span></span> <span data-ttu-id="2ce82-349">Para o Azure Active Directory, confira [Migrar aplicativos do Azure AD Graph para o Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).</span><span class="sxs-lookup"><span data-stu-id="2ce82-349">For Azure Active Directory, see [Migrate Azure AD Graph apps to Microsoft Graph](./migrate-azure-ad-graph-planning-checklist.md).</span></span>
