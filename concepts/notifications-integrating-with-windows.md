---
title: Integração do aplicativo UWP do Windows no SDK do lado do cliente para notificações ao usuário
description: Integre o aplicativo UWP do Windows com notificações de usuário no SDK do cliente.
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: e389e9c319cb2841aa0ddf1dc697134c8c7f4011
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063247"
---
# <a name="integrate-your-windows-uwp-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="e81f9-103">Integração do aplicativo UWP do Windows no SDK do lado do cliente para notificações ao usuário</span><span class="sxs-lookup"><span data-stu-id="e81f9-103">Integrate your Windows UWP app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="e81f9-104">Após [registrar seu aplicativo](notifications-integration-app-registration.md) no Portal do Azure e integrar suas [experiências entre dispositivos](notifications-integration-cross-device-experiences-onboarding.md) no Partner Center de desenvolvimento, a próxima etapa é integrar seu aplicativo de cliente com o SDK do lado do cliente para o aplicativo UWP do Windows.</span><span class="sxs-lookup"><span data-stu-id="e81f9-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK for Windows UWP apps.</span></span>  

<span data-ttu-id="e81f9-105">Com o SDK do cliente, o aplicativo pode executar as etapas necessárias de registro para receber notificações publicadas do servidor do aplicativo direcionadas ao usuário conectado atualmente.</span><span class="sxs-lookup"><span data-stu-id="e81f9-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="e81f9-106">O SDK então gerencia as notificações no lado do cliente, incluindo receber novas notificações, gerenciar o estado de notificações para alcançar cenários como descartar de forma universal e recuperar o histórico completo de notificações.</span><span class="sxs-lookup"><span data-stu-id="e81f9-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="e81f9-107">Fluxo de notificação de entrada</span><span class="sxs-lookup"><span data-stu-id="e81f9-107">New incoming notification flow</span></span>

<span data-ttu-id="e81f9-108">Para receber novas notificações, o fluxo de dados é mostrado no diagrama a seguir.</span><span class="sxs-lookup"><span data-stu-id="e81f9-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Fluxo de nova notificação para aplicativo do Windows](images/notifications-new-notification-windows.png)

<span data-ttu-id="e81f9-110">O processo envolve alguns componentes:</span><span class="sxs-lookup"><span data-stu-id="e81f9-110">The process involves a few components:</span></span>

* <span data-ttu-id="e81f9-111">Servidor de aplicativo – back-end do aplicativo</span><span class="sxs-lookup"><span data-stu-id="e81f9-111">App server - The back end of your application</span></span>
* <span data-ttu-id="e81f9-112">Cliente do aplicativo – front-end do aplicativo (um aplicativo UWP, Android ou iOS)</span><span class="sxs-lookup"><span data-stu-id="e81f9-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="e81f9-113">Notificações do Microsoft Graph – o componente do serviço que permite que notificações ao usuário sejam publicadas, armazenadas e sincronizadas em instâncias diferentes dos clientes do aplicativo em vários dispositivos e plataformas</span><span class="sxs-lookup"><span data-stu-id="e81f9-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="e81f9-114">WNS – o serviço de notificação por push do Windows que as notificações do Microsoft Graph usa para sinalizar clientes</span><span class="sxs-lookup"><span data-stu-id="e81f9-114">WNS - The Windows push notification service that Microsoft Graph notifications uses to signal the clients</span></span>

<span data-ttu-id="e81f9-115">O diagrama mostra as próximas etapas:</span><span class="sxs-lookup"><span data-stu-id="e81f9-115">The diagram shows the following steps:</span></span> 

