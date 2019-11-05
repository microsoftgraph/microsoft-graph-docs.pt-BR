---
title: Integração do aplicativo Android no SDK do lado do cliente para notificações ao usuário
description: Integre o aplicativo Android com notificações de usuário no SDK do cliente.
localization_priority: Priority
ms.prod: Microsoft Graph notifications
ms.openlocfilehash: 69edda814508d69e47f8d70bd81df9425621aa0a
ms.sourcegitcommit: b1e1f614299f668453916bd85761ef7b6c8d6eff
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/05/2019
ms.locfileid: "37969535"
---
# <a name="integrate-your-android-app-with-the-client-side-sdk-for-user-notifications"></a><span data-ttu-id="96e71-103">Integração do aplicativo Android no SDK do lado do cliente para notificações ao usuário</span><span class="sxs-lookup"><span data-stu-id="96e71-103">Integrate your Android app with the client-side SDK for user notifications</span></span>

<span data-ttu-id="96e71-104">Após [registrar seu aplicativo](notifications-integration-app-registration.md) no Portal do Azure e integrar suas [experiências entre dispositivos](notifications-integration-cross-device-experiences-onboarding.md) no Partner Center de desenvolvimento, a próxima etapa é integrar seu aplicativo de cliente com o SDK do lado do cliente para aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="96e71-104">After you [register your app](notifications-integration-app-registration.md) in the Azure Portal and onboard your [cross-device experiences](notifications-integration-cross-device-experiences-onboarding.md) in the Partner Dev Center, the next step is to integrate your client app with the client-side SDK forAndroid apps.</span></span>  

<span data-ttu-id="96e71-105">Com o SDK do cliente, o aplicativo pode executar as etapas necessárias de registro para receber notificações publicadas do servidor do aplicativo direcionadas ao usuário conectado atualmente.</span><span class="sxs-lookup"><span data-stu-id="96e71-105">With the client-side SDK, your app can perform the necessary registration steps to start receiving notifications published from your app server targeted at the user who is currently signed in.</span></span> <span data-ttu-id="96e71-106">O SDK então gerencia as notificações no lado do cliente, incluindo receber novas notificações, gerenciar o estado de notificações para alcançar cenários como descartar de forma universal e recuperar o histórico completo de notificações.</span><span class="sxs-lookup"><span data-stu-id="96e71-106">The SDK then manages the notifications on the client side, including receiving new incoming notifications, managing the state of notifications to achieve scenarios like universal dismiss, and retrieving full notification history.</span></span> 

## <a name="new-incoming-notification-flow"></a><span data-ttu-id="96e71-107">Fluxo de notificação de entrada</span><span class="sxs-lookup"><span data-stu-id="96e71-107">New incoming notification flow</span></span>

<span data-ttu-id="96e71-108">Para receber novas notificações, o fluxo de dados é mostrado no diagrama a seguir.</span><span class="sxs-lookup"><span data-stu-id="96e71-108">For receiving new incoming notifications, the data flow is shown in the following diagram.</span></span>

![Fluxo de nova notificação para aplicativo Android](images/notifications-new-notification-android.png)

<span data-ttu-id="96e71-110">O processo envolve alguns componentes:</span><span class="sxs-lookup"><span data-stu-id="96e71-110">he process involves a few components:</span></span>

* <span data-ttu-id="96e71-111">Servidor de aplicativo – back-end do aplicativo</span><span class="sxs-lookup"><span data-stu-id="96e71-111">App server - The back end of your application</span></span>
* <span data-ttu-id="96e71-112">Cliente do aplicativo – front-end do aplicativo (um aplicativo UWP, Android ou iOS)</span><span class="sxs-lookup"><span data-stu-id="96e71-112">App client - The front end of your application (a UWP app, an Android app, or an iOS app)</span></span>
* <span data-ttu-id="96e71-113">Notificações do Microsoft Graph – o componente do serviço que permite que notificações ao usuário sejam publicadas, armazenadas e sincronizadas em instâncias diferentes dos clientes do aplicativo em vários dispositivos e plataformas</span><span class="sxs-lookup"><span data-stu-id="96e71-113">Microsoft Graph notifications - The service component that enables user notifications to be published, stored, and synced across different instances of app clients across devices and platforms</span></span>
* <span data-ttu-id="96e71-114">FCM – Firebase Cloud Messaging, o serviço de notificações por push fornecido pelo Android como parte do Google Play Services.</span><span class="sxs-lookup"><span data-stu-id="96e71-114">FCM - Firebase Cloud Messaging, the push notification service provided by Android as a part of Google Play Services.</span></span> <span data-ttu-id="96e71-115">As notificações do Microsoft Graph usam esse serviço para sinalizar clientes do aplicativo do Android sobre as alterações de dados de notificação do usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-115">Microsoft Graph notifications use this service to signal the Android app clients about user notification data changes.</span></span>  

<span data-ttu-id="96e71-116">O diagrama mostra as próximas etapas:</span><span class="sxs-lookup"><span data-stu-id="96e71-116">The diagram shows the following steps:</span></span> 

