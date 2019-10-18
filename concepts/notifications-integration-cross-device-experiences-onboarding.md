---
title: 'Integração de experiências entre dispositivos para as notificações do Microsoft Graph '
description: 'Registre seu aplicativo no Centro de Desenvolvimento do Windows para habilitar os clientes de aplicativo para receber notificações entre dispositivos enviadas pelo Microsoft Graph.  '
localization_priority: Priority
ms.prod: notifications"
ms.openlocfilehash: 789273f812c9f9a38748e47480f7141b51d6f465
ms.sourcegitcommit: 70ebcc469e2fdf2c31aeb6c5169f0101c3e698b0
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/15/2019
ms.locfileid: "34063248"
---
# <a name="onboarding-to-cross-device-experiences-for-microsoft-graph-notifications"></a>Integração de experiências entre dispositivos para as notificações do Microsoft Graph

Além do [registro do aplicativo no Portal do Azure](notifications-integration-app-registration.md), seu aplicativo deve registrar informações entre dispositivos como, por exemplo, a ID do aplicativo entre dispositivos e as credenciais de push multiplataforma para autorizar o Microsoft Graph a enviar notificações por serviços nativos de notificações por push, que correspondem a cada sistema operacional: Windows, iOS e Android. Isso é feito por meio do [ painel do Partner Center (antigo painel do Centro de Desenvolvimento do Windows)](https://partner.microsoft.com/dashboard/). 

> [!NOTE]
> Se ainda não tiver uma conta de desenvolvedor do Windows, será preciso criar uma. Para saber mais, confira [Abrir uma conta de desenvolvedor](https://docs.microsoft.com/en-us/windows/uwp/publish/opening-a-developer-account). É necessário fazer isso mesmo se não planeja criar um aplicativo UWP do Windows. Se estiver desenvolvendo um aplicativo corporativo ou de estudante como parte de uma empresa, você pode associar sua conta de desenvolvedor com uma conta apropriada do Azure AD usada para gerenciar envios de sua empresa.  Para saber mais, confira [associar o Azure Active Directory com sua conta do Partner Center](https://docs.microsoft.com/en-us/windows/uwp/publish/associate-azure-ad-with-partner-center).

Para começar, entre no [painel do Partner Center](https://partner.microsoft.com/en-us/dashboard) com sua conta de desenvolvedor do Windows (não pode usar uma conta do Azure AD):

1.  No menu à esquerda, acesse **Experiências entre Dispositivos**, selecione **Configurar um novo aplicativo entre dispositivos**, e forneça o nome do aplicativo, conforme mostrado na captura de tela a seguir.

![Configure um novo registro do aplicativo entre dispositivos](images/notifications-crossdevice-new-configure.png)

2.  Selecione todas as plataformas compatíveis em que seu aplicativo estará disponível e habilitado para receber notificações. Você pode selecionar plataformas compatíveis que incluem o Windows, Android e iOS, conforme mostrado. 

![Configure tipos de plataforma compatível](images/notifications-crossdevice-supported-platforms.png)

3.  Forneça IDs de aplicativo para cada uma das plataformas em seu aplicativo estará disponível, conforme mostrado.

 ![Forneça as IDs de aplicativos específicos da plataforma](images/notifications-crossdevice-platform-appids.png)

> [!NOTE] 
> Você pode adicionar outras IDs (até dez) por plataforma – isso ocorre se você tiver várias versões do mesmo aplicativo, ou até mesmo diferentes aplicativos, e deseja receber a mesma notificação enviada pelo servidor do aplicativo e direcionadas ao mesmo usuário.

4.  Forneça ou selecione a ID de aplicativo na conta da Microsoft e/ou registro do aplicativo do Azure AD. Essa ID do cliente corresponde à conta da Microsoft ou registro do aplicativo do Azure AD obtido ao registrar no Portal do Azure.

![Forneça as IDs de cliente do registro do aplicativo Azure para MSA e AAD](images/notifications-crossdevice-azureportal-clientid.png)

5.  As notificações do Microsoft Graph usam cada plataforma nativa de notificação em todas as plataformas principais para enviar notificações aos pontos de extremidade do aplicativo do cliente, ou seja, WNS (para Windows UWP), FCM (para Android) e APNS (para iOS). Forneça as credenciais dessas plataformas de notificação para habilitar as notificações do Microsoft Graph para enviar notificações para o servidor do aplicativo ao publicar notificações direcionadas pelo usuário, conforme mostrado.

 ![Forneça credenciais de push entre dispositivos](images/notifications-crossdevice-push-cred.png)

> [!NOTE]
> Para aplicativos UWP do Windows, habilitar as notificações por push WNS é um pré-requisito para usar as notificações do Microsoft Graph. Para saber mais, confira a [Visão geral do WNS](https://docs.microsoft.com/en-us/windows/uwp/design/shell/tiles-and-notifications/windows-push-notification-services--wns--overview). Após fazer a integração, você pode fornecer credenciais de push pelo Partner Center para a plataforma do dispositivo conectado.

6.  Verifique o domínio do aplicativo entre dispositivos, que serve como um processo de verificação para provar que o aplicativo tem a propriedade desse domínio. Isso funciona como uma identidade do aplicativo entre dispositivos para o aplicativo ou os aplicativos que você registrou, conforme mostrado.
    
    ![Verificar domínio](images/notifications-crossdevice-domain-verify.png)

Isso é tudo! Você já registrou os aplicativos para receber notificações. Em seguida, adicione as [notificações SDK do Microsoft Graph](https://github.com/microsoft/project-rome) ao seu projeto na plataforma escolhida e comece a integração. 