1. <span data-ttu-id="e81f9-116">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-116">Application logic.</span></span> <span data-ttu-id="e81f9-117">Essa etapa captura o que aciona a notificação para ser publicada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-117">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="e81f9-118">Isso é lógica específica do aplicativo e pode ser uma atualização de dados ou evento sobre algo diferente do Microsoft Graph, como um novo evento do calendário ou atribuição de tarefas, ou o que o serviço de aplicativo quer notificar o usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-118">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="e81f9-119">O servidor do aplicativo publica uma notificação para o usuário alvo pela API de notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e81f9-119">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="e81f9-120">Para saber mais, consulte [integração com o lado do servidor](notifications-integrating-app-server.md).</span><span class="sxs-lookup"><span data-stu-id="e81f9-120">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="e81f9-121">Ao receber a solicitação Web com nova notificação, as notificações do Microsoft Graph mantêm o conteúdo da notificação em segurança na nuvem para esse aplicativo e esse usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-121">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="e81f9-122">Para cada instância do cliente do aplicativo inscrita para receber notificações para esse usuário, as notificações do Microsoft Graph envia um sinal para notificar cliente do aplicativo, por meio do serviço de envio por push nativo fornecido pelo sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e81f9-122">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="e81f9-123">Nesse caso, o aplicativo é um aplicativo UWP no Windows, e ele usa [notificação bruta WNS](https://docs.microsoft.com/pt-BR/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) enviar o sinal.</span><span class="sxs-lookup"><span data-stu-id="e81f9-123">In this case, the application is a UWP app on Windows, and it uses [WNS push raw notification](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) to send the signal.</span></span> 
5. <span data-ttu-id="e81f9-124">Depois que o aplicativo for sinalizado pelas notificações por push de entrada, ele pede ao SDK para buscar as alterações no repositório de notificações do usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-124">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="e81f9-125">O SDK estabelece uma conexão segura e compatível com o repositório de notificações do usuário no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e81f9-125">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="e81f9-126">O SDK recebe as alterações de dados – nesse caso, o novo conteúdo de notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-126">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="e81f9-127">O SDK dispara retornos de chamada de evento para notificar o aplicativo após a recuperação com êxito das alterações.</span><span class="sxs-lookup"><span data-stu-id="e81f9-127">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="e81f9-128">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-128">Application logic.</span></span> <span data-ttu-id="e81f9-129">Essa etapa captura o que o aplicativo escolhe fazer dentro retorno de chamada do evento.</span><span class="sxs-lookup"><span data-stu-id="e81f9-129">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="e81f9-130">Normalmente, isso resulta em alterações locais de dados do aplicativo e atualizações de interface do usuário locais.</span><span class="sxs-lookup"><span data-stu-id="e81f9-130">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="e81f9-131">Nesse caso, o aplicativo geralmente cria uma pop-up de notificação do sistema para notificar o usuário sobre o conteúdo de notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-131">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="e81f9-132">Fluxo de atualização de notificação</span><span class="sxs-lookup"><span data-stu-id="e81f9-132">Notification update flow</span></span>

<span data-ttu-id="e81f9-133">Uma das principais vantagens de usar as notificações do Microsoft Graph é que ele mantêm as notificações na nuvem com segurança e as transforma em um tipo de recurso com estado.</span><span class="sxs-lookup"><span data-stu-id="e81f9-133">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="e81f9-134">Portanto, ele pode ajudar o aplicativo a gerenciar e a sincronizar o estado correto das notificações em diferentes dispositivos para o usuário conectado em um cenário entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e81f9-134">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="e81f9-135">Quando uma notificação estiver marcada como descartada ou como lida em um dispositivo, os outros dispositivos podem ser notificados em tempo real.</span><span class="sxs-lookup"><span data-stu-id="e81f9-135">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="e81f9-136">"Manipulada uma vez, descartada em qualquer lugar" pode se tornar a promessa real como parte da experiência de notificação para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="e81f9-136">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="e81f9-137">O diagrama a seguir mostra o fluxo de dados para alterar o estado de uma notificação ou excluir a notificação em um dispositivo e receber/manipular a alteração de estado ou a exclusão em outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-137">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Atualização de fluxo de notificação para aplicativo do Windows](images/notifications-notification-update-windows.png)

<span data-ttu-id="e81f9-139">Observe que a segunda parte do fluxo é semelhante ao fluxo de tratamento de novas notificações de entrada.</span><span class="sxs-lookup"><span data-stu-id="e81f9-139">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="e81f9-140">Isso é esperado – o padrão de programação no SDK  foi projetado para que o cliente do aplicativo possa lidar com todos os tipos de alterações de dados de notificações do usuário (novas notificações de entrada, alterações de estado de notificação, notificação excluída) de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="e81f9-140">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="e81f9-141">O diagrama mostra as próximas etapas:</span><span class="sxs-lookup"><span data-stu-id="e81f9-141">The diagram shows the following steps:</span></span>