1. <span data-ttu-id="96e71-117">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96e71-117">Application logic.</span></span> <span data-ttu-id="96e71-118">Essa etapa captura o que aciona a notificação para ser publicada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-118">This step captures what triggers the notification to be published to the user.</span></span> <span data-ttu-id="96e71-119">Isso é lógica específica do aplicativo e pode ser uma atualização de dados ou evento sobre algo diferente do Microsoft Graph, como um novo evento do calendário ou atribuição de tarefas, ou o que o serviço de aplicativo quer notificar o usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-119">This is app-specific logic, and can be an event or data update about something else in Microsoft Graph, such as a new calendar event or task assignment, or else your app service wants to notify the user about.</span></span>
2. <span data-ttu-id="96e71-120">O servidor do aplicativo publica uma notificação para o usuário alvo pela API de notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96e71-120">The app server publishes a notification to the targeted user via the Microsoft Graph notifications API.</span></span> <span data-ttu-id="96e71-121">Para saber mais, consulte [integração com o lado do servidor](notifications-integrating-app-server.md).</span><span class="sxs-lookup"><span data-stu-id="96e71-121">For more details, see [server side integration](notifications-integrating-app-server.md).</span></span>
3. <span data-ttu-id="96e71-122">Ao receber a solicitação Web com nova notificação, as notificações do Microsoft Graph mantêm o conteúdo da notificação em segurança na nuvem para esse aplicativo e esse usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-122">On receiving the web request containing the new notification, Microsoft Graph notifications persists the content of the notification securely in the cloud for this app and this user.</span></span>
4. <span data-ttu-id="96e71-123">Para cada instância do cliente do aplicativo inscrita para receber notificações para esse usuário, as notificações do Microsoft Graph envia um sinal para notificar cliente do aplicativo, por meio do serviço de envio por push nativo fornecido pelo sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="96e71-123">For each app client instance subscribing to receive notifications for this user, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="96e71-124">Nesse caso, o aplicativo é um aplicativo Android, e ele usa [mensagens de dados FCM](https://firebase.google.com/docs/cloud-messaging/concept-options) para enviar o sinal.</span><span class="sxs-lookup"><span data-stu-id="96e71-124">In this case, the application is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
5. <span data-ttu-id="96e71-125">Depois que o aplicativo for sinalizado pelas notificações por push de entrada, ele pede ao SDK para buscar as alterações no repositório de notificações do usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-125">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
6. <span data-ttu-id="96e71-126">O SDK estabelece uma conexão segura e compatível com o repositório de notificações do usuário no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96e71-126">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
7. <span data-ttu-id="96e71-127">O SDK recebe as alterações de dados – nesse caso, o novo conteúdo de notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-127">The SDK gets the data changes - in this case, the new notification contents.</span></span> 
8. <span data-ttu-id="96e71-128">O SDK dispara retornos de evento para notificá-o aplicativo após as alterações são recuperadas com êxito.</span><span class="sxs-lookup"><span data-stu-id="96e71-128">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
9. <span data-ttu-id="96e71-129">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96e71-129">Application logic.</span></span> <span data-ttu-id="96e71-130">Essa etapa captura o que o aplicativo escolhe fazer dentro retorno de chamada do evento.</span><span class="sxs-lookup"><span data-stu-id="96e71-130">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="96e71-131">Normalmente, isso resulta em alterações locais de dados do aplicativo e atualizações de interface do usuário locais.</span><span class="sxs-lookup"><span data-stu-id="96e71-131">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="96e71-132">Nesse caso, o aplicativo geralmente cria uma pop-up de notificação do sistema para notificar o usuário sobre o conteúdo de notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-132">In this case,  the app usually constructs a toast notification popup to notify the user about the notification contents.</span></span>

## <a name="notification-update-flow"></a><span data-ttu-id="96e71-133">Fluxo de atualização de notificação</span><span class="sxs-lookup"><span data-stu-id="96e71-133">Notification update flow</span></span>

<span data-ttu-id="96e71-134">Uma das principais vantagens de usar as notificações do Microsoft Graph é que ele mantêm as notificações na nuvem com segurança e as transforma em um tipo de recurso com estado.</span><span class="sxs-lookup"><span data-stu-id="96e71-134">One of the main benefits for using Microsoft Graph notifications is that it persists notifications in the cloud securely and turns them into a stateful resource type.</span></span> <span data-ttu-id="96e71-135">Portanto, ele pode ajudar o aplicativo a gerenciar e a sincronizar o estado correto das notificações em diferentes dispositivos para o usuário conectado em um cenário entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="96e71-135">Therefore, it can help your application to manage and sync the correct state of the notifications across different devices for the same signed in user in a cross-device scenario.</span></span> <span data-ttu-id="96e71-136">Quando uma notificação estiver marcada como descartada ou como lida em um dispositivo, os outros dispositivos podem ser notificados em tempo real.</span><span class="sxs-lookup"><span data-stu-id="96e71-136">When a notification is marked as dismissed, or marked as read on one device, the other devices can be notified in real-time.</span></span> <span data-ttu-id="96e71-137">"Manipulada uma vez, descartada em qualquer lugar" pode se tornar a promessa real como parte da experiência de notificação para seus usuários.</span><span class="sxs-lookup"><span data-stu-id="96e71-137">"Handled once, dismissed everywhere" can become a true promise as part of the notification experience for your users.</span></span> 

<span data-ttu-id="96e71-138">O diagrama a seguir mostra o fluxo de dados para alterar o estado de uma notificação ou excluir a notificação em um dispositivo e receber/manipular a alteração de estado ou a exclusão em outro dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96e71-138">The following diagram shows the data flow for changing the state of a notification or deleting the notification on one device, and receiving/handling the state change or the deletion on another device.</span></span>

![Atualização de fluxo de notificação para aplicativo Android](images/notifications-notification-update-android.png)

<span data-ttu-id="96e71-140">Observe que a segunda parte do fluxo é semelhante ao fluxo de tratamento de novas notificações de entrada.</span><span class="sxs-lookup"><span data-stu-id="96e71-140">Notice that the second part of the flow is similar to the flow for handling new incoming notifications.</span></span> <span data-ttu-id="96e71-141">Isso é esperado – o padrão de programação no SDK  foi projetado para que o cliente do aplicativo possa lidar com todos os tipos de alterações de dados de notificações do usuário (novas notificações de entrada, alterações de estado de notificação, notificação excluída) de maneira semelhante.</span><span class="sxs-lookup"><span data-stu-id="96e71-141">This is by design - the  programming pattern of the SDK is designed so that the application client can handle all types of user notification data changes (new incoming notifications, notification state changes, notification deleted) in a similar way.</span></span>  

<span data-ttu-id="96e71-142">O diagrama mostra as próximas etapas:</span><span class="sxs-lookup"><span data-stu-id="96e71-142">The diagram shows the following steps:</span></span>

1. <span data-ttu-id="96e71-143">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96e71-143">Application logic.</span></span> <span data-ttu-id="96e71-144">Algo aciona a notificação para ser alterada ou excluída.</span><span class="sxs-lookup"><span data-stu-id="96e71-144">Something triggers the notification to be changed or deleted.</span></span> <span data-ttu-id="96e71-145">Em geral, qualquer evento possível pode acionar a alteração de uma notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-145">In general, any event can trigger a notification to change.</span></span> 
2. <span data-ttu-id="96e71-146">Chamada do aplicativo para o SDK do cliente para atualizar ou excluir uma notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-146">App calling into the client SDK to update or delete a notification.</span></span> <span data-ttu-id="96e71-147">Atualmente, expomos duas propriedades sobre alterações de estado – **userActionState** e **readState** – mas o aplicativo pode definir esses estados e quando eles precisam ser atualizados.</span><span class="sxs-lookup"><span data-stu-id="96e71-147">Currently, we expose two properties regarding state changes - **userActionState** and **readState** - but your application can define these states and when they need to be updated.</span></span> <span data-ttu-id="96e71-148">Por exemplo, quando um usuário descartar a notificação pop-up, você pode atualizar o **userActionState** para Descartado.</span><span class="sxs-lookup"><span data-stu-id="96e71-148">For example, when a user dismisses the notification popup, you can update the **userActionState** to be Dismissed.</span></span> <span data-ttu-id="96e71-149">Quando um usuário clica na notificação pop-up e inicia o aplicativo para consumir o conteúdo correspondente do aplicativo, você pode atualizar o **userActionState** para ativado e atualizar o **readState** para Lido.</span><span class="sxs-lookup"><span data-stu-id="96e71-149">When a user clicks the notification popup and launches the app to consume corresponding app content, you can update the **userActionState** to be Activated and update the **readState** to be Read.</span></span> 
3. <span data-ttu-id="96e71-150">Depois que a API correspondente é chamada para atualizar ou excluir uma notificação, o SDK irá chamar o repositório na nuvem de notificação de usuário para dispersar essa alteração para as outras instâncias de cliente do aplicativo com o mesmo usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="96e71-150">After the corresponding API is called to update or delete a notification, the SDK will call into the user notification store in the cloud in order to fan-out this change to the other app client instances with the same signed in user.</span></span> 
4. <span data-ttu-id="96e71-151">Ao receber a solicitação de atualização/exclusão de um cliente, as notificações do Microsoft Graph irão atualizar o repositório de notificação e identificar as outras instâncias de cliente do aplicativo inscritas para essa alteração.</span><span class="sxs-lookup"><span data-stu-id="96e71-151">On receiving the update/delete request from a client, Microsoft Graph notifications will update the notification store, and identify the other app client instances that subscribed to this change.</span></span>
5. <span data-ttu-id="96e71-152">Para cada inscrição do cliente do aplicativo, as notificações do Microsoft Graph envia um sinal para notificar o cliente do aplicativo, por meio do serviço de envio por push nativo fornecido pelo sistema operacional.</span><span class="sxs-lookup"><span data-stu-id="96e71-152">For each app client subscription, Microsoft Graph notifications sends a signal to notify the app client, via the native push service provided by the operating system.</span></span> <span data-ttu-id="96e71-153">Nesse caso, esse é um aplicativo Android, e ele usa [mensagens de dados FCM](https://firebase.google.com/docs/cloud-messaging/concept-options) para enviar o sinal.</span><span class="sxs-lookup"><span data-stu-id="96e71-153">In this case, this is an Android app, and it uses [FCM data message](https://firebase.google.com/docs/cloud-messaging/concept-options) to send the signal.</span></span> 
6. <span data-ttu-id="96e71-154">Depois que o aplicativo for sinalizado pelas notificações por push de entrada, ele pede ao SDK para buscar as alterações no repositório de notificações do usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-154">After the application is signaled by the incoming push notification, it asks the SDK to fetch for the changes in the user notification store.</span></span> 
7. <span data-ttu-id="96e71-155">O SDK estabelece uma conexão segura e compatível com o repositório de notificações do usuário no Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96e71-155">The SDK establishes a secure and compliant connection with the user notifications store in Microsoft Graph.</span></span>
8. <span data-ttu-id="96e71-156">O SDK recebe as alterações de dados – nesse caso, as alterações são atualizações de notificação de estado ou exclusões de notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-156">The SDK gets the data changes - in this case, the changes are notification state updates or notification deletions.</span></span> 
9. <span data-ttu-id="96e71-157">O SDK dispara retornos de evento para notificá-o aplicativo após as alterações são recuperadas com êxito.</span><span class="sxs-lookup"><span data-stu-id="96e71-157">The SDK fires event callbacks to notify the app after the changes are successfully retrieved.</span></span> 
10. <span data-ttu-id="96e71-158">Lógica do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96e71-158">Application logic.</span></span> <span data-ttu-id="96e71-159">Essa etapa captura o que o aplicativo escolhe fazer dentro retorno de chamada do evento.</span><span class="sxs-lookup"><span data-stu-id="96e71-159">This step captures what your app chooses to do inside the event callback.</span></span> <span data-ttu-id="96e71-160">Normalmente, isso resulta em alterações locais de dados do aplicativo e atualizações de interface do usuário locais.</span><span class="sxs-lookup"><span data-stu-id="96e71-160">Usually, this results in local app data changes and local UI updates.</span></span> <span data-ttu-id="96e71-161">Nesse caso, como há atualizações de notificação, o aplicativo deve atualizar a interface do usuário no local para refletir a alteração de estado.</span><span class="sxs-lookup"><span data-stu-id="96e71-161">In this case, because there are notification updates, the app should update the UI locally to reflect the state change.</span></span> <span data-ttu-id="96e71-162">Por exemplo, se uma notificação estiver marcada como ativada, você pode remover a mensagem de notificação correspondente dentro da bandeja de notificação do Android para obter "manipulada uma vez, descartada em todo lugar".</span><span class="sxs-lookup"><span data-stu-id="96e71-162">For example, if a notification is marked as activated, you can remove the corresponding notification message inside Android's notification tray to achieve "handled once, dismissed everywhere".</span></span> 

<span data-ttu-id="96e71-163">Para obter mais informações sobre as notificações do Microsoft Graph, consulte a [visão geral das notificações do Microsoft Graph](notifications-concept-overview.md).</span><span class="sxs-lookup"><span data-stu-id="96e71-163">For more information about Microsoft Graph notifications, see [Microsoft Graph Notifications overview](notifications-concept-overview.md).</span></span> <span data-ttu-id="96e71-164">Para saber mais sobre as etapas necessárias para integrar com as notificações do Microsoft Graph de ponta a ponta, confira a [visão geral de integração](notifications-integration-e2e-overview.md) das notificações do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="96e71-164">For more information about the steps required to integrate with Microsoft Graph notifications from end to end, see Microsoft Graph notifications [integration overview](notifications-integration-e2e-overview.md).</span></span>

## <a name="development-environment-and-requirements"></a><span data-ttu-id="96e71-165">Ambiente e os requisitos de desenvolvimento</span><span class="sxs-lookup"><span data-stu-id="96e71-165">Development environment and requirements</span></span>

<span data-ttu-id="96e71-166">Para usar as notificações do Microsoft Graph, será necessário um IDE de desenvolvimento de aplicativos Android e um dispositivo Android com uma das arquiteturas suportadas (**armeabi-v7a**, **arm64-v8a**, **x86**, ou **x86_64**) ou um emulador.</span><span class="sxs-lookup"><span data-stu-id="96e71-166">To use Microsoft Graph notifications, you will need an Android app development IDE and an Android device with one of the supported architectures (**armeabi-v7a**, **arm64-v8a**, **x86**, or **x86_64**) or an emulator.</span></span> <span data-ttu-id="96e71-167">O sistema deve ser o Android 4.4.2 ou posterior.</span><span class="sxs-lookup"><span data-stu-id="96e71-167">The system must be running Android 4.4.2 or later.</span></span>

## <a name="adding-the-sdk-to-your-project"></a><span data-ttu-id="96e71-168">Adicionar o SDK ao seu projeto</span><span class="sxs-lookup"><span data-stu-id="96e71-168">Adding the SDK to your project</span></span>

<span data-ttu-id="96e71-169">Insira as seguintes referências do repositório para o arquivo *build.gradle* na raiz do seu projeto.</span><span class="sxs-lookup"><span data-stu-id="96e71-169">Insert the following repository references into the *build.gradle* file at the root of your project.</span></span>

```Java
allprojects {
    repositories {
    jcenter()
    maven { url 'https://maven.google.com' }
    maven { url 'https://projectrome.bintray.com/maven/' }
    }
}
```

<span data-ttu-id="96e71-170">Depois insira a dependência a seguir para o arquivo _build.gradle_ que está na pasta do projeto.</span><span class="sxs-lookup"><span data-stu-id="96e71-170">Then, insert the following dependency into the _build.gradle_ file that is in your project folder.</span></span>

```Java
dependencies { 
    ...
    implementation 'com.microsoft.connecteddevices:connecteddevices-sdk:+'
}
```

<span data-ttu-id="96e71-171">Se você quiser usar ProGuard em seu aplicativo, adicione as regras ProGuard dessas novas APIs.</span><span class="sxs-lookup"><span data-stu-id="96e71-171">If you want to use ProGuard in your app, add the ProGuard Rules for these new APIs.</span></span> <span data-ttu-id="96e71-172">Crie um arquivo chamado *proguard-rules.txt* na pasta *Aplicativo* do seu projeto e cole nos conteúdos de [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt).</span><span class="sxs-lookup"><span data-stu-id="96e71-172">Create a file called *proguard-rules.txt* in the *App* folder of your project, and paste in the contents of [ProGuard_Rules_for_Android_Rome_SDK.txt](https://github.com/Microsoft/project-rome/blob/master/Android/ProGuard_Rules_for_Android_Rome_SDK.txt).</span></span>
<span data-ttu-id="96e71-173">No arquivo do projeto *AndroidManifest.xml*, adicione as seguintes permissões dentro do elemento `manifest` (se já não estiverem presentes).</span><span class="sxs-lookup"><span data-stu-id="96e71-173">In your project's *AndroidManifest.xml* file, add the following permissions inside the `manifest` element (if they are not already present).</span></span> <span data-ttu-id="96e71-174">Isso dá permissão ao aplicativo para se conectar à Internet e permitem a descoberta Bluetooth em seu dispositivo.</span><span class="sxs-lookup"><span data-stu-id="96e71-174">This gives your app permission to connect to the Internet and to enable Bluetooth discovery on your device.</span></span>
<span data-ttu-id="96e71-175">Observe que as permissões relacionadas ao Bluetooth só são necessárias para usar a descoberta Bluetooth; elas não são necessárias para os recursos da plataformas de dispositivos conectados.</span><span class="sxs-lookup"><span data-stu-id="96e71-175">Note that the Bluetooth-related permissions are only necessary for using Bluetooth discovery; they are not needed for the other features in the Connected Devices Platform.</span></span> <span data-ttu-id="96e71-176">Além disso, `ACCESS_COARSE_LOCATION` só é necessário em SDKs 21 do Android e versões posteriores.</span><span class="sxs-lookup"><span data-stu-id="96e71-176">Additionally, `ACCESS_COARSE_LOCATION` is only required on Android SDKs 21 and later.</span></span> <span data-ttu-id="96e71-177">Em SDKs 23 do Android e versões posteriores, você também deve solicitar ao usuário para conceder acesso à localização no tempo de execução.</span><span class="sxs-lookup"><span data-stu-id="96e71-177">On Android SDKs 23 and later, you must also prompt the user to grant location access at runtime.</span></span>

```xml
<uses-permission android:name="android.permission.INTERNET" />
<uses-permission android:name="android.permission.BLUETOOTH" />
<uses-permission android:name="android.permission.BLUETOOTH_ADMIN" />
<uses-permission android:name="android.permission.ACCESS_COARSE_LOCATION" />
<uses-permission android:name="android.permission.ACCESS_NETWORK_STATE" />
```
<span data-ttu-id="96e71-178">Em seguida, acesse as classes de atividade onde desejar que a funcionalidade dos Dispositivos Conectados seja localizada.</span><span class="sxs-lookup"><span data-stu-id="96e71-178">Next, go to the activity classes where you would like the Connected Devices functionality to be located.</span></span> <span data-ttu-id="96e71-179">Importar os namespaces a seguir.</span><span class="sxs-lookup"><span data-stu-id="96e71-179">Import the following namespaces.</span></span>

```java
import com.microsoft.connecteddevices;
import com.microsoft.connecteddevices.userdata;
import com.microsoft.connecteddevices.userdata.usernotifications;
```

## <a name="initializing-the-connected-device-platforms"></a><span data-ttu-id="96e71-180">Inicializar as Plataformas do Dispositivo Conectado</span><span class="sxs-lookup"><span data-stu-id="96e71-180">Initializing the Connected Device Platforms</span></span>

<span data-ttu-id="96e71-181">No SDK do lado do cliente é desenvolvido com base em uma infraestrutura chamada Plataforma de Dispositivo Conectado.</span><span class="sxs-lookup"><span data-stu-id="96e71-181">The client-side SDK is built on top of an infrastructure called Connected Device Platform.</span></span> <span data-ttu-id="96e71-182">Antes de poder usar qualquer recurso, a plataforma deve ser inicializada em seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96e71-182">Before any feature can be used, the platform must be initialized within your app.</span></span> <span data-ttu-id="96e71-183">As etapas de inicialização que devem ocorrer em sua classe principal no método **OnCreate**, porque eles são necessários para ocorrer os cenários de notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-183">The initialization steps should occur in your main class **OnCreate** method, because they are required before the notification scenarios can take place.</span></span>

<span data-ttu-id="96e71-184">Você deve criar e inicializar a plataforma ao instanciar a classe [**ConnectedDevicesPlatform**](https://docs.microsoft.com/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest).</span><span class="sxs-lookup"><span data-stu-id="96e71-184">You must construct and initialize the platform by instantiating the [**ConnectedDevicesPlatform**](https://docs.microsoft.com/java/api/com.microsoft.connecteddevices.connecteddevicesplatform?view=rome-android-latest) class.</span></span> <span data-ttu-id="96e71-185">Antes de fazer isso, certifique-se de conectar manipuladores de eventos, pois depois que a plataforma é iniciada, os eventos podem começar a acionar.</span><span class="sxs-lookup"><span data-stu-id="96e71-185">Before doing that, make sure to hook up event handlers, because after the platform is started, the events might begin to fire.</span></span> 

```java
ConnectedDevicesPlatform platform = new ConnectedDevicesPlatform(context);

platform.getAccountManager().accessTokenRequested().subscribe((accountManager, args) -> onAccessTokenRequested(accountManager, args));
platform.getAccountManager().accessTokenInvalidated().subscribe((accountManager, args) -> onAccessTokenInvalidated(accountManager, args));
platform.getNotificationRegistrationManager().notificationRegistrationStateChanged().subscribe((notificationRegistrationManager, args) -> onNotificationRegistrationStateChanged(notificationRegistrationManager, args));

platform.start();
```

### <a name="handling-account-access-token"></a><span data-ttu-id="96e71-186">Gerenciar tokens de acesso à conta</span><span class="sxs-lookup"><span data-stu-id="96e71-186">Handling account access token</span></span>

<span data-ttu-id="96e71-187">Todas as chamadas de Web que o SDK realiza, incluindo a recuperação do conteúdo de uma nova notificação de entrada, atualização de notificação de estado e muito mais, são leituras de ou escrevendo para os dados do usuário e, portanto, sempre exigem um token de acesso válido.</span><span class="sxs-lookup"><span data-stu-id="96e71-187">All the web calls the SDK makes, including retrieving the content of a new incoming notification, updating notification states, and more, are reading from or writing to the user's data, and therefore always require a valid access token.</span></span> <span data-ttu-id="96e71-188">O SDK requer que você trate os seguintes eventos – chamados quando um token de acesso for solicitado ou invalidado – para garantir que, depois da plataforma inicializar, o token de acesso do usuário seja tratado corretamente.</span><span class="sxs-lookup"><span data-stu-id="96e71-188">The SDK requires you to handle the following events - invoked when an access token is requested or invalidated - to make sure that after the platform is initialized, your access token for the user is handled correctly.</span></span> 

#### <a name="accesstokenrequested"></a><span data-ttu-id="96e71-189">accessTokenRequested</span><span class="sxs-lookup"><span data-stu-id="96e71-189">accessTokenRequested</span></span> 

<span data-ttu-id="96e71-190">Para uma implementação completa, confira o [exemplo de aplicativo Android](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span><span class="sxs-lookup"><span data-stu-id="96e71-190">For a full implementation, see the [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenRequested(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenRequestedEventArgs args) {
    ConnectedDevicesAccessTokenRequest request = args.getRequest();
    List<String> scopes = request.getScopes();

    // We always need to complete the request, even if a matching account is not found
    if (account == null) {
        request.completeWithErrorMessage("The app could not find a matching ConnectedDevicesAccount to get a token");
        return;
    }

    // Complete the request with a token
    account.getAccessTokenAsync(scopes)
        .thenAcceptAsync((String token) -> {
            request.completeWithAccessToken(token);
        }).exceptionally(throwable -> {
            request.completeWithErrorMessage("The Account could not return a token with those scopes");
            return null;
    });
}
```

#### <a name="accesstokeninvalidated"></a><span data-ttu-id="96e71-191">accessTokenInvalidated</span><span class="sxs-lookup"><span data-stu-id="96e71-191">accessTokenInvalidated</span></span>

<span data-ttu-id="96e71-192">Para uma implementação completa, confira o [exemplo de aplicativo Android](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span><span class="sxs-lookup"><span data-stu-id="96e71-192">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

```Java
private void onAccessTokenInvalidated(ConnectedDevicesAccountManager sender, ConnectedDevicesAccessTokenInvalidatedEventArgs args, List<Account> accounts) {
    Log.i(TAG, "Token invalidated for account: " + args.getAccount().getId());
}

```

### <a name="handling-push-registration-expiration"></a><span data-ttu-id="96e71-193">Gerenciar validade de registro de push</span><span class="sxs-lookup"><span data-stu-id="96e71-193">Handling push registration expiration</span></span> 

<span data-ttu-id="96e71-194">As notificações do Microsoft Graph usa o WNS, a plataforma de push nativa no Android, para sinalizar o aplicativo de cliente sobre alterações de dados de notificações do usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-194">Microsoft Graph notifications uses FCM, the native push platform on Android, to signal the client application on user notifications data changes.</span></span> <span data-ttu-id="96e71-195">Isso acontece quando novas notificações recebidas forem publicadas do servidor de aplicativos, ou quando o estado de qualquer notificação é atualizado em outro dispositivo com o mesmo usuário conectado em um cenário entre dispositivos.</span><span class="sxs-lookup"><span data-stu-id="96e71-195">This happens when new incoming notifications are published from your app server, or when any notification's state is updated on a different device with the same signed in user in a cross-device scenario.</span></span> 

<span data-ttu-id="96e71-196">Portanto, é necessário um token FCM válido que permite mensagens de notificação de dados para ter êxito.</span><span class="sxs-lookup"><span data-stu-id="96e71-196">Therefore, a valid FCM token that allows data notification messages to come through successfully is required.</span></span> <span data-ttu-id="96e71-197">O seguinte retorno de chamada de evento trata da validade de tokens FCM por push.</span><span class="sxs-lookup"><span data-stu-id="96e71-197">The following event callback handles FCM push token expirations.</span></span> 

#### <a name="notificationregistrationstatechanged"></a><span data-ttu-id="96e71-198">notificationRegistrationStateChanged</span><span class="sxs-lookup"><span data-stu-id="96e71-198">notificationRegistrationStateChanged</span></span>

<span data-ttu-id="96e71-199">Para uma implementação completa, confira o [exemplo de aplicativo Android](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span><span class="sxs-lookup"><span data-stu-id="96e71-199">For a full implementation, see the  [Android sample app](https://github.com/Microsoft/project-rome/blob/release/1.3.0/Android/samples/graphnotificationssample/app/src/main/java/com/microsoft/connecteddevices/graphnotifications/ConnectedDevicesManager.java).</span></span> 

## <a name="signing-in-your-user"></a><span data-ttu-id="96e71-200">Entrar com seu usuário</span><span class="sxs-lookup"><span data-stu-id="96e71-200">Signing in your user</span></span>

<span data-ttu-id="96e71-201">As notificações do Microsoft Graph, como vários outros tipos de recursos no Microsoft Graph, são centralizadas em torno dos usuários.</span><span class="sxs-lookup"><span data-stu-id="96e71-201">Microsoft Graph notifications, like many other resource types in Microsoft Graph, are centralized around users.</span></span> <span data-ttu-id="96e71-202">Para que o aplicativo assine e comece a receber notificações para o usuário conectado, primeiro é necessário obter um token OAuth válido a ser usado no processo de registro.</span><span class="sxs-lookup"><span data-stu-id="96e71-202">In order for your app to subscribe to and start receiving notifications for the signed in user, you first need to obtain a valid OAuth token to be used in the registration process.</span></span> <span data-ttu-id="96e71-203">Você pode usar o método que preferir para gerar e gerenciamento os tokens OAuth.</span><span class="sxs-lookup"><span data-stu-id="96e71-203">You can use your preferred method of generating and managing the OAuth tokens.</span></span> <span data-ttu-id="96e71-204">Exemplo de aplicativo que usa ADAL.</span><span class="sxs-lookup"><span data-stu-id="96e71-204">The sample app used ADAL.</span></span> 

<span data-ttu-id="96e71-205">Se você estiver usando uma conta da Microsoft, será necessário incluir as seguintes permissões em uma solicitação de entrada: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, e `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span><span class="sxs-lookup"><span data-stu-id="96e71-205">If you're using a Microsoft account, you will need to include the following permissions in your sign-in request: `wl.offline_access"`, `ccs.ReadWrite`, `wns.connect`, `asimovrome.telemetry`, and `https://activity.windows.com/UserActivity.ReadWrite.CreatedByApp`.</span></span> 

<span data-ttu-id="96e71-206">Se você estiver usando uma conta do Azure AD, você precisará solicitar o seguinte público: `https://cdpcs.access.microsoft.com`.</span><span class="sxs-lookup"><span data-stu-id="96e71-206">If you're using an Azure AD account, you'll need to request the following audience: `https://cdpcs.access.microsoft.com`.</span></span>

## <a name="adding-the-user-account-to-the-platform"></a><span data-ttu-id="96e71-207">Adicionar a conta de usuário à plataforma</span><span class="sxs-lookup"><span data-stu-id="96e71-207">Adding the user account to the platform</span></span> 

<span data-ttu-id="96e71-208">Será preciso registrar a conta do usuário conectado com um SDK, o que envolve a adição de contas e o registro de um canal push para receber as notificações por push iniciais através de FCM.</span><span class="sxs-lookup"><span data-stu-id="96e71-208">You need to register the signed in user account with the SDK, which involves adding the account and registering a push channel in order to receive the initial push notifications through FCM.</span></span> 

```Java
public AsyncOperation<Boolean> prepareAccountAsync(final Context context) {
    // Accounts can be in 3 different scenarios:
    // 1: cached account in good standing (initialized in the SDK and our token cache).
    // 2: account missing from the SDK but present in our cache: Add and initialize account.
    // 3: account missing from our cache but present in the SDK. Log the account out async

    // Subcomponents (e.g. UserDataFeed) can only be initialized when an account is in both the app cache
    // and the SDK cache.
    // For scenario 1, initialize our subcomponents.
    // For scenario 2, subcomponents will be initialized after InitializeAccountAsync registers the account with the SDK.
    // For scenario 3, InitializeAccountAsync will unregister the account and subcomponents will never be initialized.
    switch (mState) {
        // Scenario 1
        case IN_APP_CACHE_AND_SDK_CACHE:
            mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
            return registerAccountWithSdkAsync();
        // Scenario 2
        case IN_APP_CACHE_ONLY: {
            // Add the this account to the ConnectedDevicesPlatform.AccountManager
            return mPlatform.getAccountManager().addAccountAsync(mAccount).thenComposeAsync((ConnectedDevicesAddAccountResult result) -> {
                // We failed to add the account, so exit with a failure to prepare bool
                if (result.getStatus() != ConnectedDevicesAccountAddedStatus.SUCCESS) {
                    result.getStatus());
                    return AsyncOperation.completedFuture(false);
                }

                // Set the registration state of this account as in both app and sdk cache
                mState = AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE;
                mUserNotificationsManager = new UserNotificationsManager(context, mAccount, mPlatform);
                return registerAccountWithSdkAsync();
            });
        }
        // Scenario 3
        case IN_SDK_CACHE_ONLY:
            // Remove the account from the SDK since the app has no knowledge of it
            mPlatform.getAccountManager().removeAccountAsync(mAccount);
            // This account could not be prepared
            return AsyncOperation.completedFuture(false);
        default:
            // This account could not be prepared
            Log.e(TAG, "Failed to prepare account " + mAccount.getId() + " due to unknown state!");
            return AsyncOperation.completedFuture(false);
    }
}
```

```Java
public AsyncOperation<Boolean> registerAccountWithSdkAsync() {
    if (mState != AccountRegistrationState.IN_APP_CACHE_AND_SDK_CACHE) {
        AsyncOperation<Boolean> toReturn = new AsyncOperation<>();
        toReturn.completeExceptionally(new IllegalStateException("Cannot register this account due to bad state: " + mAccount.getId()));
        return toReturn;
    }

    // Grab the shared GCM/FCM notification token from this app's BroadcastReceiver
    return RomeNotificationReceiver.getNotificationRegistrationAsync().thenComposeAsync((ConnectedDevicesNotificationRegistration notificationRegistration) -> {
        // Perform the registration using the NotificationRegistration
        return mPlatform.getNotificationRegistrationManager().registerAsync(mAccount, notificationRegistration)
            .thenComposeAsync((result) -> {
                if (result.getStatus() == ConnectedDevicesNotificationRegistrationStatus.SUCCESS) {
                    Log.i(TAG, "Successfully registered account " + mAccount.getId() + " for cloud notifications");
                } else {
                    // It would be a good idea for apps to take a look at the different statuses here and perhaps attempt some sort of remediation.
                    // For example, token request failed could mean that the user needs to sign in again. An app could prompt the user for this action 
                    // and retry the operation afterwards.
                    Log.e(TAG, "Failed to register account " + mAccount.getId() + " for cloud notifications!");
                    return AsyncOperation.completedFuture(false);
                }

                return mUserNotificationsManager.registerForAccountAsync();
            });
    });
}
```

## <a name="subscribing-to-receive-users-notifications"></a><span data-ttu-id="96e71-209">Inscrever-se para receber notificações do usuário</span><span class="sxs-lookup"><span data-stu-id="96e71-209">Subscribing to receive user's notifications</span></span> 

<span data-ttu-id="96e71-210">Você precisa instanciar um objeto **UserDataFeed** para o aplicativo para este usuário conectado.</span><span class="sxs-lookup"><span data-stu-id="96e71-210">You need to instantiate a **UserDataFeed** object for your application for this logged in user.</span></span> <span data-ttu-id="96e71-211">O aplicativo é identificado pela ID de aplicativo multiplataforma fornecidas durante a [integração de experiências entre dispositivos](notifications-integration-cross-device-experiences-onboarding.md).</span><span class="sxs-lookup"><span data-stu-id="96e71-211">Your application is identified by the cross-platform app ID you provided during the [Cross-Device Experiences onboarding](notifications-integration-cross-device-experiences-onboarding.md).</span></span>

```Java
public UserNotificationsManager(@NonNull Context context, @NonNull ConnectedDevicesAccount account, @NonNull ConnectedDevicesPlatform platform)
{
    Context context = new Context;
    UserDataFeed feed = UserDataFeed.getForAccount(account, platform, Secrets.APP_HOST_NAME);
    UserNotificationChannel channel = new UserNotificationChannel(feed);
    UserNotificationReader reader = channel.createReader();
    reader.dataChanged().subscribe((reader, aVoid) -> readFromCache(reader));
    }
}
```

## <a name="receiving-and-managing-user-notifications"></a><span data-ttu-id="96e71-212">Receber e gerenciar as notificações do usuário</span><span class="sxs-lookup"><span data-stu-id="96e71-212">Receiving and managing user notifications</span></span>

<span data-ttu-id="96e71-213">O diagrama de fluxo já apresentado nesse tópico mostra que os padrões de programação para lidar com novas notificações de entrada de um servidor do aplicativo e uma atualização de notificação ou exclusão iniciado de outra instância do aplicativo do cliente são semelhantes.</span><span class="sxs-lookup"><span data-stu-id="96e71-213">The flow diagram earlier in this topic shows that the programming patterns to handle a new incoming notifications from an app server and a notification update or deletion initiated from another app client instance are similar.</span></span> <span data-ttu-id="96e71-214">A seguir estão as etapas para lidar com essas alterações de dados.</span><span class="sxs-lookup"><span data-stu-id="96e71-214">The following are the steps for handling these data changes.</span></span> 

### <a name="handling-incoming-push-notification-signal"></a><span data-ttu-id="96e71-215">Gerenciar sinal de notificações por push de entrada</span><span class="sxs-lookup"><span data-stu-id="96e71-215">Handling incoming push notification signal</span></span>

<span data-ttu-id="96e71-216">Todos os tipos de alterações de dados de notificações do usuário geram um sinal que é entregue para os clientes do aplicativo como uma notificação por push.</span><span class="sxs-lookup"><span data-stu-id="96e71-216">All types of user notification data changes generate a signal that gets delivered to the app clients as a push notification.</span></span> <span data-ttu-id="96e71-217">Para aplicativos Android, o sinal será enviado como uma mensagem de dados FCM por push.</span><span class="sxs-lookup"><span data-stu-id="96e71-217">For Android apps, the signal is delivered as a FCM push data message.</span></span> <span data-ttu-id="96e71-218">Ao receber sinal de mensagem de dados, o aplicativo deve chamar **TryParse** para acionar o SDK para buscar no serviço de notificações do Microsoft Graph para as alterações de dados reais.</span><span class="sxs-lookup"><span data-stu-id="96e71-218">On receiving the data message signal, the app should call **TryParse** to trigger the SDK to fetch from the Microsoft Graph notifications service for the actual data changes.</span></span>

```Java
public void onMessageReceived(RemoteMessage message) {
    Map data = message.getData();
    ConnectedDevicesNotification notification = ConnectedDevicesNotification.tryParse(data);

    if (notification != null) {
        try {
            ConnectedDevicesPlatform platform = ConnectedDevicesManager.getConnectedDevicesManager(getApplicationContext()).getPlatform();

            // NOTE: it may be useful to attach completion to this async in order to know when the notification is done being processed.
            // This would be a good time to stop a background service or otherwise cleanup.
            platform.processNotificationAsync(notification);
        } catch (Exception e) {
            Log.e(TAG, "Failed to process FCM notification" + e.getMessage());
        }
    }
}
```

### <a name="handling-user-notification-data-changes"></a><span data-ttu-id="96e71-219">Gerenciar alterações de dados de notificação do usuário</span><span class="sxs-lookup"><span data-stu-id="96e71-219">Handling user notification data changes</span></span>

<span data-ttu-id="96e71-220">Após o SDK buscar com êxito as alterações de dados, um retorno de chamada do evento é invocado e o cliente de aplicativo deve lidar com a criação, atualização ou exclusão da notificação.</span><span class="sxs-lookup"><span data-stu-id="96e71-220">After the SDK successfully completes fetching the data changes, an event callback is invoked and the app client is expected to handle notification creation, update, or deletion.</span></span>

```Java
private void readFromCache(final UserNotificationReader reader)
{
    reader.readBatchAsync(Long.MAX_VALUE).thenAccept(notifications -> {
        synchronized (this) {
            for (final UserNotification notification : notifications) {
                if (notification.getStatus() == UserNotificationStatus.ACTIVE) {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));

                    if (notification.getUserActionState() == UserNotificationUserActionState.NO_INTERACTION) {
                        mNewNotifications.add(notification);
                        if (notification.getReadState() != UserNotificationReadState.READ) {
                            clearNotification(mContext.getApplicationContext(), notification.getId());
                            addNotification(mContext.getApplicationContext(), notification.getContent(), notification.getId());
                        }
                    } else {
                        clearNotification(mContext.getApplicationContext(), notification.getId());
                    }

                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    mHistoricalNotifications.add(0, notification);
                } else {
                    removeIf(mNewNotifications, item -> notification.getId().equals(item.getId()));
                    removeIf(mHistoricalNotifications, item -> notification.getId().equals(item.getId()));
                    clearNotification(mContext.getApplicationContext(), notification.getId());
                }
            }
        }

    });
}
```

### <a name="update-state-of-a-notification"></a><span data-ttu-id="96e71-221">Atualização do estado de uma notificação</span><span class="sxs-lookup"><span data-stu-id="96e71-221">Update state of a notification</span></span>

<span data-ttu-id="96e71-222">Se a alteração do estado de notificação é iniciada da instância do cliente do aplicativo (por exemplo, se a notificação pop-up do sistema nesse dispositivo é ativada pelo usuário), o aplicativo deve chamar o SDK para atualizar o estado de notificação para que essa alteração de estado seja sincronizada em todos os dispositivos usados pelo mesmo usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-222">If a notification state change is initiated from this app client instance (for example, if the toast notification popup on this device is activated by the user), the app needs to call the SDK to update the notification's state in order to have this state change synced across all devices used by the same user.</span></span> 

```Java
notification.setUserActionState(UserNotificationUserActionState.ACTIVATED);
notification.saveAsync().whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully activated the notification");
    }
});

```

### <a name="delete-a-notification"></a><span data-ttu-id="96e71-223">Excluir uma notificação</span><span class="sxs-lookup"><span data-stu-id="96e71-223">Delete a notification</span></span>

<span data-ttu-id="96e71-224">Se a exclusão de uma notificação é iniciada da instância do cliente de aplicativo (por exemplo, se a tarefa correspondente a essa notificação for marcada como concluída e removida do banco de dados do aplicativo), o aplicativo deve chamar o SDK para excluir a notificação para que essa operação de exclusão seja sincronizada em todos os dispositivos usados pelo mesmo usuário.</span><span class="sxs-lookup"><span data-stu-id="96e71-224">If a notification deletion is initiated from this app client instance (for example, if the task corresponding to this notification is marked as complete and is removed from your app's database), the app needs to call the SDK to delete the notification in order to have this delete operation synced across all devices used by the same user.</span></span> 

<span data-ttu-id="96e71-225">Uma notificação é removida do repositório de notificação do usuário apenas se expirada ou explicitamente excluída.</span><span class="sxs-lookup"><span data-stu-id="96e71-225">A notification is removed from the user notification store only if it is expired or explicitly deleted.</span></span> <span data-ttu-id="96e71-226">Uma notificação do usuário não é excluída quando você atualiza o **UserActionState** para Descartado, porque a definição semântica do **UserActionState** é definida pelo próprio aplicativo.</span><span class="sxs-lookup"><span data-stu-id="96e71-226">A user notification is not deleted when you update the **UserActionState** to be Dismissed, because the semantic definition of **UserActionState** is defined by the application itself.</span></span>

```Java
channel.deleteUserNotificationAsync(notification.getId()).whenCompleteAsync((userNotificationUpdateResult, throwable) -> {
    if (throwable == null && userNotificationUpdateResult != null && userNotificationUpdateResult.getSucceeded()) {
        Log.d(TAG, "Successfully deleted the notification");
    }
});
```

## <a name="see-also"></a><span data-ttu-id="96e71-227">Confira também</span><span class="sxs-lookup"><span data-stu-id="96e71-227">See also</span></span>

- <span data-ttu-id="96e71-228">[Referência da API](https://docs.microsoft.com/windows/project-rome/notifications/api-reference-for-android) para o conjunto completo de APIs relacionadas aos recursos de notificação no SDK.</span><span class="sxs-lookup"><span data-stu-id="96e71-228">[API reference](https://docs.microsoft.com/windows/project-rome/notifications/api-reference-for-android) for the full set of APIs related to notification features in the SDK.</span></span> 
- <span data-ttu-id="96e71-229">[Exemplo do lado do cliente](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample) para aplicativos Android.</span><span class="sxs-lookup"><span data-stu-id="96e71-229">[Client-side sample](https://github.com/Microsoft/project-rome/tree/master/Android/samples/graphnotificationssample) for Android apps.</span></span>
- <span data-ttu-id="96e71-230">[Exemplo do servidor do aplicativo](notifications-integrating-app-server.md) para publicar as notificações.</span><span class="sxs-lookup"><span data-stu-id="96e71-230">[App server sample](notifications-integrating-app-server.md) for publishing notifications.</span></span> 
