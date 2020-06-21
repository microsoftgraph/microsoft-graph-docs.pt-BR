---
title: Problemas conhecidos com o Microsoft Graph
description: Este artigo descreve os problemas conhecidos do Microsoft Graph.
author: MSGraphDocsVTeam
localization_priority: Priority
ms.openlocfilehash: 98c61991ec99b1f7776c03f5fa5bc2400b5950a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744052"
---
# <a name="known-issues-with-microsoft-graph"></a><span data-ttu-id="04bcf-103">Problemas conhecidos com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="04bcf-103">Known issues with Microsoft Graph</span></span>

<span data-ttu-id="04bcf-104">Este artigo descreve os problemas conhecidos do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04bcf-104">This article describes known issues with Microsoft Graph.</span></span> 

<span data-ttu-id="04bcf-105">Para relatar um problema conhecido, confira a página de [suporte do Microsoft Graph](https://developer.microsoft.com/graph/support) .</span><span class="sxs-lookup"><span data-stu-id="04bcf-105">To report a known issue, see the [Microsoft Graph support](https://developer.microsoft.com/graph/support) page.</span></span>

<span data-ttu-id="04bcf-106">Para obter informações sobre as atualizações mais recentes para a API do Microsoft Graph, consulte o [changelog do Microsoft Graph](changelog.md).</span><span class="sxs-lookup"><span data-stu-id="04bcf-106">For information about the latest updates to the Microsoft Graph API, see the [Microsoft Graph changelog](changelog.md).</span></span>

## <a name="bookings"></a><span data-ttu-id="04bcf-107">Reservas</span><span class="sxs-lookup"><span data-stu-id="04bcf-107">Bookings</span></span>

### <a name="errorexceededfindcountlimit-when-querying-bookingbusinesses"></a><span data-ttu-id="04bcf-108">ErrorExceededFindCountLimit ao consultar bookingBusinesses</span><span class="sxs-lookup"><span data-stu-id="04bcf-108">ErrorExceededFindCountLimit when querying bookingBusinesses</span></span>

<span data-ttu-id="04bcf-109">A obtenção da lista de `bookingBusinesses` falha com o seguinte código de erro quando a organização tem várias empresas de Reservas e a conta que está fazendo a solicitação não é um administrador:</span><span class="sxs-lookup"><span data-stu-id="04bcf-109">Getting the list of `bookingBusinesses` fails with the following error code when an organization has several Bookings businesses and the account making the request is not an administrator:</span></span>

```json
{
  "error": {
    "code": "ErrorExceededFindCountLimit",
    "message":
      "The GetBookingMailboxes request returned too many results. Please specify a query to limit the results.",
  }
}
```

<span data-ttu-id="04bcf-110">Como alternativa, você pode limitar o conjunto de empresas retornadas pela solicitação, incluindo um parâmetro `query`, por exemplo:</span><span class="sxs-lookup"><span data-stu-id="04bcf-110">As a workaround, you can limit the set of businesses returned by the request by including a `query` parameter, for example:</span></span>

```
GET https://graph.microsoft.com/beta/bookingBusinesses?query=Fabrikam
```
## <a name="calendars"></a><span data-ttu-id="04bcf-111">Calendários</span><span class="sxs-lookup"><span data-stu-id="04bcf-111">Calendars</span></span>

### <a name="accessing-a-shared-calendar"></a><span data-ttu-id="04bcf-112">Acessar um calendário compartilhado</span><span class="sxs-lookup"><span data-stu-id="04bcf-112">Accessing a shared calendar</span></span>

<span data-ttu-id="04bcf-113">Ao tentar acessar eventos em um calendário compartilhado por outro usuário usando a operação a seguir:</span><span class="sxs-lookup"><span data-stu-id="04bcf-113">When attempting to access events in a calendar that has been shared by another user using the following operation:</span></span>

```http
GET /users/{id}/calendars/{id}/events
```

<span data-ttu-id="04bcf-114">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`.</span><span class="sxs-lookup"><span data-stu-id="04bcf-114">You may get HTTP 500 with the error code `ErrorInternalServerTransientError`.</span></span> <span data-ttu-id="04bcf-115">The error occurs because:</span><span class="sxs-lookup"><span data-stu-id="04bcf-115">The error occurs because:</span></span>

- <span data-ttu-id="04bcf-116">Historicamente, há duas maneiras de compartilhar o calendário, que são chamadas de "antiga" e "nova" abordagens, para fins de diferenciá-las.</span><span class="sxs-lookup"><span data-stu-id="04bcf-116">Historically, there are two ways that calendar sharing has been implemented, which, for the purpose of differentiating them, are referred to as the "old" approach and "new" approach.</span></span>
- <span data-ttu-id="04bcf-117">A nova abordagem está disponível atualmente para compartilhamento de calendários, com permissões de exibição ou edição, mas não com permissões de representante.</span><span class="sxs-lookup"><span data-stu-id="04bcf-117">The new approach is currently available for sharing calendars with view or edit permissions, but not with delegate permissions.</span></span>
- <span data-ttu-id="04bcf-118">Você pode usar a API REST de calendário para exibir ou editar calendários compartilhados somente quando os calendários são compartilhados de acordo com a **nova** abordagem.</span><span class="sxs-lookup"><span data-stu-id="04bcf-118">You can use the calendar REST API to view or edit shared calendars only if the calendars were shared using the **new** approach.</span></span>
- <span data-ttu-id="04bcf-119">Não é possível usar a API REST de calendário para exibir ou editar esses calendários ou os respectivos eventos quando eles são compartilhados de acordo com a **antiga** abordagem.</span><span class="sxs-lookup"><span data-stu-id="04bcf-119">You cannot use the calendar REST API to view or edit such calendars (or their events) if the calendars were shared using the **old** approach.</span></span>


<span data-ttu-id="04bcf-120">Se você compartilhar o calendário com permissões de exibição ou edição usando a abordagem antiga, poderá resolver o problema e atualizar manualmente o compartilhamento do calendário para usar a nova abordagem.</span><span class="sxs-lookup"><span data-stu-id="04bcf-120">If a calendar was shared with view or edit permissions but using the old approach, you can now work around the error and manually upgrade the calendar sharing to use the new approach.</span></span>
<span data-ttu-id="04bcf-121">Com o tempo, o Outlook atualizará automaticamente todos os calendários compartilhados para usar a nova abordagem, incluindo calendários compartilhados com permissões delegadas.</span><span class="sxs-lookup"><span data-stu-id="04bcf-121">Over time, Outlook will automatically upgrade all shared calendars to use the new approach, including calendars shared with delegate permissions.</span></span>

<span data-ttu-id="04bcf-122">Para atualizar manualmente um calendário compartilhado e usar a nova abordagem, faça os seguintes procedimentos:</span><span class="sxs-lookup"><span data-stu-id="04bcf-122">To manually upgrade a shared calendar to use the new approach, follow these steps:</span></span>
1.  <span data-ttu-id="04bcf-123">O destinatário remove o calendário previamente compartilhado com ele.</span><span class="sxs-lookup"><span data-stu-id="04bcf-123">The recipient removes the calendar that was previously shared to them.</span></span>
2.  <span data-ttu-id="04bcf-124">O proprietário compartilha novamente o calendário no Outlook na Web, no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="04bcf-124">The calendar owner re-shares the calendar in Outlook on the web, Outlook on iOS, or Outlook on Android.</span></span>
3.  <span data-ttu-id="04bcf-125">The recipient re-accepts the shared calendar using Outlook on the web.</span><span class="sxs-lookup"><span data-stu-id="04bcf-125">The recipient re-accepts the shared calendar using Outlook on the web.</span></span> <span data-ttu-id="04bcf-126">(It will be possible to use other Outlook clients soon.)</span><span class="sxs-lookup"><span data-stu-id="04bcf-126">(It will be possible to use other Outlook clients soon.)</span></span>
4.  <span data-ttu-id="04bcf-127">O destinatário verifica se o calendário foi compartilhado novamente com êxito por meio da nova abordagem, com permissão para exibi-lo no Outlook para iOS ou no Outlook para Android.</span><span class="sxs-lookup"><span data-stu-id="04bcf-127">The recipient verifies that the calendar has been re-shared successfully using the new approach by being able to view the shared calendar in Outlook on iOS or Outlook on Android.</span></span>

<span data-ttu-id="04bcf-128">A calendar shared with you in the new approach appears as just another calendar in your mailbox.</span><span class="sxs-lookup"><span data-stu-id="04bcf-128">A calendar shared with you in the new approach appears as just another calendar in your mailbox.</span></span> <span data-ttu-id="04bcf-129">You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar.</span><span class="sxs-lookup"><span data-stu-id="04bcf-129">You can use the calendar REST API to view or edit events in the shared calendar, as if it's your own calendar.</span></span> <span data-ttu-id="04bcf-130">As an example:</span><span class="sxs-lookup"><span data-stu-id="04bcf-130">As an example:</span></span>

```http
GET /me/calendars/{id}/events
```

### <a name="adding-and-accessing-ics-based-calendars-in-users-mailbox"></a><span data-ttu-id="04bcf-131">Adicionar e acessar calendários baseados em ICS na caixa de correio do usuário</span><span class="sxs-lookup"><span data-stu-id="04bcf-131">Adding and accessing ICS-based calendars in user's mailbox</span></span>

<span data-ttu-id="04bcf-132">Atualmente, há suporte parcial para um calendário com base em uma Inscrição em Calendário da Internet (ICS):</span><span class="sxs-lookup"><span data-stu-id="04bcf-132">Currently, there is partial support for a calendar based on an Internet Calendar Subscription (ICS):</span></span>

* <span data-ttu-id="04bcf-133">Você pode adicionar um calendário baseado em ICS para uma caixa de correio do usuário por meio da interface do usuário, mas não através da API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04bcf-133">You can add an ICS-based calendar to a user mailbox through the user interface, but not through the Microsoft Graph API.</span></span>
* <span data-ttu-id="04bcf-134">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars.</span><span class="sxs-lookup"><span data-stu-id="04bcf-134">[Listing the user's calendars](/graph/api/user-list-calendars?view=graph-rest-1.0) lets you get the **name**, **color** and **id** properties of each [calendar](/graph/api/resources/calendar?view=graph-rest-1.0) in the user's default calendar group, or a specified calendar group, including any ICS-based calendars.</span></span> <span data-ttu-id="04bcf-135">You cannot store or access the ICS URL in the calendar resource.</span><span class="sxs-lookup"><span data-stu-id="04bcf-135">You cannot store or access the ICS URL in the calendar resource.</span></span>
* <span data-ttu-id="04bcf-136">Você também pode [listar os eventos](/graph/api/calendar-list-events?view=graph-rest-1.0) de um calendário baseado em ICS.</span><span class="sxs-lookup"><span data-stu-id="04bcf-136">You can also [list the events](/graph/api/calendar-list-events?view=graph-rest-1.0) of an ICS-based calendar.</span></span>

### <a name="attaching-large-files-to-events"></a><span data-ttu-id="04bcf-137">Anexar arquivos grandes a eventos</span><span class="sxs-lookup"><span data-stu-id="04bcf-137">Attaching large files to events</span></span>
<span data-ttu-id="04bcf-138">Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="04bcf-138">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="04bcf-139">Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="04bcf-139">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="onlinemeetingurl-property-support-for-microsoft-teams"></a><span data-ttu-id="04bcf-140">Suporte de propriedade onlineMeetingUrl do Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="04bcf-140">onlineMeetingUrl property support for Microsoft Teams</span></span>

<span data-ttu-id="04bcf-141">Atualmente, a propriedade **onlineMeetingUrl** de um [evento](/graph/api/resources/event?view=graph-rest-1.0) de reunião do Skype indica a URL da reunião online.</span><span class="sxs-lookup"><span data-stu-id="04bcf-141">Currently, the **onlineMeetingUrl** property of a Skype meeting [event](/graph/api/resources/event?view=graph-rest-1.0) would indicate the online meeting URL.</span></span> <span data-ttu-id="04bcf-142">No entanto, essa propriedade para um evento de reunião do Microsoft Teams está definida como nula.</span><span class="sxs-lookup"><span data-stu-id="04bcf-142">However, that property for a Microsoft Teams meeting event is set to null.</span></span>

<span data-ttu-id="04bcf-143">A versão beta oferece uma solução alternativa, na qual é possível usar a propriedade **onlineMeetingProvider** de um [evento](/graph/api/resources/event?view=graph-rest-beta)para verificar se o provedor é o Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="04bcf-143">The beta version offers a workaround, where you can use the **onlineMeetingProvider** property of an [event](/graph/api/resources/event?view=graph-rest-beta) to verify if the provider is Microsoft Teams.</span></span> <span data-ttu-id="04bcf-144">Por meio da propriedade **onlineMeeting** do **evento**, você pode acessar o **joinUrl**.</span><span class="sxs-lookup"><span data-stu-id="04bcf-144">Through the **onlineMeeting** property of the **event**, you can access the **joinUrl**.</span></span>

## <a name="change-notifications"></a><span data-ttu-id="04bcf-145">Notificações de alteração</span><span class="sxs-lookup"><span data-stu-id="04bcf-145">Change notifications</span></span>

### <a name="additional-notifications-for-users"></a><span data-ttu-id="04bcf-146">Notificações adicionais para usuários</span><span class="sxs-lookup"><span data-stu-id="04bcf-146">Additional notifications for users</span></span>

<span data-ttu-id="04bcf-147">As [assinaturas](/graph/api/resources/subscription) de alterações para o **usuário** com o **changeType** definido como **atualizado** também receberão notificações de **changeType**: **atualizado** na criação do usuário e exclusão reversível do usuário.</span><span class="sxs-lookup"><span data-stu-id="04bcf-147">[Subscriptions](/graph/api/resources/subscription) to changes for **user** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on user creation and user soft deletion.</span></span>

### <a name="additional-notifications-for-groups"></a><span data-ttu-id="04bcf-148">Notificações adicionais para grupos</span><span class="sxs-lookup"><span data-stu-id="04bcf-148">Additional notifications for groups</span></span>

<span data-ttu-id="04bcf-149">As [assinaturas](/graph/api/resources/subscription) de alterações no **grupo** com o **changeType** definido como **atualizado** também receberão notificações **changeType**: **atualizado** na criação do grupo e exclusão reversível do grupo.</span><span class="sxs-lookup"><span data-stu-id="04bcf-149">[Subscriptions](/graph/api/resources/subscription) to changes for **group** with **changeType** set to **updated** will also receive notifications of **changeType**: **updated** on group creation and group soft deletion.</span></span>

## <a name="cloud-communications"></a><span data-ttu-id="04bcf-150">Comunicações na nuvem</span><span class="sxs-lookup"><span data-stu-id="04bcf-150">Cloud communications</span></span> 

<span data-ttu-id="04bcf-151">O cliente do Microsoft Teams não mostra o menu **Exibir detalhes da Reunião** para reuniões de canal criadas por meio da API de comunicações na nuvem.</span><span class="sxs-lookup"><span data-stu-id="04bcf-151">The Microsoft Teams client does not show the **View Meeting details**  menu for channel meetings created via the cloud communications API.</span></span>

## <a name="cloud-solution-provider-apps"></a><span data-ttu-id="04bcf-152">Aplicativos de Provedor de Soluções na Nuvem</span><span class="sxs-lookup"><span data-stu-id="04bcf-152">Cloud Solution Provider apps</span></span>

### <a name="csp-apps-must-use-azure-ad-endpoint"></a><span data-ttu-id="04bcf-153">Os aplicativos CSP devem usar o ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="04bcf-153">CSP apps must use Azure AD endpoint</span></span>

<span data-ttu-id="04bcf-154">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers.</span><span class="sxs-lookup"><span data-stu-id="04bcf-154">Cloud solution provider (CSP) apps must acquire tokens from the Azure AD (v1) endpoints to successfully call Microsoft Graph in their partner-managed customers.</span></span> <span data-ttu-id="04bcf-155">Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span><span class="sxs-lookup"><span data-stu-id="04bcf-155">Currently, acquiring a token through the newer Azure AD v2.0 endpoint is not supported.</span></span>

### <a name="pre-consent-for-csp-apps-doesnt-work-in-some-customer-tenants"></a><span data-ttu-id="04bcf-156">A pré-autorização para aplicativos CSP não funciona em alguns locatários do cliente</span><span class="sxs-lookup"><span data-stu-id="04bcf-156">Pre-consent for CSP apps doesn't work in some customer tenants</span></span>

<span data-ttu-id="04bcf-157">Sob certas circunstâncias, o pré-consentimento para aplicativos CSP pode não funcionar para alguns de seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="04bcf-157">Under certain circumstances, pre-consent for CSP apps may not work for some of your customer tenants.</span></span>

- <span data-ttu-id="04bcf-158">Para aplicativos que usam permissões delegadas, ao usar o aplicativo pela primeira vez com um novo locatário do cliente, você poderá receber esse erro após o logon: `AADSTS50000: There was an error issuing a token`.</span><span class="sxs-lookup"><span data-stu-id="04bcf-158">For apps using delegated permissions, when using the app for the first time with a new customer tenant you might receive this error after sign-in: `AADSTS50000: There was an error issuing a token`.</span></span>
- <span data-ttu-id="04bcf-159">Para aplicativos que usam permissões de aplicativos, seu aplicativo pode adquirir um token, mas inesperadamente receber uma mensagem de acesso negado ao chamar o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04bcf-159">For apps using application permissions, your app can acquire a token, but unexpectedly gets an access denied message when calling Microsoft Graph.</span></span>

<span data-ttu-id="04bcf-160">Estamos trabalhando para corrigir esse problema o mais rápido possível, de modo que a pré-autorização funcionará para todos os seus locatários de clientes.</span><span class="sxs-lookup"><span data-stu-id="04bcf-160">We are working to fix this issue as soon as possible, so that pre-consent will work for all your customer tenants.</span></span>

<span data-ttu-id="04bcf-161">Enquanto isso, para desbloquear o desenvolvimento e testes, você pode usar a seguinte solução alternativa.</span><span class="sxs-lookup"><span data-stu-id="04bcf-161">In the meantime, to unblock development and testing you can use the following workaround.</span></span>

><span data-ttu-id="04bcf-162">**NOTE:** This is not a permanent solution and is only intended to unblock development.</span><span class="sxs-lookup"><span data-stu-id="04bcf-162">**NOTE:** This is not a permanent solution and is only intended to unblock development.</span></span>  <span data-ttu-id="04bcf-163">This workaround will not be required once the aforementioned issue is fixed.</span><span class="sxs-lookup"><span data-stu-id="04bcf-163">This workaround will not be required once the aforementioned issue is fixed.</span></span>  <span data-ttu-id="04bcf-164">This workaround does not need to be undone once the fix is in place.</span><span class="sxs-lookup"><span data-stu-id="04bcf-164">This workaround does not need to be undone once the fix is in place.</span></span>

1. <span data-ttu-id="04bcf-165">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window.</span><span class="sxs-lookup"><span data-stu-id="04bcf-165">Open an Azure AD v2 PowerShell session and connect to your `customer` tenant by entering your admin credentials into the sign-in window.</span></span> <span data-ttu-id="04bcf-166">You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span><span class="sxs-lookup"><span data-stu-id="04bcf-166">You can download and install Azure AD PowerShell V2 from [here](https://www.powershellgallery.com/packages/AzureAD).</span></span>

    ```PowerShell
    Connect-AzureAd -TenantId {customerTenantIdOrDomainName}
    ```

2. <span data-ttu-id="04bcf-167">Crie o servicePrincipal do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04bcf-167">Create the Microsoft Graph service principal.</span></span>

    ```PowerShell
    New-AzureADServicePrincipal -AppId 00000003-0000-0000-c000-000000000000
    ```
## <a name="contacts"></a><span data-ttu-id="04bcf-168">Contatos</span><span class="sxs-lookup"><span data-stu-id="04bcf-168">Contacts</span></span>

### <a name="organization-contacts-available-in-only-beta"></a><span data-ttu-id="04bcf-169">Contatos de organização disponíveis somente na versão beta</span><span class="sxs-lookup"><span data-stu-id="04bcf-169">Organization contacts available in only beta</span></span>

<span data-ttu-id="04bcf-170">Only personal contacts are currently supported.</span><span class="sxs-lookup"><span data-stu-id="04bcf-170">Only personal contacts are currently supported.</span></span> <span data-ttu-id="04bcf-171">Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span><span class="sxs-lookup"><span data-stu-id="04bcf-171">Organizational contacts are not currently supported in `/v1.0`, but can be found in `/beta`.</span></span>

### <a name="default-contacts-folder"></a><span data-ttu-id="04bcf-172">Pasta Contatos padrão</span><span class="sxs-lookup"><span data-stu-id="04bcf-172">Default contacts folder</span></span>

<span data-ttu-id="04bcf-173">Na versão `/v1.0`, `GET /me/contactFolders` não inclui a pasta de contatos do usuário padrão.</span><span class="sxs-lookup"><span data-stu-id="04bcf-173">In the `/v1.0` version, `GET /me/contactFolders` does not include the user's default contacts folder.</span></span>

<span data-ttu-id="04bcf-174">A fix will be made available.</span><span class="sxs-lookup"><span data-stu-id="04bcf-174">A fix will be made available.</span></span> <span data-ttu-id="04bcf-175">Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span><span class="sxs-lookup"><span data-stu-id="04bcf-175">Meanwhile, you can use the following [list contacts](/graph/api/user-list-contacts?view=graph-rest-1.0) query and the **parentFolderId** property as a workaround to get the folder ID of the default contacts folder:</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/contacts?$top=1&$select=parentFolderId
```

<span data-ttu-id="04bcf-176">Na consulta acima:</span><span class="sxs-lookup"><span data-stu-id="04bcf-176">In the above query:</span></span>

1. <span data-ttu-id="04bcf-177">`/me/contacts?$top=1` obtém as propriedades de um [contato](/graph/api/resources/contact?view=graph-rest-1.0) na pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="04bcf-177">`/me/contacts?$top=1` gets the properties of a [contact](/graph/api/resources/contact?view=graph-rest-1.0) in the default contacts folder.</span></span>
2. <span data-ttu-id="04bcf-178">A anexação de `&$select=parentFolderId` retorna apenas a propriedade **parentFolderId** do contato, que é a ID da pasta de contatos padrão.</span><span class="sxs-lookup"><span data-stu-id="04bcf-178">Appending `&$select=parentFolderId` returns only the contact's **parentFolderId** property, which is the ID of the default contacts folder.</span></span>


### <a name="accessing-contacts-via-a-contact-folder-in-beta"></a><span data-ttu-id="04bcf-179">Acessar contatos por meio de uma pasta de contatos na versão beta</span><span class="sxs-lookup"><span data-stu-id="04bcf-179">Accessing contacts via a contact folder in beta</span></span>

<span data-ttu-id="04bcf-180">Atualmente, não há na versão `/beta` um problema que impeça o acesso a um [contato](/graph/api/resources/contact?view=graph-rest-beta) especificando sua pasta pai na URL de solicitação REST, conforme mostrado nos dois cenários abaixo.</span><span class="sxs-lookup"><span data-stu-id="04bcf-180">In the `/beta` version, there is currently an issue that prevents accessing a [contact](/graph/api/resources/contact?view=graph-rest-beta) by specifying its parent folder in the REST request URL, as shown in the 2 scenarios below.</span></span>

* <span data-ttu-id="04bcf-181">Acessando um contato a partir de um nível superior do [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) do usuário.</span><span class="sxs-lookup"><span data-stu-id="04bcf-181">Accessing a contact from a top level [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-beta) of the user's.</span></span>

```http
GET /me/contactfolders/{id}/contacts/{id}
GET /users/{id | userPrincipalName}/contactfolders/{id}/contacts/{id}
```

* <span data-ttu-id="04bcf-182">Accessing a contact contained in a child folder of a **contactFolder**.</span><span class="sxs-lookup"><span data-stu-id="04bcf-182">Accessing a contact contained in a child folder of a **contactFolder**.</span></span>  <span data-ttu-id="04bcf-183">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span><span class="sxs-lookup"><span data-stu-id="04bcf-183">The example below shows one level of nesting, but a contact can be located in a child of a child and so on.</span></span>

```http
GET /me/contactFolder/{id}/childFolders/{id}/.../contacts/{id}
GET /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts/{id}
```

<span data-ttu-id="04bcf-184">Como alternativa, você pode simplesmente [obter](/graph/api/contact-get?view=graph-rest-beta) o contato, especificando sua identificação conforme mostrado abaixo, uma vez que o GET /contacts na versão `/beta` se aplica a todos os contatos na caixa de correio do usuário:</span><span class="sxs-lookup"><span data-stu-id="04bcf-184">As an alternative, you can simply [get](/graph/api/contact-get?view=graph-rest-beta) the contact by specifying its ID as shown below, since GET /contacts in the `/beta` version applies to all the contacts in the user's mailbox:</span></span>

```http
GET /me/contacts/{id}
GET /users/{id | userPrincipalName}/contacts/{id}
```
## <a name="delta-query"></a><span data-ttu-id="04bcf-185">Consulta delta</span><span class="sxs-lookup"><span data-stu-id="04bcf-185">Delta query</span></span>

* <span data-ttu-id="04bcf-186">O contexto de OData às vezes é retornado incorretamente ao controlar alterações nas relações.</span><span class="sxs-lookup"><span data-stu-id="04bcf-186">OData context is sometimes returned incorrectly when tracking changes to relationships.</span></span>
* <span data-ttu-id="04bcf-187">As extensões de esquema (herdadas) não são retornadas com instrução $select, mas são retornadas sem $select.</span><span class="sxs-lookup"><span data-stu-id="04bcf-187">Schema extensions (legacy) are not returned with $select statement, but are returned without $select.</span></span>
* <span data-ttu-id="04bcf-188">Os clientes não podem controlar alterações em extensões abertas ou extensões de esquema.</span><span class="sxs-lookup"><span data-stu-id="04bcf-188">Clients cannot track changes to open extensions or registered schema extensions.</span></span>

## <a name="extensions"></a><span data-ttu-id="04bcf-189">Extensões</span><span class="sxs-lookup"><span data-stu-id="04bcf-189">Extensions</span></span>

### <a name="change-tracking-is-not-supported"></a><span data-ttu-id="04bcf-190">Não há suporte para o controle de alterações</span><span class="sxs-lookup"><span data-stu-id="04bcf-190">Change tracking is not supported</span></span>

<span data-ttu-id="04bcf-191">O controle de alterações (consulta delta) não tem suporte nas propriedades de extensão do esquema ou abrir.</span><span class="sxs-lookup"><span data-stu-id="04bcf-191">Change tracking (delta query) is not supported for open or schema extension properties.</span></span>

### <a name="creating-a-resource-and-open-extension-at-the-same-time"></a><span data-ttu-id="04bcf-192">Criar um recurso e uma extensão aberta ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="04bcf-192">Creating a resource and open extension at the same time</span></span>

<span data-ttu-id="04bcf-193">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**.</span><span class="sxs-lookup"><span data-stu-id="04bcf-193">You cannot specify an open extension at the same time you create an instance of **administrativeUnit**, **device**, **group**, **organization** or **user**.</span></span> <span data-ttu-id="04bcf-194">You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span><span class="sxs-lookup"><span data-stu-id="04bcf-194">You must first create the instance and then specify the open extension data in a subsequent ``POST`` request on that instance.</span></span>

### <a name="creating-a-resource-instance-and-adding-schema-extension-data-at-the-same-time"></a><span data-ttu-id="04bcf-195">Criar uma instância de recurso e adicionar dados de extensão de esquema ao mesmo tempo</span><span class="sxs-lookup"><span data-stu-id="04bcf-195">Creating a resource instance and adding schema extension data at the same time</span></span>

<span data-ttu-id="04bcf-196">Não é possível especificar uma extensão de esquema na mesma operação, como criar uma instância de **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="04bcf-196">You cannot specify a schema extension in the same operation as creating an instance of **contact**, **event**, **message**, or **post**.</span></span>
<span data-ttu-id="04bcf-197">Você deve primeiro criar a instância de recurso e, em seguida, fazer um `PATCH` para essa instância para adicionar uma extensão de esquema e dados personalizados.</span><span class="sxs-lookup"><span data-stu-id="04bcf-197">You must first create the resource instance and then do a `PATCH` to that instance to add a schema extension and custom data.</span></span>

### <a name="limit-of-100-schema-extension-property-values-allowed-per-resource-instance"></a><span data-ttu-id="04bcf-198">Limite de 100 valores de propriedade de extensão de esquema permitido por instância de recursos</span><span class="sxs-lookup"><span data-stu-id="04bcf-198">Limit of 100 schema extension property values allowed per resource instance</span></span>

<span data-ttu-id="04bcf-199">Recursos de diretório, como **dispositivo**, **grupo** e **usuário**, atualmente limitam o número total de valores de propriedade de extensão de esquema que podem ser definidas em um recurso, até 100.</span><span class="sxs-lookup"><span data-stu-id="04bcf-199">Directory resources, such as **device**, **group** and **user**, currently limit the total number of schema extension property values that can be set on a resource instance, to 100.</span></span>

### <a name="filtering-on-schema-extension-properties-not-supported-on-all-entity-types"></a><span data-ttu-id="04bcf-200">Não há suporte a filtragem em propriedades de extensão de esquema em todos os tipos de entidade</span><span class="sxs-lookup"><span data-stu-id="04bcf-200">Filtering on schema extension properties not supported on all entity types</span></span>

<span data-ttu-id="04bcf-201">Não há suporte a filtragem em propriedades de extensão de esquema (usando a expressão `$filter`) para tipos de entidade do Outlook – **contato**, **evento**, **mensagem** ou **postagem**.</span><span class="sxs-lookup"><span data-stu-id="04bcf-201">Filtering on schema extension properties (using the `$filter` expression) is not supported for Outlook entity types - **contact**, **event**, **message**, or **post**.</span></span>

## <a name="files-onedrive"></a><span data-ttu-id="04bcf-202">Arquivos (OneDrive)</span><span class="sxs-lookup"><span data-stu-id="04bcf-202">Files (OneDrive)</span></span>

* <span data-ttu-id="04bcf-203">O primeiro acesso a uma unidade pessoal de um usuário pelo Microsoft Graph antes que ele acesse o próprio site pessoal por um navegador resulta em uma resposta 401.</span><span class="sxs-lookup"><span data-stu-id="04bcf-203">First time access to a user's personal drive through Microsoft Graph before the user accesses their personal site through a browser leads to a 401 response.</span></span>

## <a name="groups"></a><span data-ttu-id="04bcf-204">Grupos</span><span class="sxs-lookup"><span data-stu-id="04bcf-204">Groups</span></span>

### <a name="permissions-for-groups-and-microsoft-teams"></a><span data-ttu-id="04bcf-205">Permissões para grupos e Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="04bcf-205">Permissions for groups and Microsoft Teams</span></span>

<span data-ttu-id="04bcf-206">O Microsoft Graph expõe duas permissões ([*Group.Read.All*](permissions-reference.md#group-permissions) e [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) para obter acesso a APIs de grupos e Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="04bcf-206">Microsoft Graph exposes two permissions ([*Group.Read.All*](permissions-reference.md#group-permissions) and [*Group.ReadWrite.All*](permissions-reference.md#group-permissions)) for access to the APIs for groups and Microsoft Teams.</span></span>
<span data-ttu-id="04bcf-207">As permissões do aplicativo devem ser consentidas por um administrador.</span><span class="sxs-lookup"><span data-stu-id="04bcf-207">These permissions must be consented to by an administrator.</span></span>
<span data-ttu-id="04bcf-208">No futuro, pretendemos adicionar novas permissões para grupos e equipes que possam ser consentidas pelos usuários.</span><span class="sxs-lookup"><span data-stu-id="04bcf-208">In the future, we plan to add new permissions for groups and teams that users can consent to.</span></span>

<span data-ttu-id="04bcf-209">Also, only the API for core group administration and management supports access using delegated or app-only permissions.</span><span class="sxs-lookup"><span data-stu-id="04bcf-209">Also, only the API for core group administration and management supports access using delegated or app-only permissions.</span></span> <span data-ttu-id="04bcf-210">All other features of the group API support only delegated permissions.</span><span class="sxs-lookup"><span data-stu-id="04bcf-210">All other features of the group API support only delegated permissions.</span></span>

<span data-ttu-id="04bcf-211">Exemplos de recursos de grupo que oferecem suporte a permissões delegadas e somente para aplicativos:</span><span class="sxs-lookup"><span data-stu-id="04bcf-211">Examples of group features that support delegated and app-only permissions:</span></span>

* <span data-ttu-id="04bcf-212">Criar e excluir grupos</span><span class="sxs-lookup"><span data-stu-id="04bcf-212">Creating and deleting groups</span></span>
* <span data-ttu-id="04bcf-213">Obter e atualizar propriedades do grupo pertencentes ao gerenciamento ou administração de grupo</span><span class="sxs-lookup"><span data-stu-id="04bcf-213">Getting and updating group properties pertaining to group administration or management</span></span>
* <span data-ttu-id="04bcf-214">[Definições do diretório](/graph/api/resources/directoryobject?view=graph-rest-1.0), tipo e sincronização do grupo</span><span class="sxs-lookup"><span data-stu-id="04bcf-214">Group [directory settings](/graph/api/resources/directoryobject?view=graph-rest-1.0), type, and synchronization</span></span>
* <span data-ttu-id="04bcf-215">Membros e proprietários de grupo</span><span class="sxs-lookup"><span data-stu-id="04bcf-215">Group owners and membership</span></span>
* <span data-ttu-id="04bcf-216">Obtendo conversas de grupo e threads</span><span class="sxs-lookup"><span data-stu-id="04bcf-216">Getting group conversations and threads</span></span>

<span data-ttu-id="04bcf-217">Exemplos de recursos de grupo que oferecem suporte somente a permissões delegadas:</span><span class="sxs-lookup"><span data-stu-id="04bcf-217">Examples of group features that support only delegated permissions:</span></span>

* <span data-ttu-id="04bcf-218">Agrupar eventos, foto</span><span class="sxs-lookup"><span data-stu-id="04bcf-218">Group events, photo</span></span>
* <span data-ttu-id="04bcf-219">Remetentes externos, remetentes aceitos ou rejeitados e assinatura de grupo</span><span class="sxs-lookup"><span data-stu-id="04bcf-219">External senders, accepted or rejected senders, group subscription</span></span>
* <span data-ttu-id="04bcf-220">Favoritos do usuário e contagem de não vistos</span><span class="sxs-lookup"><span data-stu-id="04bcf-220">User favorites and unseen count</span></span>

### <a name="policy"></a><span data-ttu-id="04bcf-221">Política</span><span class="sxs-lookup"><span data-stu-id="04bcf-221">Policy</span></span>

<span data-ttu-id="04bcf-222">O uso do Microsoft Graph para criar e nomear um grupo do Office 365 ultrapassa qualquer política de grupo do Office 365 que seja configurada pelo Outlook Web App.</span><span class="sxs-lookup"><span data-stu-id="04bcf-222">Using Microsoft Graph to create and name an Office 365 group bypasses any Office 365 group policies that are configured through Outlook Web App.</span></span>

### <a name="setting-the-allowexternalsenders-property"></a><span data-ttu-id="04bcf-223">Definir a propriedade allowExternalSenders</span><span class="sxs-lookup"><span data-stu-id="04bcf-223">Setting the allowExternalSenders property</span></span>

<span data-ttu-id="04bcf-224">Atualmente, há um problema que impede a configuração da propriedade **allowExternalSenders** de um grupo em uma operação de POST ou PATCH no `/v1.0` e no `/beta`.</span><span class="sxs-lookup"><span data-stu-id="04bcf-224">There is currently an issue that prevents setting the **allowExternalSenders** property of a group in a POST or PATCH operation, in both `/v1.0` and `/beta`.</span></span>

### <a name="using-delta-query"></a><span data-ttu-id="04bcf-225">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="04bcf-225">Using delta query</span></span>

<span data-ttu-id="04bcf-226">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="04bcf-226">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

## <a name="identity-and-access--application-and-service-principal-apis"></a><span data-ttu-id="04bcf-227">Identidade e acesso | APIs da entidade de serviço e aplicativo</span><span class="sxs-lookup"><span data-stu-id="04bcf-227">Identity and access | Application and service principal APIs</span></span>

<span data-ttu-id="04bcf-228">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development.</span><span class="sxs-lookup"><span data-stu-id="04bcf-228">There are changes to the [application](/graph/api/resources/application?view=graph-rest-beta) and [servicePrincipal](/graph/api/resources/serviceprincipal?view=graph-rest-beta) entities currently in development.</span></span> <span data-ttu-id="04bcf-229">The following is a summary of current limitations and in-development API features.</span><span class="sxs-lookup"><span data-stu-id="04bcf-229">The following is a summary of current limitations and in-development API features.</span></span>

<span data-ttu-id="04bcf-230">Limitações atuais:</span><span class="sxs-lookup"><span data-stu-id="04bcf-230">Current limitations:</span></span>

* <span data-ttu-id="04bcf-231">Algumas propriedades do aplicativo (como appRoles e addIns) não estarão disponíveis até que todas as alterações sejam concluídas.</span><span class="sxs-lookup"><span data-stu-id="04bcf-231">Some application properties (such as appRoles and addIns) will not be available until all changes are completed.</span></span>
* <span data-ttu-id="04bcf-232">Somente aplicativos multilocatários podem ser registrados.</span><span class="sxs-lookup"><span data-stu-id="04bcf-232">Only multi-tenant apps can be registered.</span></span>
* <span data-ttu-id="04bcf-233">Atualizar aplicativos é restrito aos aplicativos registrados após a atualização inicial beta.</span><span class="sxs-lookup"><span data-stu-id="04bcf-233">Updating apps is restricted to apps registered after the initial beta update.</span></span>
* <span data-ttu-id="04bcf-234">Usuários do Azure Active Directory podem registrar aplicativos e adicionar proprietários adicionais.</span><span class="sxs-lookup"><span data-stu-id="04bcf-234">Azure Active Directory users can register apps and add additional owners.</span></span>
* <span data-ttu-id="04bcf-235">Suporte para protocolos OpenID Connect e OAuth.</span><span class="sxs-lookup"><span data-stu-id="04bcf-235">Support for OpenID Connect and OAuth protocols.</span></span>
* <span data-ttu-id="04bcf-236">Atribuições de política para uma falha de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="04bcf-236">Policy assignments to an application fail.</span></span>
* <span data-ttu-id="04bcf-237">Falha em operações em ownedObjects que exigem appId (por exemplo, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span><span class="sxs-lookup"><span data-stu-id="04bcf-237">Operations on ownedObjects that require appId fail (For example, users/{id|userPrincipalName}/ownedObjects/{id}/...).</span></span>

<span data-ttu-id="04bcf-238">Em desenvolvimento:</span><span class="sxs-lookup"><span data-stu-id="04bcf-238">In development:</span></span>

* <span data-ttu-id="04bcf-239">Capacidade de registrar aplicativos de um único locatário.</span><span class="sxs-lookup"><span data-stu-id="04bcf-239">Ability to register single tenant apps.</span></span>
* <span data-ttu-id="04bcf-240">Atualizações para o servicePrincipal.</span><span class="sxs-lookup"><span data-stu-id="04bcf-240">Updates to servicePrincipal.</span></span>
* <span data-ttu-id="04bcf-241">Migração de aplicativos Azure AD existentes para um modelo atualizado.</span><span class="sxs-lookup"><span data-stu-id="04bcf-241">Migration of existing Azure AD apps to updated model.</span></span>
* <span data-ttu-id="04bcf-242">Suporte para appRoles, clientes pré-autorizados, reivindicações opcionais, reivindicações de associação de grupo e identidade visual.</span><span class="sxs-lookup"><span data-stu-id="04bcf-242">Support for appRoles, pre-authorized clients, optional claims, group membership claims, and branding</span></span>
* <span data-ttu-id="04bcf-243">Os usuários de conta Microsoft (MSA) podem registrar aplicativos.</span><span class="sxs-lookup"><span data-stu-id="04bcf-243">Microsoft account (MSA) users can register apps.</span></span>
* <span data-ttu-id="04bcf-244">Suporte para protocolos SAML e WsFed.</span><span class="sxs-lookup"><span data-stu-id="04bcf-244">Support for SAML and WsFed protocols.</span></span>

## <a name="identity-and-access--conditional-access"></a><span data-ttu-id="04bcf-245">Identidade e acesso | Acesso condicional</span><span class="sxs-lookup"><span data-stu-id="04bcf-245">Identity and access | Conditional access</span></span>

### <a name="permissions"></a><span data-ttu-id="04bcf-246">Permissões</span><span class="sxs-lookup"><span data-stu-id="04bcf-246">Permissions</span></span>

<span data-ttu-id="04bcf-247">Atualmente, a permissão Policy.Read.All é necessária para chamar as APIs POST e PATCH.</span><span class="sxs-lookup"><span data-stu-id="04bcf-247">Currently, the Policy.Read.All permission is required to call POST and PATCH APIs.</span></span> <span data-ttu-id="04bcf-248">No futuro, a permissão Policy.ReadWrite.ConditionalAccess possibilitará que você leia as políticas do diretório.</span><span class="sxs-lookup"><span data-stu-id="04bcf-248">In the future, the Policy.ReadWrite.ConditionalAccess permission will enable you to read policies from the directory.</span></span>

## <a name="json-batching"></a><span data-ttu-id="04bcf-249">Envio em lote JSON</span><span class="sxs-lookup"><span data-stu-id="04bcf-249">JSON Batching</span></span>

### <a name="no-nested-batch"></a><span data-ttu-id="04bcf-250">Nenhum lote aninhado</span><span class="sxs-lookup"><span data-stu-id="04bcf-250">No nested batch</span></span>

<span data-ttu-id="04bcf-251">Solicitações de lote JSON não devem conter quaisquer solicitações em lotes aninhados.</span><span class="sxs-lookup"><span data-stu-id="04bcf-251">JSON batch requests must not contain any nested batch requests.</span></span>

### <a name="all-individual-requests-must-be-synchronous"></a><span data-ttu-id="04bcf-252">Todas as solicitações individuais devem ser síncronas</span><span class="sxs-lookup"><span data-stu-id="04bcf-252">All individual requests must be synchronous</span></span>

<span data-ttu-id="04bcf-253">All requests contained in a batch request must be executed synchronously.</span><span class="sxs-lookup"><span data-stu-id="04bcf-253">All requests contained in a batch request must be executed synchronously.</span></span> <span data-ttu-id="04bcf-254">If present, the `respond-async` preference will be ignored.</span><span class="sxs-lookup"><span data-stu-id="04bcf-254">If present, the `respond-async` preference will be ignored.</span></span>

### <a name="no-transactions"></a><span data-ttu-id="04bcf-255">Sem transações</span><span class="sxs-lookup"><span data-stu-id="04bcf-255">No transactions</span></span>

<span data-ttu-id="04bcf-256">Microsoft Graph does not currently support transactional processing of individual requests.</span><span class="sxs-lookup"><span data-stu-id="04bcf-256">Microsoft Graph does not currently support transactional processing of individual requests.</span></span> <span data-ttu-id="04bcf-257">The `atomicityGroup` property on individual requests will be ignored.</span><span class="sxs-lookup"><span data-stu-id="04bcf-257">The `atomicityGroup` property on individual requests will be ignored.</span></span>

### <a name="uris-must-be-relative"></a><span data-ttu-id="04bcf-258">URIs devem ser relativas</span><span class="sxs-lookup"><span data-stu-id="04bcf-258">URIs must be relative</span></span>

<span data-ttu-id="04bcf-259">Always specify relative URIs in batch requests.</span><span class="sxs-lookup"><span data-stu-id="04bcf-259">Always specify relative URIs in batch requests.</span></span> <span data-ttu-id="04bcf-260">Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span><span class="sxs-lookup"><span data-stu-id="04bcf-260">Microsoft Graph then makes these URLs absolute by using the version endpoint included in the batch URL.</span></span>

### <a name="limit-on-batch-size"></a><span data-ttu-id="04bcf-261">Limite de tamanho de lote</span><span class="sxs-lookup"><span data-stu-id="04bcf-261">Limit on batch size</span></span>

<span data-ttu-id="04bcf-262">No momento, as solicitações de lote JSON estão limitadas a 20 solicitações individuais.</span><span class="sxs-lookup"><span data-stu-id="04bcf-262">JSON batch requests are currently limited to 20 individual requests.</span></span>

### <a name="simplified-dependencies"></a><span data-ttu-id="04bcf-263">Dependências simplificadas</span><span class="sxs-lookup"><span data-stu-id="04bcf-263">Simplified dependencies</span></span>

<span data-ttu-id="04bcf-264">Individual requests can depend on other individual requests.</span><span class="sxs-lookup"><span data-stu-id="04bcf-264">Individual requests can depend on other individual requests.</span></span> <span data-ttu-id="04bcf-265">Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span><span class="sxs-lookup"><span data-stu-id="04bcf-265">Currently, requests can only depend on a single other request, and must follow one of these three patterns:</span></span>

1. <span data-ttu-id="04bcf-266">Paralelo – nenhuma solicitação individual declara uma dependência na propriedade `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="04bcf-266">Parallel - no individual request states a dependency in the `dependsOn` property.</span></span>
2. <span data-ttu-id="04bcf-267">Serial – todas as solicitações individuais dependem da solicitação individual anterior.</span><span class="sxs-lookup"><span data-stu-id="04bcf-267">Serial - all individual requests depend on the previous individual request.</span></span>
3. <span data-ttu-id="04bcf-268">Mesmo – todas as solicitações individuais indicam que uma dependência na propriedade `dependsOn` declaram a mesma dependência.</span><span class="sxs-lookup"><span data-stu-id="04bcf-268">Same - all individual requests that state a dependency in the `dependsOn` property, state the same dependency.</span></span>

<span data-ttu-id="04bcf-269">Conforme o processamento em lotes JSON amadurece, essas limitações são removidas.</span><span class="sxs-lookup"><span data-stu-id="04bcf-269">As JSON batching matures, these limitations will be removed.</span></span>

## <a name="mail-outlook"></a><span data-ttu-id="04bcf-270">Email (Outlook)</span><span class="sxs-lookup"><span data-stu-id="04bcf-270">Mail (Outlook)</span></span>

### <a name="attaching-large-files-to-messages"></a><span data-ttu-id="04bcf-271">Anexando grandes arquivos a mensagens</span><span class="sxs-lookup"><span data-stu-id="04bcf-271">Attaching large files to messages</span></span>
<span data-ttu-id="04bcf-272">Um aplicativo com permissões delegadas retorna `HTTP 403 Forbidden` ao tentar [anexar arquivos grandes](outlook-large-attachments.md) a uma mensagem ou evento do Outlook que está em uma caixa de correio compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="04bcf-272">An app with delegated permissions returns `HTTP 403 Forbidden` when attempting to [attach large files](outlook-large-attachments.md) to an Outlook message or event that is in a shared or delegated mailbox.</span></span> <span data-ttu-id="04bcf-273">Com as permissões delegadas, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) só é bem sucedida se a mensagem ou o evento estiver na caixa de correio do usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="04bcf-273">With delegated permissions, [createUploadSession](/graph/api/attachment-createuploadsession?view=graph-rest-1.0) succeeds only if the message or event is in the signed-in user's mailbox.</span></span>

### <a name="the-comment-parameter-for-creating-a-draft"></a><span data-ttu-id="04bcf-274">O parâmetro de comentário para criar um rascunho</span><span class="sxs-lookup"><span data-stu-id="04bcf-274">The comment parameter for creating a draft</span></span>

<span data-ttu-id="04bcf-275">O parâmetro **comment** para criar uma resposta ou rascunho de encaminhamento ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) não se torna parte do corpo do rascunho de mensagem resultante.</span><span class="sxs-lookup"><span data-stu-id="04bcf-275">The **comment** parameter for creating a reply or forward draft ([createReply](/graph/api/message-createreply?view=graph-rest-1.0), [createReplyAll](/graph/api/message-createreplyall?view=graph-rest-1.0), [createForward](/graph/api/message-createforward?view=graph-rest-1.0)) does not become part of the body of the resultant message draft.</span></span>

### <a name="get-messages-returns-chats-in-microsoft-teams"></a><span data-ttu-id="04bcf-276">As mensagens GET retornam chats no Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="04bcf-276">GET messages returns chats in Microsoft Teams</span></span>

<span data-ttu-id="04bcf-277">Em pontos de extremidade beta e v1, a resposta de `GET /users/id/messages` inclui chats do usuário no Microsoft Teams que ocorreu fora do escopo de uma equipe ou de um canal.</span><span class="sxs-lookup"><span data-stu-id="04bcf-277">In both the v1 and beta endpoints, the response of `GET /users/id/messages` includes the user's Microsoft Teams chats that occurred outside the scope of a team or channel.</span></span> <span data-ttu-id="04bcf-278">Essas mensagens de chat tem "IM" como o assunto.</span><span class="sxs-lookup"><span data-stu-id="04bcf-278">These chat messages have "IM" as their subject.</span></span>

## <a name="teamwork-microsoft-teams"></a><span data-ttu-id="04bcf-279">Trabalho em equipe (Microsoft Teams)</span><span class="sxs-lookup"><span data-stu-id="04bcf-279">Teamwork (Microsoft Teams)</span></span>

### <a name="get-teams-is-not-supported"></a><span data-ttu-id="04bcf-280">GET /teams não tem suporte</span><span class="sxs-lookup"><span data-stu-id="04bcf-280">GET /teams is not supported</span></span>

<span data-ttu-id="04bcf-281">Para obter uma lista de equipes, confira [listar todas as equipes](teams-list-all-teams.md) e [listar suas equipes](/graph/api/user-list-joinedteams?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="04bcf-281">To get a list of teams, see [list all teams](teams-list-all-teams.md) and [list your teams](/graph/api/user-list-joinedteams?view=graph-rest-1.0).</span></span>

### <a name="post-teams-is-only-available-in-beta"></a><span data-ttu-id="04bcf-282">POST /teams está disponível apenas na versão beta</span><span class="sxs-lookup"><span data-stu-id="04bcf-282">POST /teams is only available in beta</span></span>
<span data-ttu-id="04bcf-283">Para criar equipes no v 1.0, confira [criar equipe](/graph/api/team-put-teams?view=graph-rest-1.0).</span><span class="sxs-lookup"><span data-stu-id="04bcf-283">To create teams in v1.0, see [create team](/graph/api/team-put-teams?view=graph-rest-1.0).</span></span>

### <a name="missing-teams-in-list-all-teams"></a><span data-ttu-id="04bcf-284">Equipes ausentes em listas todas as equipes</span><span class="sxs-lookup"><span data-stu-id="04bcf-284">Missing teams in list all teams</span></span>

<span data-ttu-id="04bcf-285">Algumas equipes que foram criadas no passado mas não foram usadas recentemente por um usuário do Microsoft Teams não são listadas por [listar todas as equipes](teams-list-all-teams.md).</span><span class="sxs-lookup"><span data-stu-id="04bcf-285">Some teams that were created in the past but haven't been used recently by a Microsoft Teams user aren't listed by [list all teams](teams-list-all-teams.md).</span></span>
<span data-ttu-id="04bcf-286">Novas equipes serão listadas.</span><span class="sxs-lookup"><span data-stu-id="04bcf-286">New teams will be listed.</span></span>
<span data-ttu-id="04bcf-287">Algumas equipes antigas não têm uma propriedade **resourceProvisioningOptions** que contém “Equipe”, que é configurada em equipes recém-criadas e equipes que são visitadas no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="04bcf-287">Certain old teams don't have a **resourceProvisioningOptions** property that contains "Team", which is set on newly created teams and teams that are visited in Microsoft Teams.</span></span>
<span data-ttu-id="04bcf-288">No futuro, vamos configurar **resourceProvisioningOptions** em equipes existentes que não foram abertas no Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="04bcf-288">In the future, we will set **resourceProvisioningOptions** on existing teams that have not been opened in Microsoft Teams.</span></span>

## <a name="users"></a><span data-ttu-id="04bcf-289">Usuários</span><span class="sxs-lookup"><span data-stu-id="04bcf-289">Users</span></span>

### <a name="no-instant-access-after-creation"></a><span data-ttu-id="04bcf-290">Sem acesso instantâneo após a criação</span><span class="sxs-lookup"><span data-stu-id="04bcf-290">No instant access after creation</span></span>

<span data-ttu-id="04bcf-291">Users can be created immediately through a POST on the user entity.</span><span class="sxs-lookup"><span data-stu-id="04bcf-291">Users can be created immediately through a POST on the user entity.</span></span> <span data-ttu-id="04bcf-292">An Office 365 license must first be assigned to a user, in order to get access to Office 365 services.</span><span class="sxs-lookup"><span data-stu-id="04bcf-292">An Office 365 license must first be assigned to a user, in order to get access to Office 365 services.</span></span> <span data-ttu-id="04bcf-293">Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="04bcf-293">Even then, due to the distributed nature of the service, it might take 15 minutes before files, messages and events entities are available for use for this user, through the Microsoft Graph API.</span></span> <span data-ttu-id="04bcf-294">During this time, apps will receive a 404 HTTP error response.</span><span class="sxs-lookup"><span data-stu-id="04bcf-294">During this time, apps will receive a 404 HTTP error response.</span></span>

### <a name="photo-restrictions"></a><span data-ttu-id="04bcf-295">Restrições de foto</span><span class="sxs-lookup"><span data-stu-id="04bcf-295">Photo restrictions</span></span>

<span data-ttu-id="04bcf-296">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span><span class="sxs-lookup"><span data-stu-id="04bcf-296">Reading and updating a user's profile photo is only possible if the user has a mailbox.</span></span> <span data-ttu-id="04bcf-297">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.</span><span class="sxs-lookup"><span data-stu-id="04bcf-297">Additionally, any photos that *may* have been previously stored using the **thumbnailPhoto** property (using the Office 365 unified API preview, or the Azure AD Graph, or through AD Connect synchronization) are no longer accessible through the Microsoft Graph **photo** property of the [user](/graph/api/resources/user?view=graph-rest-1.0) resource.</span></span>
<span data-ttu-id="04bcf-298">Failure to read or update a photo, in this case, would result in the following error:</span><span class="sxs-lookup"><span data-stu-id="04bcf-298">Failure to read or update a photo, in this case, would result in the following error:</span></span>

```javascript
{
  "error": {
    "code": "ErrorNonExistentMailbox",
    "message": "The SMTP address has no mailbox associated with it."
  }
}
```

### <a name="using-delta-query"></a><span data-ttu-id="04bcf-299">Uso da consulta delta</span><span class="sxs-lookup"><span data-stu-id="04bcf-299">Using delta query</span></span>

<span data-ttu-id="04bcf-300">Para saber mais sobre problemas conhecidos com o uso da consulta delta, veja a [seção da consulta delta](#delta-query) deste artigo.</span><span class="sxs-lookup"><span data-stu-id="04bcf-300">For known issues using delta query, see the [delta query section](#delta-query) in this article.</span></span>

### <a name="revoke-sign-in-sessions-returns-wrong-http-code"></a><span data-ttu-id="04bcf-301">A revogação de sessões de entrada retorna um código HTTP errado</span><span class="sxs-lookup"><span data-stu-id="04bcf-301">Revoke sign-in sessions returns wrong HTTP code</span></span>

<span data-ttu-id="04bcf-302">O [usuário: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) deve retornar uma resposta `204 No content` para ter revogações bem-sucedidas e um código de erro HTTP (4xx ou 5xx) se algo der errado com a solicitação.</span><span class="sxs-lookup"><span data-stu-id="04bcf-302">The [user: revokeSignInSessions API](/graph/api/user-revokesigninsessions?view=graph-rest-1.0) should return a `204 No content` response for successful revocations, and an HTTP error code (4xx or 5xx) if anything goes wrong with the request.</span></span>  <span data-ttu-id="04bcf-303">No entanto, devido a um problema de serviço, essa API retorna um parâmetro `200 OK` e um parâmetro booleano que é sempre true.</span><span class="sxs-lookup"><span data-stu-id="04bcf-303">However, due to a service issue, this API returns a `200 OK` and a Boolean parameter that is always true.</span></span>  <span data-ttu-id="04bcf-304">Até que isso seja corrigido, é recomendado que desenvolvedores simplesmente tratem qualquer código de retorno 2xx como bem-sucedido para esta API.</span><span class="sxs-lookup"><span data-stu-id="04bcf-304">Until this is fixed, developers are simply advised to treat any 2xx return code as success for this API.</span></span>

### <a name="incomplete-objects-when-using-getbyids-request"></a><span data-ttu-id="04bcf-305">Objetos incompletos ao usar a solicitação getByIds</span><span class="sxs-lookup"><span data-stu-id="04bcf-305">Incomplete objects when using getByIds request</span></span>

<span data-ttu-id="04bcf-306">A solicitação de objetos usando a opção de [Obter objetos de diretório de uma lista de IDs](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) deve retornar objetos completos.</span><span class="sxs-lookup"><span data-stu-id="04bcf-306">Requesting objects using [Get directory objects from a list of IDs](/graph/api/directoryobject-getbyids?view=graph-rest-1.0) should return full objects.</span></span> <span data-ttu-id="04bcf-307">No entanto, atualmente, os objetos de [usuário](/graph/api/resources/user?view=graph-rest-1.0) no ponto de extremidade v1.0 são retornados com um conjunto limitado de propriedades.</span><span class="sxs-lookup"><span data-stu-id="04bcf-307">However, currently [user](/graph/api/resources/user?view=graph-rest-1.0) objects on the v1.0 endpoint are returned with a limited set of properties.</span></span> <span data-ttu-id="04bcf-308">Como solução temporária, ao usar a operação em combinação com a opção de consulta `$select`, objetos de [usuário](/graph/api/resources/user?view=graph-rest-1.0) mais completos serão retornados.</span><span class="sxs-lookup"><span data-stu-id="04bcf-308">As a temporary workaround, when you use the operation in combination with the `$select` query option, more complete [user](/graph/api/resources/user?view=graph-rest-1.0) objects will be returned.</span></span> <span data-ttu-id="04bcf-309">Esse comportamento não está de acordo com as especificações do OData.</span><span class="sxs-lookup"><span data-stu-id="04bcf-309">This behavior is not in accordance with the OData specifications.</span></span> <span data-ttu-id="04bcf-310">Como esse comportamento pode ser atualizado no futuro, use esta solução alternativa apenas quando fornecer `$select=` com todas as propriedades de seu interesse e somente se futuras alterações nessa solução alternativa forem aceitáveis.</span><span class="sxs-lookup"><span data-stu-id="04bcf-310">Because this behavior might be updated in the future, use this workaround only when you provide `$select=` with all the properties you are interested in, and only if future breaking changes to this workaround are acceptable.</span></span>

## <a name="query-parameter-limitations"></a><span data-ttu-id="04bcf-311">Limitações de parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="04bcf-311">Query parameter limitations</span></span>

* <span data-ttu-id="04bcf-312">Não há suporte para vários namespaces.</span><span class="sxs-lookup"><span data-stu-id="04bcf-312">Multiple namespaces are not supported.</span></span>
* <span data-ttu-id="04bcf-313">Não há suporte para GETs em `$ref` e conversão em usuários, grupos, dispositivos, entidades de serviço e aplicativos.</span><span class="sxs-lookup"><span data-stu-id="04bcf-313">GETs on `$ref` and casting is not supported on users, groups, devices, service principals and applications.</span></span>
* <span data-ttu-id="04bcf-314">`@odata.bind` is not supported.</span><span class="sxs-lookup"><span data-stu-id="04bcf-314">`@odata.bind` is not supported.</span></span>  <span data-ttu-id="04bcf-315">This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span><span class="sxs-lookup"><span data-stu-id="04bcf-315">This means that developers won’t be able to properly set the **acceptedSenders** or **rejectedSenders** navigation property on a group.</span></span>
* <span data-ttu-id="04bcf-316">`@odata.id` não está presente na navegação sem confinamento (como mensagens) quando há o uso de metadados mínimos.</span><span class="sxs-lookup"><span data-stu-id="04bcf-316">`@odata.id` is not present on non-containment navigations (like messages) when using minimal metadata.</span></span>
* <span data-ttu-id="04bcf-317">`$expand`:</span><span class="sxs-lookup"><span data-stu-id="04bcf-317">`$expand`:</span></span>
  * <span data-ttu-id="04bcf-318">Não há suporte para `nextLink`</span><span class="sxs-lookup"><span data-stu-id="04bcf-318">No support for `nextLink`</span></span>
  * <span data-ttu-id="04bcf-319">Não há suporte para mais de um nível de expansão</span><span class="sxs-lookup"><span data-stu-id="04bcf-319">No support for more than 1 level of expand</span></span>
  * <span data-ttu-id="04bcf-320">Não há suporte com parâmetros adicionais (`$filter`, `$select`)</span><span class="sxs-lookup"><span data-stu-id="04bcf-320">No support with extra parameters (`$filter`, `$select`)</span></span>
* <span data-ttu-id="04bcf-321">`$filter`:</span><span class="sxs-lookup"><span data-stu-id="04bcf-321">`$filter`:</span></span>
  * <span data-ttu-id="04bcf-322">Não há suporte para filtros no ponto de extremidade `/attachments`.</span><span class="sxs-lookup"><span data-stu-id="04bcf-322">`/attachments` endpoint does not support filters.</span></span> <span data-ttu-id="04bcf-323">Se presente, o parâmetro `$filter` é ignorado.</span><span class="sxs-lookup"><span data-stu-id="04bcf-323">If present, the `$filter` parameter is ignored.</span></span>
  * <span data-ttu-id="04bcf-324">Não há suporte para filtragem de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="04bcf-324">Cross-workload filtering is not supported.</span></span>
* <span data-ttu-id="04bcf-325">`$search`:</span><span class="sxs-lookup"><span data-stu-id="04bcf-325">`$search`:</span></span>
  * <span data-ttu-id="04bcf-326">A pesquisa de texto completo só está disponível para um subconjunto de entidades, como mensagens.</span><span class="sxs-lookup"><span data-stu-id="04bcf-326">Full-text search is only available for a subset of entities such as messages.</span></span>
  * <span data-ttu-id="04bcf-327">Não há suporte para pesquisa de carga de trabalho cruzada.</span><span class="sxs-lookup"><span data-stu-id="04bcf-327">Cross-workload searching is not supported.</span></span>


## <a name="functionality-available-only-in-office-365-rest-or-azure-ad-graph-apis"></a><span data-ttu-id="04bcf-328">Funcionalidade disponível apenas nas APIs Graph do Azure AD ou REST do Office 365</span><span class="sxs-lookup"><span data-stu-id="04bcf-328">Functionality available only in Office 365 REST or Azure AD Graph APIs</span></span>

<span data-ttu-id="04bcf-329">Alguns recursos ainda não estão disponíveis no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="04bcf-329">Some functionality is not yet available in Microsoft Graph.</span></span> <span data-ttu-id="04bcf-330">Se você não vir a funcionalidade que está procurando, poderá usar as [APIs REST do Office 365](https://docs.microsoft.com/previous-versions/office/office-365-api/) específicas do ponto de extremidade.</span><span class="sxs-lookup"><span data-stu-id="04bcf-330">If you don't see the functionality you're looking for, you can use the endpoint-specific [Office 365 REST APIs](https://docs.microsoft.com/previous-versions/office/office-365-api/).</span></span> <span data-ttu-id="04bcf-331">Para o Azure Active Directory, confira [Migrar aplicativos do Azure AD Graph para o Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="04bcf-331">For Azure Active Directory, see [Migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span> 