1. <span data-ttu-id="e81f9-142">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-142">Application logic.</span></span> <span data-ttu-id="e81f9-143">Algo aciona a notificação para ser alterada ou excluída.</span><span class="sxs-lookup"><span data-stu-id="e81f9-143">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="e81f9-144">Em geral, qualquer evento possível pode acionar a alteração de uma notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-144">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="e81f9-145">Chamada do aplicativo para o SDK do cliente para atualizar ou excluir uma notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-145">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="e81f9-146">Atualmente, expomos duas propriedades sobre alterações de estado – **userActionState** e **readState** – mas o aplicativo pode definir esses estados e quando eles precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="e81f9-146">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="e81f9-147">Por exemplo, quando um usuário descartar a notificação pop-up, você pode atualizar o **userActionState** para Descartado.</span><span class="sxs-lookup"><span data-stu-id="e81f9-147">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="e81f9-148">Quando um usuário clica na notificação pop-up e inicia o aplicativo para consumir o conteúdo correspondente do aplicativo, você pode atualizar o **userActionState** para ativado e atualizar o **readState** para Lido.</span><span class="sxs-lookup"><span data-stu-id="e81f9-148">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="e81f9-149">Depois que a API correspondente é chamada para atualizar ou excluir uma notificação, o SDK irá chamar o repositório na nuvem de notificação de usuário para dispersar essa alteração para as outras instâncias de cliente do aplicativo com o mesmo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e81f9-149">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="e81f9-150">Ao receber a solicitação de atualização/exclusão de um cliente, as notificações do Microsoft Graph irão atualizar o repositório de notificação e identificar as outras instâncias de cliente do aplicativo inscritas para essa alteração.</span><span class="sxs-lookup"><span data-stu-id="e81f9-150">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="e81f9-151">Para cada inscrição do cliente do aplicativo, as notificações do Microsoft Graph envia um sinal para notificar cliente do aplicativo, por meio do serviço de envio por push nativo fornecido pelo sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="e81f9-151">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="e81f9-152">Nesse caso, esse é um aplicativo UWP no Windows, e ele usa [notificação bruta WNS](https://docs.microsoft.com/pt-BR/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) para enviar o sinal.</span><span class="sxs-lookup"><span data-stu-id="e81f9-152">In this case, this is a UWP app on Windows, and it uses [WNS push raw notification](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/raw-notification-overview) to send the signal.</span></span> 
6. <span data-ttu-id="e81f9-153">Depois que o aplicativo for sinalizado pelas notificações por push de entrada, ele pede ao SDK para buscar as alterações no repositório de notificações do usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-153">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="e81f9-154">O SDK estabelece uma conexão segura e compatível com o repositório de notificações do usuário no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e81f9-154">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="e81f9-155">O SDK recebe as alterações de dados – nesse caso, as alterações são atualizações de notificação de estado ou exclusões de notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-155">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="e81f9-156">O SDK dispara retornos de chamada de evento para notificar o aplicativo após a recuperação com êxito das alterações.</span><span class="sxs-lookup"><span data-stu-id="e81f9-156">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="e81f9-157">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-157">Application logic.</span></span> <span data-ttu-id="e81f9-158">Essa etapa captura o que o aplicativo escolhe fazer dentro retorno de chamada do evento.</span><span class="sxs-lookup"><span data-stu-id="e81f9-158">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="e81f9-159">Normalmente, isso resulta em alterações locais de dados do aplicativo e atualizações de interface do usuário locais.</span><span class="sxs-lookup"><span data-stu-id="e81f9-159">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="e81f9-160">Nesse caso, como há atualizações de notificação, o aplicativo deve atualizar a interface do usuário no local para refletir a alteração de estado.</span><span class="sxs-lookup"><span data-stu-id="e81f9-160">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="e81f9-161">Por exemplo, se uma notificação estiver marcada como ativada, você pode remover a notificação pop-up do sistema correspondente dentro da central de ações do Windows para obter "manipulada uma vez, descartada em todo lugar".</span><span class="sxs-lookup"><span data-stu-id="e81f9-161">For example, if a notification is marked as activated, you can remove the corresponding toast notification popup inside Windows action center to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="e81f9-162">Para obter mais informações sobre as notificações do Microsoft Graph, consulte a  [visão geral das notificações do Microsoft Graph](notifications-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="e81f9-162">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="e81f9-163">Para saber mais sobre as etapas necessárias para integrar com as notificações do Microsoft Graph de ponta a ponta, confira a [visão geral da integração](notifications-integration-e2e-overview.md) das notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e81f9-163">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="e81f9-164">Adicionar o SDK ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="e81f9-164">Adding the OfficeThemes.css file to your project</span></span>

<span data-ttu-id="e81f9-165">No Windows, o SDK do lado do cliente é um pacote do NuGet que envia fora do sistema operacional Windows.</span><span class="sxs-lookup"><span data-stu-id="e81f9-165">On Windows, the client-side SDK is a NuGet package that ships outside of the Windows operating system.</span></span> <span data-ttu-id="e81f9-166">Essa API está disponível no C#, C++, e WinJS.</span><span class="sxs-lookup"><span data-stu-id="e81f9-166">This API is available in C#, C++, and WinJS.</span></span> 

<span data-ttu-id="e81f9-167">Baixe o pacote do NuGet para as notificações SDK do Microsoft Graph para aplicativos do Windows no [nuget](https://www.nuget.org/packages/Microsoft.ConnectedDevices.UserNotifications), ou use as etapas a seguir para baixá-lo da solução do aplicativo no Visual Studio:</span><span class="sxs-lookup"><span data-stu-id="e81f9-167">Download the NuGet package for the Microsoft Graph notifications SDK for Windows apps on [nuget](https://www.nuget.org/packages/Microsoft.ConnectedDevices.UserNotifications), or use the following steps to download it from your app solution in Visual Studio:</span></span> 

<span data-ttu-id="e81f9-168">No Visual Studio, clique com o botão direito do mouse no projeto para abrir o menu de contexto, e depois clique em **Gerenciar pacotes do NuGet...**.</span><span class="sxs-lookup"><span data-stu-id="e81f9-168">In Visual Studio, right-click the project to bring up the context menu, and then click **Manage NuGet Packages…**.</span></span>

![Gerenciar Pacotes do NuGet](images/notifications-nuget-1-manage.png)

<span data-ttu-id="e81f9-170">Acesse a guia **Procurar** e pesquise por Microsoft.ConnectedDevices.UserNotifications.</span><span class="sxs-lookup"><span data-stu-id="e81f9-170">Go to the **Browse** tab, and search for Microsoft.ConnectedDevices.UserNotifications.</span></span>

![Encontrar pacotes do NuGet](images/notifications-nuget-2-find.png)

<span data-ttu-id="e81f9-172">Você verá as notificações do Microsoft Graph no SDK do lado do cliente nos resultados da pesquisa.</span><span class="sxs-lookup"><span data-stu-id="e81f9-172">You will see the Microsoft Graph notifications client-side SDK in the search results.</span></span> <span data-ttu-id="e81f9-173">Clique no botão **Instalar** para instalar o pacote..</span><span class="sxs-lookup"><span data-stu-id="e81f9-173">Click the **Install** button to install it.</span></span> 

![Instalar pacotes do NuGet](images/notifications-nuget-3-install.png)

<span data-ttu-id="e81f9-175">Após a conclusão da instalação, o pacote é exibido abaixo de **Referências** no Gerenciador de Soluções.</span><span class="sxs-lookup"><span data-stu-id="e81f9-175">After the installation finishes, the package shows up under **References** in the Solution Explorer.</span></span> 

<span data-ttu-id="e81f9-176">Para saber mais sobre a incluisão e o consumo de pacotes do NuGet de seu aplicativo UWP, confira:</span><span class="sxs-lookup"><span data-stu-id="e81f9-176">For more details about including and consuming NuGet packages from your UWP app, see:</span></span>

* <span data-ttu-id="e81f9-177">
  [Usar os pacotes do nuget.org](https://docs.microsoft.com/pt-BR/azure/devops/artifacts/nuget/upstream-sources?view=vsts&tabs=new-nav)</span><span class="sxs-lookup"><span data-stu-id="e81f9-177">[Use packages from nuget.org](https://docs.microsoft.com/en-us/azure/devops/artifacts/nuget/upstream-sources?view=vsts&tabs=new-nav)</span></span>
* <span data-ttu-id="e81f9-178">
  [Início rápido: Instalar e usar um pacote no Visual Studio](https://docs.microsoft.com/pt-BR/nuget/quickstart/install-and-use-a-package-in-visual-studio)</span><span class="sxs-lookup"><span data-stu-id="e81f9-178">[Quickstart: Install and use a package in Visual Studio](https://docs.microsoft.com/en-us/nuget/quickstart/install-and-use-a-package-in-visual-studio)</span></span>


## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="e81f9-179">Inicializando as Plataformas de Dispositivo Conectado</span><span class="sxs-lookup"><span data-stu-id="e81f9-179">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="e81f9-180">No SDK do lado do cliente é desenvolvido com base em uma infraestrutura chamada Plataforma de Dispositivo Conectado.</span><span class="sxs-lookup"><span data-stu-id="e81f9-180">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="e81f9-181">Antes de poder usar qualquer recurso, a plataforma deve ser inicializada em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-181">Before you can use any features, the platform must be initialized within your app.</span></span> <span data-ttu-id="e81f9-182">As etapas de inicialização que devem ocorrer em sua classe principal no método **OnLaunched** ou **onActivated**, porque eles são necessários para ocorrer os cenários de notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-182">The initialization steps should occur in your main class **OnLaunched** or **onActivated** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="e81f9-183">Você deve criar e inicializar a plataforma ao instanciar a classe **ConnectedDevicesPlatform**.</span><span class="sxs-lookup"><span data-stu-id="e81f9-183">You must construct and initialize the platform by instantiating the **ConnectedDevicesPlatform** class.</span></span> <span data-ttu-id="e81f9-184">Antes de fazer isso, certifique-se de conectar manipuladores de eventos, como mostrado, pois depois que a plataforma é iniciada, os eventos podem começar a acionar.</span><span class="sxs-lookup"><span data-stu-id="e81f9-184">Before doing that, make sure to hook up event handlers, as shown, because after platform is started, the events might begin to fire.</span></span> 


```C#
var platform = new ConnectedDevicesPlatform();
platform.AccountManager.AccessTokenRequested += AccountManager_AccessTokenRequestedAsync;
platform.AccountManager.AccessTokenInvalidated += AccountManager_AccessTokenInvalidated;
platform.NotificationRegistrationManager.NotificationRegistrationStateChanged += NotificationRegistrationManager_NotificationRegistrationStateChanged;
platform.Start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="e81f9-185">Gerenciar tokens de acesso à conta</span><span class="sxs-lookup"><span data-stu-id="e81f9-185">Handling account access token</span></span>

<span data-ttu-id="e81f9-186">Todas as chamadas de Web que o SDK realiza, incluindo a recuperação do conteúdo de uma nova notificação de entrada, atualização de notificação de estado e muito mais, são leituras de ou escrevendo para os dados do usuário e, portanto, sempre exigem um token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="e81f9-186">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="e81f9-187">O SDK requer que você trate os seguintes eventos – chamados quando um token de acesso for solicitado ou invalidado – para garantir que, depois da plataforma inicializar, o token de acesso do usuário seja tratado corretamente.</span><span class="sxs-lookup"><span data-stu-id="e81f9-187">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accountmanageraccesstokenrequestedasync"></a><span data-ttu-id="e81f9-188">AccountManager_AccessTokenRequestedAsync</span><span class="sxs-lookup"><span data-stu-id="e81f9-188">AccountManager_AccessTokenRequestedAsync</span></span>

<span data-ttu-id="e81f9-189">Para uma implementação completa, confira o [exemplo de aplicativo Windows](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span><span class="sxs-lookup"><span data-stu-id="e81f9-189">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private async void AccountManager_AccessTokenRequestedAsync(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args)
{
    private List<Account> accounts = new List<Account>();
    var account = accounts.Find((x) => x.EqualsTo(args.Request.Account));
    if (account != null)
    {
        try
        {
            var accessToken = await account.GetAccessTokenAsync(args.Request.Scopes);
            args.Request.CompleteWithAccessToken(accessToken);
        }
        catch (Exception ex)
        {
            args.Request.CompleteWithErrorMessage(ex.Message);
        }
    }
}
```

#### <a name="accountmanageraccesstokeninvalidated"></a><span data-ttu-id="e81f9-190">AccountManager_AccessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="e81f9-190">AccountManager_AccessTokenInvalidated</span></span>

<span data-ttu-id="e81f9-191">Para uma implementação completa, confira o [exemplo de aplicativo Windows](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span><span class="sxs-lookup"><span data-stu-id="e81f9-191">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private void AccountManager_AccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args)
{
    Logger.Instance.LogMessage($"Token Invalidated. AccountId: {args.Account.Id}, AccountType: {args.Account.Id}, scopes: {string.Join(" ", args.Scopes)}");
}
```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="e81f9-192">Gerenciar validade de registro de push</span><span class="sxs-lookup"><span data-stu-id="e81f9-192">Handling push registration expiration</span></span> 

<span data-ttu-id="e81f9-193">As notificações do Microsoft Graph usa o WNS, a plataforma de push nativa no Windows, para sinalizar o aplicativo de cliente sobre alterações de dados de notificações do usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-193">Microsoft Graph notifications uses WNS, the native push platform on Windows, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="e81f9-194">Isso acontece quando novas notificações recebidas forem publicadas do servidor de aplicativos, ou quando o estado de qualquer notificação é atualizado em outro dispositivo com o mesmo usuário conectado em um cenário entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="e81f9-194">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="e81f9-195">Por esse motivo, é necessário um canal WNS válido que permite que as notificações brutas por push para ter êxito.</span><span class="sxs-lookup"><span data-stu-id="e81f9-195">For this reason, a valid WNS channel that allows raw push notifications to come through successfully is required.</span></span> <span data-ttu-id="e81f9-196">O seguinte retorno de chamada de evento trata da validade do canal WNS por push.</span><span class="sxs-lookup"><span data-stu-id="e81f9-196">The following event callback handles WNS push channel expirations.</span></span> 

#### <a name="notificationregistrationmanagernotificationregistrationstatechanged"></a><span data-ttu-id="e81f9-197">NotificationRegistrationManager_NotificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="e81f9-197">NotificationRegistrationManager_NotificationRegistrationStateChanged</span></span>

<span data-ttu-id="e81f9-198">Para uma implementação completa, confira o [exemplo de aplicativo Windows](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span><span class="sxs-lookup"><span data-stu-id="e81f9-198">For a full implementation, see the [Windows app sample](https://github.com/Microsoft/project-rome/blob/master/Windows/samples/GraphNotificationsSample/ConnectedDevicesManager.cs).</span></span> 

```C#
private async void NotificationRegistrationManager_NotificationRegistrationStateChanged(ConnectedDevicesNotificationRegistrationManager sender, ConnectedDevicesNotificationRegistrationStateChangedEventArgs args)
{
    if ((args.State == ConnectedDevicesNotificationRegistrationState.Expired) || (args.State == ConnectedDevicesNotificationRegistrationState.Expiring))
    {
        var account = m_accounts.Find((x) => x.EqualsTo(args.Account));
        if (account != null)
        {
            await account.RegisterAccountWithSdkAsync();
        }
    }
}
```

## <a name="signing-in-your-user"></a><span data-ttu-id="e81f9-199">Entrar com seu usuário</span><span class="sxs-lookup"><span data-stu-id="e81f9-199">Signing in your user</span></span>

<span data-ttu-id="e81f9-200">As notificações do Microsoft Graph, como vários outros tipos de recursos no Microsoft Graph, são centralizadas em torno dos usuários.</span><span class="sxs-lookup"><span data-stu-id="e81f9-200">Microsoft Graph notifications, like many other resource types inside Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="e81f9-201">Para que o aplicativo assine e comece a receber notificações para o usuário conectado, primeiro é necessário obter um token OAuth válido a ser usado no processo de registro.</span><span class="sxs-lookup"><span data-stu-id="e81f9-201">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="e81f9-202">Você pode usar o método que preferir para gerar e gerenciamento os tokens OAuth.</span><span class="sxs-lookup"><span data-stu-id="e81f9-202">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="e81f9-203">Exemplo de aplicativo que usa ADAL.</span><span class="sxs-lookup"><span data-stu-id="e81f9-203">The sample app uses ADAL.</span></span> 

<span data-ttu-id="e81f9-204">Se você estiver usando uma conta da Microsoft, será necessário incluir as seguintes permissões em uma solicitação de entrada: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, e `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span><span class="sxs-lookup"><span data-stu-id="e81f9-204">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="e81f9-205">Se você estiver usando uma conta do Azure AD, você precisará solicitar o seguinte público: `https://cdpcs.access.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="e81f9-205">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>


## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="e81f9-206">Adicionar a conta de usuário à plataforma</span><span class="sxs-lookup"><span data-stu-id="e81f9-206">Adding the user account to the platform</span></span> 

<span data-ttu-id="e81f9-207">Será preciso registrar a conta do usuário conectado com o SDK.</span><span class="sxs-lookup"><span data-stu-id="e81f9-207">You need to register the signed in user account with the SDK.</span></span> <span data-ttu-id="e81f9-208">Isso envolve a adição de conta e registro de um canal de push para receber as notificações por push iniciais através do WNS.</span><span class="sxs-lookup"><span data-stu-id="e81f9-208">This involves adding the account and registering a push channel to receive the initial push notifications through WNS.</span></span> 

```C#
var account = new ConnectedDevicesAccount(accountId, accountType);           
var addResult = await platform.AccountManager.AddAccountAsync(account);
if (addResult.Status != ConnectedDevicesAccountAddedStatus.Success)
{
    throw new Exception("Add account failed with " + addResult.Status + "!");
}            

var pushChannel = await PushNotificationChannelManager.CreatePushNotificationChannelForApplicationAsync();
ConnectedDevicesNotificationRegistration registration = new ConnectedDevicesNotificationRegistration();
registration.Type = ConnectedDevicesNotificationType.WNS;
registration.Token = pushChannel.Uri;
var registerResult = await platform.NotificationRegistrationManager.RegisterAsync(account, registration);
if (registerResult.Status != ConnectedDevicesNotificationRegistrationStatus.Success)
{
    throw new Exception("Register push channel failed with " + registerResult.Status + "!");
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="e81f9-209">Inscrever-se para receber notificações do usuário</span><span class="sxs-lookup"><span data-stu-id="e81f9-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="e81f9-210">Você precisa instanciar um objeto **UserDataFeed** para o aplicativo para este usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="e81f9-210">You need to instantiate a **UserDataFeed** object for your application for this signed in user.</span></span> <span data-ttu-id="e81f9-211">O aplicativo é identificado pela ID de aplicativo multiplataforma fornecidas durante o processo de [integração de experiências entre dispositivos](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="e81f9-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md) process.</span></span>

```C#
UserDataFeed feed = UserDataFeed.GetForAccount(account, platform, "YOUR_HOST_HERE");

var scopes = new List<UserDataFeedSyncScope> { UserNotificationChannel.SyncScope };
var subscribeResult = await feed.SubscribeToSyncScopesAsync(scopes);
if (!subscribeResult)
{
    throw new Exception("Subsribe failed!");
}
var channel = new UserNotificationChannel(feed);
var reader = channel.CreateReader();
reader.DataChanged += Reader_DataChanged;
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="e81f9-212">Receber e gerenciar as notificações do usuário</span><span class="sxs-lookup"><span data-stu-id="e81f9-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="e81f9-213">O diagrama de fluxo já apresentado nesse tópico mostra que os padrões de programação para lidar com novas notificações de entrada de um servidor do aplicativo e uma atualização de notificação ou exclusão iniciado de outra instância do aplicativo do cliente são semelhantes.</span><span class="sxs-lookup"><span data-stu-id="e81f9-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="e81f9-214">A seguir estão as etapas para lidar com essas alterações de dados.</span><span class="sxs-lookup"><span data-stu-id="e81f9-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="e81f9-215">Gerenciar sinal de notificações por push de entrada</span><span class="sxs-lookup"><span data-stu-id="e81f9-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="e81f9-216">Todos os tipos de alterações de dados de notificações do usuário geram um sinal que é entregue para os clientes do aplicativo como uma notificação por push.</span><span class="sxs-lookup"><span data-stu-id="e81f9-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="e81f9-217">Para aplicativos UWP do Windows, o sinal será enviado como uma notificação bruta WNS por push.</span><span class="sxs-lookup"><span data-stu-id="e81f9-217">For Windows UWP apps, the signal is delivered as a WNS push raw notification.</span></span> <span data-ttu-id="e81f9-218">Ao receber sinal de notificação bruta por push, o aplicativo deve chamar **TryParse** para acionar o SDK para buscar no serviço de notificações do Microsoft Graph para as alterações de dados reais.</span><span class="sxs-lookup"><span data-stu-id="e81f9-218">On receiving the raw push signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```C#
public async Task ReceiveNotificationAsync(string content)
{
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.TryParse(content);
    if (notification != null)
    {
        await platform.ProcessNotificationAsync(notification);
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="e81f9-219">Gerenciar alterações de dados de notificação do usuário</span><span class="sxs-lookup"><span data-stu-id="e81f9-219">Handling user notification data changes</span></span>

<span data-ttu-id="e81f9-220">Após o SDK buscar com êxito as alterações de dados, um retorno de chamada do evento é invocado e o cliente de aplicativo deve lidar com a criação, atualização ou exclusão da notificação.</span><span class="sxs-lookup"><span data-stu-id="e81f9-220">After the SDK successfully fetches the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```C#
private async void Reader_DataChanged(UserNotificationReader reader, object args)
{
    var notifications = await reader.ReadBatchAsync(UInt32.MaxValue);

    foreach (var notification in notifications)
    {
        // Handle notification changes based on change type;
    }
}
```


### <a name="update-state-of-a-notification"></a><span data-ttu-id="e81f9-221">Atualização do estado de uma notificação</span><span class="sxs-lookup"><span data-stu-id="e81f9-221">Update state of a notification</span></span>

<span data-ttu-id="e81f9-222">Se a alteração do estado de notificação é iniciada da instância do cliente do aplicativo (por exemplo, se a notificação pop-up do sistema nesse dispositivo é ativada pelo usuário), o aplicativo deve chamar o SDK para atualizar o estado de notificação para que essa alteração de estado seja sincronizada em todos os dispositivos usados pelo mesmo usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```C#
notification.UserActionState = UserNotificationUserActionState.Activated;
await notification.SaveAsync();
```

### <a name="delete-a-notification"></a><span data-ttu-id="e81f9-223">Excluir uma notificação</span><span class="sxs-lookup"><span data-stu-id="e81f9-223">Delete a notification</span></span>

<span data-ttu-id="e81f9-224">Se a exclusão de uma notificação é iniciada da instância do cliente de aplicativo (por exemplo, se a tarefa correspondente a essa notificação for marcada como concluída e removida do banco de dados do aplicativo), o aplicativo deve chamar o SDK para excluir a notificação para que essa operação de exclusão seja sincronizada em todos os dispositivos usados pelo mesmo usuário.</span><span class="sxs-lookup"><span data-stu-id="e81f9-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="e81f9-225">Uma notificação é removida do repositório de notificação do usuário apenas se expirada ou explicitamente excluída.</span><span class="sxs-lookup"><span data-stu-id="e81f9-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="e81f9-226">Uma notificação do usuário não é excluída quando você atualiza o **UserActionState** para Descartado, porque a definição semântica do **UserActionState** é definida pelo próprio aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e81f9-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```C#
await channel.DeleteUserNotificationAsync(notification.Id);
```

## <a name="see-also"></a><span data-ttu-id="e81f9-227">Confira também</span><span class="sxs-lookup"><span data-stu-id="e81f9-227">See also</span></span>

- <span data-ttu-id="e81f9-228">
  [Referência da API](https://docs.microsoft.com/pt-BR/windows/project-rome/notifications/api-reference-for-windows/) para o conjunto completo de APIs relacionadas aos recursos de notificação no SDK.</span><span class="sxs-lookup"><span data-stu-id="e81f9-228">[API reference](https://docs.microsoft.com/en-us/windows/project-rome/notifications/api-reference-for-windows/) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="e81f9-229">[Exemplo do lado do cliente](https://github.com/Microsoft/project-rome/tree/master/Windows/samples/GraphNotificationsSample) para aplicativos UWP do Windows.</span><span class="sxs-lookup"><span data-stu-id="e81f9-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Windows/samples/GraphNotificationsSample) for Windows UWP apps.</span></span>
- <span data-ttu-id="e81f9-230">[Exemplo do servidor do aplicativo](notifications-integrating-app-server.md) para publicar as notificações.</span><span class="sxs-lookup"><span data-stu-id="e81f9-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
