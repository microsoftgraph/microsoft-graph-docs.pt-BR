---
title: 'Criar aplicativos para diversos dispositivos com a tecnologia do Project Rome '
description: 'Você pode usar o Project Rome para criar experiências que abrangem vários dispositivos e plataformas sem complicações, reduzindo conflitos para usuários e ajudando a promover o engajamento com o aplicativo. Para que aplicativos compartilhem dados entre vários dispositivos e plataformas usando as APIs do Project Rome, é necessário configurar um aplicativo para diversos dispositivos que inclua informações sobre os aplicativos específicos de plataforma. '
ms.localizationpriority: medium
ms.prod: project-rome
ms.openlocfilehash: 8d1d58ec2da980efeab46423fd945a5afd2994fa
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139223"
---
# <a name="build-cross-device-apps-powered-by-project-rome"></a>Criar aplicativos para diversos dispositivos com a tecnologia do Project Rome 

Você pode usar o Project Rome para criar experiências que abrangem vários dispositivos e plataformas sem complicações, reduzindo conflitos para usuários e ajudando a promover o engajamento com o aplicativo. Para que aplicativos compartilhem dados entre vários dispositivos e plataformas usando as APIs do Project Rome, é necessário configurar um aplicativo para diversos dispositivos que inclua informações sobre os aplicativos específicos de plataforma. 

Um aplicativo para vários dispositivos permite que você: 

- Use a API do feed de atividades do Project Rome no Microsoft Graph.  
- Leia e grave atividades de usuários publicadas por um grupo de aplicativos específicos de plataforma usando o SDK do Project Rome para Windows, Android e/ou iOS.
-  Tenha aplicativos como destino usando os recursos de retransmissão de dispositivos do Project Rome com o SDK do Project Rome para Android ou iOS.

**Retome de onde parou em diferentes dispositivos com a API do feed de atividades**

Você pode configurar um aplicativo para vários dispositivos para Windows, iOS, Android e Web para que o aplicativo em cada plataforma possa ler e gravar as atividades do usuário publicadas por qualquer aplicativo do grupo. 

Por exemplo, uma usuária está terminando um comunicado à imprensa em seu computador no trabalho antes de jantar com os amigos. No restaurante, ela recebe uma notificação do seu chefe sobre um erro de digitação que precisa ser corrigido imediatamente. Ela abre o aplicativo em seu telefone Android e vê um cartão mostrando o comunicado à imprensa que ela estava editando mais cedo. Ela toca no cartão para abri-lo e corrigir o comunicado imediatamente e voltar para os amigos. 
 
Com essa configuração de aplicativo entre dispositivos estabelecida, o feed de atividades do usuário é sincronizado entre dispositivos e plataformas com facilidade para que você possa criar experiências que ajudam os usuários a retomar tarefas importantes de onde pararam em qualquer superfície de aplicativo. 

**Escolha tela certa na hora certa com a API de retransmissão de dispositivo**

Você pode configurar um aplicativo entre dispositivos com credenciais de notificação por push para cada uma das plataformas em que seu aplicativo está disponível, de forma que um comando ou uma notificação possa ser enviada para você em qualquer dispositivo em que usar o aplicativo, independentemente da plataforma. 

Por exemplo, uma usuária está assistindo a um vídeo enquanto vai de ônibus do trabalho pra casa. Quando ela chega em casa, toca no aplicativo para iniciar o vídeo no Xbox One para continuar assistindo na tela grande. 

Quando você associa credenciais de notificações por push a cada uma das plataformas em que seu aplicativo está disponível com o aplicativo entre dispositivos, o aplicativo do usuário pode enviar comandos para outros dispositivos e criar experiências entre várias telas ou fazer a transição de um fluxo de trabalho de um dispositivo para outro em tempo real. 

## <a name="select-the-right-hosting-method-for-your-cross-device-app-configuration"></a>Selecione o método certo de hospedagem da configuração de aplicativo entre dispositivos
Você pode hospedar a configuração de aplicativo entre dispositivos como um arquivo JSON no seu domínio ou um perfil configurável pelo [Centro de Desenvolvimento do Windows](https://developer.microsoft.com/windows). Escolha uma opção de hospedagem de acordo com os recursos do Project Rome que você deseja habilitar nos aplicativos. 

### <a name="windows-dev-center-profile-recommended"></a>Perfil do Centro de Desenvolvimento do Windows (recomendado) 
Você pode acessar todos os recursos de Rome Project usando um aplicativo entre dispositivos gerenciado no [Centro de Desenvolvimento do Windows](https://developer.microsoft.com/windows). O Centro de Desenvolvimento do Windows também oferece a *melhor* maneira de gerenciar alterações de configuração do aplicativo entre dispositivos. Você pode salvar atualizações em um perfil existente de forma mais segura antes de estar pronto para publicar as alterações de produção. Quando você publica alterações em um aplicativo entre dispositivos existente no Centro de Desenvolvimento, o novo perfil entrará em vigor após aproximadamente **uma hora**.  

### <a name="externally-hosted-json-file-limited"></a>Arquivo JSON hospedado externamente (limitado) 
Você pode usar os seguintes recursos do Project Rome em todas as plataformas compatíveis usando um aplicativo entre dispositivos gerenciado como um arquivo JSON hospedado externamente:  

* Ler e gravar as atividades de usuário de todas as plataformas usando a [API do feed de atividades](/graph/api/resources/activity-feed-api-overview?view=graph-rest-1.0)
* Gravar atividades de usuário de todas as plataformas (Windows, iOS, Android, Web) usando SDKs do Project Rome.

Se você **apenas** acessar esses recursos, é possível hospedar a configuração de aplicativo entre dispositivos externamente em seu domínio como um arquivo JSON.

## <a name="configure-a-cross-device-app-using-the-windows-dev-center"></a>Configurar um aplicativo entre dispositivos usando o Centro de Desenvolvimento do Windows
Uma ID de aplicativo entre dispositivos é representada como um nome de domínio de sua propriedade. O domínio aponta para um mapeamento das IDs de aplicativo específicas da plataforma armazenadas como um arquivo JSON hospedado em seu domínio ou configuráveis pelo Centro de Desenvolvimento do Windows. Depois de identificar o domínio que você vai usar para representar a sua ID de aplicativo entre dispositivos, você precisará coletar informações para configurar o perfil associado. 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id-and-enable-domain-verification"></a>Etapa 1: Selecione um domínio seguro para sua ID de aplicativo entre dispositivos e habilitar a verificação de domínio
O domínio usado como sua ID de aplicativo entre dispositivos deve ser um domínio de nível superior ou um subdomínio e deve ser protegida via TLS. Por exemplo: https://contoso.com ou https://myapp.contoso.com, mas NÃO https://myapp.contoso.com/somepath. **Você deve ter um domínio exclusivo (ou subdomínio) por aplicativo entre dispositivos.** No entanto, você decide que aplicativos serão associados a um único aplicativo entre dispositivos de acordo com o comportamento multiplataforma ao qual deseja oferecer suporte. 

Por exemplo, um desenvolvedor de aplicativos com um pacote de aplicativos de jogos pode usar um subdomínio separado para cada um para garantir que cada aplicativo esteja inscrito apenas nas atividades do usuário que pode retomar ao ler dados em vários dispositivos e plataformas. Por outro lado, um desenvolvedor de aplicativos com um pacote de aplicativos de produtividade projetados para funcionar juntos pode usar um domínio único para todos eles para que qualquer aplicativo possa iniciar um membro do pacote entre dispositivos.  

#### <a name="assert-domain-ownership-with-the-windows-dev-center"></a>Reafirmar a propriedade do domínio com o Centro de Desenvolvimento do Windows
Ao usar o Centro de Desenvolvimento do Windows para gerenciar a configuração do aplicativo entre dispositivos, o domínio que representa a ID de aplicativo entre dispositivos é armazenado como parte do perfil de aplicativo entre dispositivos para a Microsoft pode verificar se você é o proprietário do domínio. A propriedade do domínio **deve ser verificada** para concluir a publicação da configuração do aplicativo entre dispositivos, portanto, é uma boa ideia resolver isso primeiro. Se seu domínio ainda não tiver sido verificado, você poderá salvar os detalhes do aplicativo entre dispositivos e executar novamente a verificação depois de concluir esta etapa para publicar seu aplicativo entre dispositivos.

Para reafirmar a propriedade do domínio do aplicativo entre dispositivos, será preciso adicionar uma entrada [DNS TXT](https://go.microsoft.com/fwlink/?linkid=871417) do seu domínio com um valor exclusivo fornecido no Centro de Desenvolvimento. Esse valor é exclusivo por aplicativo entre dispositivos. Para localizar o valor exclusivo do aplicativo, entre no Centro de Desenvolvimento do Windows e escolha **Experiências entre dispositivos** no menu à esquerda para começar a configurar um novo aplicativo entre dispositivos. Depois que você dá um nome para o novo aplicativo entre dispositivos, selecione **Verificar seu domínio de aplicativo entre dispositivos** no submenu. Esta página exibirá instruções com um valor exclusivo em **linha** (por exemplo, MS=95ff4557-813f-45a5-b2f6-1f94170b979f). Certifique-se de copiar o valor inteiro incluindo "MS =".

### <a name="step-2-collect-your-platform-specific-application-ids"></a>Etapa 2: Coletar as IDs de aplicativo específicas da plataforma
Coletar as IDs de aplicativos específicas da plataforma para cada aplicativo e a plataforma usará [APIs do Project Rome](/graph/api/resources/project-rome-overview?view=graph-rest-1.0).

Você precisará coletar cada uma das IDs de aplicativo específicas da plataforma para associá-las à sua identidade de aplicativo entre dispositivos. Com o Centro de Desenvolvimento do Windows, você poderá selecionar aplicativos na Plataforma Universal do Windows associados à sua conta de desenvolvedor, mas será preciso fornecer IDs de aplicativo manualmente para qualquer um dos aplicativos Android, iOS ou win32 e identificar a URL principal de qualquer aplicativo Web associado. Você pode associar até 10 IDs por plataforma. 

Para encontrar as IDs:

* **windows_universal** – forneça uma AUMID para cada aplicativo UWP. Para saber mais, veja [Encontrar a ID de modelo de usuário do aplicativo de um aplicativo instalado (Industry 8.1)](/previous-versions/windows/embedded/dn449300(v=winembedded.82)) e [Aplicativo](/uwp/schemas/appxpackage/appxmanifestschema/element-application).
* **windows_win32** – forneça um AUMID para cada aplicativo. Nos aplicativos win32, você precisará usar um script para recuperar essas informações. Para saber mais, veja [Encontrar a ID de modelo de usuário do aplicativo de um aplicativo instalado (Industry 8.1)](/previous-versions/windows/embedded/dn449300(v=winembedded.82)).
* **android** – para saber mais, veja [Alterar o nome do pacote](https://developer.android.com/studio/build/application-id.html#change_the_package_name). 
* **ios** – para saber mais, veja [Pacote](https://developer.apple.com/documentation/foundation/bundle) e [Propriedades obrigatórias, localizáveis e editáveis](https://help.apple.com/itunes-connect/developer/#/devfc3066644).
* **msa** – entre no [portal de registro do Aplicativo](https://apps.dev.microsoft.com). Você pode exibir a ID de aplicativo/ID de cliente para qualquer um de seus aplicativos. O Live SDK (valores hexadecimais) e os Identificadores de aplicativos convergentes (GUIDs) têm suporte.   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>Etapa 3: Configurar suporte para a conta Microsoft ou o Azure AD
Para habilitar experiências entre dispositivos, os usuários do aplicativo devem entrar com uma conta [da Microsoft](https://account.microsoft.com/account) ou uma conta [Azure Active Directory](/azure/active-directory/develop/active-directory-developers-guide) (Azure AD). Você fornecerá IDs do cliente/aplicativo para oferecer suporte à autenticação como parte de sua configuração de aplicativo entre dispositivos para permitir o suporte entre plataformas. É possível fornecer até 10 instâncias.

Você pode localizar as IDs de aplicativo/cliente existentes ou provisionar novas entrando no [portal de registro do aplicativo](https://apps.dev.microsoft.com) com sua conta de desenvolvedor. Quando você entra no portal, é possível exibir a ID do cliente/aplicativo de qualquer um dos aplicativos. O Live SDK (valores hexadecimais) e os identificadores de aplicativos convergentes (GUIDs) têm suporte.   

Se você estiver criando um aplicativo que dará suporte a usuários do Azure AD e não usar um identificador de aplicativo convergente emitido pelo [Portal de registro de aplicativo](https://apps.dev.microsoft.com), será preciso fornecer o GUID para a ID de aplicativo do seu aplicativo do Azure. Para localizar o GUID de seu locatário: 

1. Entre no [Portal do Azure](https://portal.azure.com). 
2. Selecione **Azure Active Directory**.
3. Em **Gerenciar**, selecione **Registros de aplicativo**. 
4. Selecione o aplicativo na lista e exiba a ID do aplicativo (GUID) listada em **Essentials**.

### <a name="step-4-configure-support-for-cross-platform-push-notifications-optional"></a>Etapa 4: Configurar o suporte para notificações de push multiplataforma (opcional) 
Se você tiver optado por configurar o aplicativo entre dispositivos no Centro de Desenvolvimento do Windows, será possível habilitar o suporte para notificações por push multiplataforma fornecendo as credenciais que você usa com as APIs para as plataformas de mensagens por push do iOS e do Android. Elas serão necessárias se você estiver usando os SDKs do Project Rome para iOS e Android e quiser publicar mais do que atividades do usuário. Se você estiver usando as APIs do Project Rome somente no Microsoft Graph, não será necessário executar esta etapa. Você pode associar até 10 conjuntos de credenciais por plataforma. 

>**Importante:** não armazene credenciais de notificações por push em um arquivo JSON hospedado externamente.

Para encontrar as IDs:

* 
  **Serviço de Notificação do Windows** – veja [Registrar seu aplicativo e receber as credenciais para o serviço de nuvem](/previous-versions/windows/apps/hh913756(v=win.10)#registering-your-app-and-receiving-the-credentials-for-your-cloud-service) e o [Portal de registro do aplicativo](https://apps.dev.microsoft.com).
* **Apple Push Notification Service** – confira [Visão geral de APNs](https://developer.apple.com/library/content/documentation/NetworkingInternet/Conceptual/RemoteNotificationsPG/APNSOverview.html).
* **Google Cloud Messaging** – veja [Mensagens em nuvem Firebase](https://firebase.google.com/docs/cloud-messaging/).

**Observação:** se você estiver usando o Firebase para as notificações por push em dispositivos iOS com credenciais do Android, será necessário fornecer suas credenciais de APNs como parte da configuração do aplicativo entre dispositivos. 

## <a name="configure-a-cross-device-app-using-an-externally-hosted-json-file"></a>Configurar um aplicativo entre dispositivos usando um arquivo JSON hospedado externamente
Uma ID de aplicativo entre dispositivos é representada como um nome de domínio de sua propriedade. O domínio aponta para um mapeamento das IDs de aplicativo específicas da plataforma armazenadas como um arquivo JSON hospedado em seu domínio ou configuráveis pelo Centro de Desenvolvimento do Windows. Depois de identificar o domínio que você vai usar para representar a sua ID de aplicativo entre dispositivos, você precisará coletar informações para configurar o perfil associado. 

### <a name="step-1-select-a-secure-domain-for-your-cross-device-app-id"></a>Etapa 1: Selecionar um domínio seguro para sua ID de aplicativo entre dispositivos
Uma ID de aplicativo entre dispositivos é representada como um nome de domínio de sua propriedade. Deve ser um domínio de nível superior ou um subdomínio e deve ser protegido via TLS. Por exemplo: https://contoso.com ou https://myapp.contoso.com, mas NÃO https://myapp.contoso.com/somepath. Você deve ter um domínio exclusivo (ou subdomínio) por aplicativo entre dispositivos. No entanto, você decide que aplicativos serão associados a um único aplicativo entre dispositivos de acordo com o comportamento multiplataforma ao qual deseja oferecer suporte. 

Por exemplo, um desenvolvedor de aplicativos com um pacote de aplicativos de jogos pode usar um subdomínio separado em cada um para garantir que cada aplicativo esteja inscrito apenas nas atividades do usuário que pode retomar ao ler dados em vários dispositivos e plataformas. Um desenvolvedor de aplicativos com um pacote de aplicativos de produtividade projetados para funcionar juntos pode usar um domínio único para todos eles para que qualquer aplicativo possa iniciar um membro do pacote entre dispositivos.  

#### <a name="assert-domain-ownership-with-an-externally-hosted-json-file"></a>Reafirme a propriedade do domínio com um arquivo JSON hospedado externamente 
Se estiver usando um arquivo JSON hospedado externamente para gerenciar seu aplicativo entre dispositivos, você reafirma a propriedade do domínio incluindo suas IDs de aplicativo Azure AD ou conta da Microsoft no arquivo cross-platform-app-identifiers. A propriedade do domínio será verificada como parte do processo de publicação ao usar a API do feed de atividades para criar as atividades do usuário.

O sistema armazenará em cache o conteúdo do arquivo JSON para evitar gerar solicitações frequentes em seu domínio. Se configurado, o serviço respeitará os cabeçalhos de cache HTTP ao avaliar quando o cache deverá ser atualizado. Se não estiver configurado, o serviço será atualizado a cada 24 horas. 

### <a name="step-2-collect-your-platform-specific-application-ids-and-construct-your-json-file"></a>Etapa 2: Coletar as IDs de aplicativo específicas da plataforma e criar o arquivo JSON
Coletar as IDs de aplicativos específicas da plataforma para cada aplicativo e a plataforma que usará o feed de atividades e/ou a API de retransmissão do dispositivo. 

Você precisará coletar cada uma das IDs de aplicativo específicas da plataforma para associá-las à sua identidade de aplicativo entre dispositivos. Com um arquivo JSON hospedado externamente, você precisará coletar IDs de aplicativo para cada um dos aplicativos específicos da plataforma para serem configuradas como parte do aplicativo entre dispositivos e agrupá-las no formato especificado. Você pode associar até 10 IDs por plataforma. 

#### <a name="constructing-your-cross-platform-app-identifiers-file"></a>Criar o arquivo cross-platform-app-identifiers
O arquivo JSON em si deve ser chamado de **cross-platform-app-identifiers** e hospedado no raiz do domínio HTTPS. O conteúdo do arquivo é uma matriz JSON de mapeamentos entre as plataformas compatíveis de seu aplicativo e as IDs do aplicativo nesta plataforma. Quando criar o arquivo, inclua um objeto JSON para cada aplicativo e plataforma que usarão APIs do Project Rome. 
 
O arquivo permitirá diversos objetos JSON com o mesmo identificador de plataforma. Por exemplo, um aplicativo para iPhone e um aplicativo para iPad devem ser listados como objetos JSON separados, cada um com um valor de plataforma do iOS. O identificador de plataforma Web é mostrado no exemplo a seguir.
 
Não é necessário incluir um objeto JSON para todas as plataformas. Inclua apenas objetos JSON nas plataformas nas quais seu aplicativo esteja usando APIs do Project Rome. Por exemplo, se você não tiver um cliente de aplicativo na plataforma Android, não será necessária uma entrada de arquivo para Android.
 
O exemplo a seguir inclui todos os identificadores de plataforma válidos aceitos atualmente. Objetos JSON com um valor de plataforma inválido serão removidos.  

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

Para encontrar as IDs:

* **windows_universal** – forneça uma AUMID para cada aplicativo UWP. Para saber mais, veja [Encontrar a ID de modelo de usuário do aplicativo de um aplicativo instalado (Industry 8.1)](/previous-versions/windows/embedded/dn449300(v=winembedded.82)) e [Aplicativo](/uwp/schemas/appxpackage/appxmanifestschema/element-application).
* **windows_win32** – forneça um AUMID para cada aplicativo. Nos aplicativos win32, você precisará usar um script para recuperar essas informações. Para saber mais, veja [Encontrar a ID de modelo de usuário do aplicativo de um aplicativo instalado (Industry 8.1)](/previous-versions/windows/embedded/dn449300(v=winembedded.82)).
* **android** – para saber mais, veja [Alterar o nome do pacote](https://developer.android.com/studio/build/application-id.html#change_the_package_name). 
* **ios** – para saber mais, veja [Pacote](https://developer.apple.com/documentation/foundation/bundle) e [Propriedades obrigatórias, localizáveis e editáveis](https://help.apple.com/itunes-connect/developer/#/devfc3066644).
* **msa** – entre no [portal de registro do Aplicativo](https://apps.dev.microsoft.com). Você pode exibir a ID de aplicativo/ID de cliente para qualquer um de seus aplicativos. O Live SDK (valores hexadecimais) e os Identificadores de aplicativos convergentes (GUIDs) têm suporte.   

### <a name="step-3-configure-support-for-microsoft-account-or-azure-ad"></a>Etapa 3: Configurar suporte para a conta Microsoft ou o Azure AD
Para habilitar experiências entre dispositivos, seus usuários do aplicativo devem entrar com uma conta Microsoft ou uma conta do Azure AD. Você fornecerá IDs do cliente/aplicativo para oferecer suporte à autenticação como parte de sua configuração de aplicativo entre dispositivos para permitir o suporte entre plataformas. É possível fornecer até 10 instâncias.

```[
{"platform":"windows_universal", "application":"Microsoft.Contoso_8wekyb3d8bbwe"},
{"platform":"windows_win32", "application":"DefaultBrowser_NOPUBLISHERID!Microsoft.Contoso.Default"},
{"platform":"android","application":"com.example.myapp"},
{"platform":"ios", "application":"com.example.myapp"},
{"platform":"web", "application":"https://contoso.com"},
{"platform":"web", "application":"https://chat.contoso.com"},
{"platform":"msa", "application":"00000000603E0BF"},
{"platform":"msa", "application":"48932b46-98b1-4020-9be4-cc7a65643c9e"},
]
```

Você pode encontrar suas IDs de aplicativo/IDs de cliente existentes ou provisionar novas ao entrar no [Portal](https://apps.dev.microsoft.com) de Registro de Aplicativos com sua conta de desenvolvedor. Quando você entra, é possível exibir a ID do cliente/aplicativo de qualquer um dos aplicativos. O Live SDK (valores hexadecimais) e os identificadores de aplicativos convergentes (GUIDs) têm suporte. Use o tipo de plataforma "msa" ao adicionar as IDs usadas para habilitar o suporte em uma conta da Microsoft ou Azure AD, como mostrado no exemplo anterior.  

>**Observação:** Se você estiver criando um aplicativo que dê suporte a usuários do Azure AD e não usar uma ID de aplicativo convergente emitida por meio do [Portal](https://apps.dev.microsoft.com)de Registro de Aplicativos, será necessário fornecer o GUID para a ID do aplicativo do seu aplicativo do Azure. Esse tipo de ID também deve ser configurada como tipo de plataforma "msa". 

Para localizar o GUID no Portal do Azure para o seu locatário: 

1. Entre no [Portal do Azure](https://portal.azure.com).
2. Selecione **Azure Active Directory**. 
3. Em **Gerenciar**, selecione **Registros de aplicativo**.
4. Selecione o aplicativo na lista. Você pode exibir sua ID de aplicativo (GUID) em **Essentials**.

#### <a name="encoding-the-cross-platform-app-identifiers-file"></a>Codificar o arquivo cross-platform-app-identifiers 
Se não estiver vendo as atividades serem retomadas nos aplicativos nativos corretos entre plataformas ou não conseguir ler as atividades publicadas por todos os membros no grupo, seu arquivo JSON poderá não estar sendo processado corretamente. Ao emitir esse arquivo, certifique-se de salvar o arquivo cross-platform-app-identifiers com codificação "Unicode (UTF-8 sem assinatura) – Codepage 65001".

#### <a name="updating-the-cross-platform-app-identifiers-json-file"></a>Atualizar o arquivo JSON cross-platform-app-identifiers 
O sistema armazenará em cache o conteúdo do arquivo JSON para evitar gerar solicitações frequentes em seu domínio. Se configurado, o serviço respeitará os cabeçalhos de cache HTTP ao avaliar quando o cache deverá ser atualizado. Se não estiver configurado, o serviço será atualizado a cada 24 horas. 

## <a name="configure-your-app-client"></a>Configurar o cliente de aplicativos 
Se estiver usando as APIs no lado do cliente para Windows, iOS ou Android, será necessário verificar se seu cliente de aplicativos está configurado com o valor de host que representa a identidade de aplicativo entre dispositivos (por exemplo, contoso.com).

### <a name="microsoft-graph-apps"></a>Aplicativos Microsoft Graph 
Se estiver usando a API do feed de atividades no Microsoft Graph, seu valor de host precisa ser fornecido na propriedade **activitySourceHost**. Para saber mais, veja [tipo de recurso de atividade](/graph/api/resources/projectrome-activity?view=graph-rest-1.0).

### <a name="universal-windows-apps"></a>Aplicativos Universais do Windows
Se tiver um aplicativo do Windows, será necessário configurar o valor do host no manifesto do aplicativo antes de publicar os dados. Para saber mais, veja [uap5:UserActivity](/uwp/schemas/appxpackage/uapmanifestschema/element-uap5-useractivity). 

<!-- Removing until we add the details.
### iOS & Android apps
*Details coming soon.*
-->

## <a name="maintaining-your-cross-device-app-configuration"></a>Manter a configuração do aplicativo entre dispositivos
Ao lançar um novo aplicativo que gerará atividades de usuário, é importante atualizar o aplicativo entre dispositivos com os novos valores de configuração antecipadamente para que as novas atividades publicadas sejam associadas corretamente com o aplicativo entre dispositivos. A configuração de aplicativo entre dispositivos associada às atividades do usuário que foram publicadas antes de uma alteração na configuração não será atualizada automaticamente. No entanto, uma operação de atualização realizada em qualquer atividade com uma configuração anterior será atualizada para a versão mais recente do arquivo.  

## <a name="troubleshooting"></a>Solução de problemas

A seguir estão alguns problemas comuns que podem acontecer com a API do feed de atividades.

### <a name="activities-are-not-available-to-read-and-write-for-all-apps-in-the-cross-device-app-configuration"></a>As atividades não estão disponíveis para ler e gravar em todos os aplicativos na configuração de aplicativo entre dispositivos
A API do feed de atividades recebe a configuração de aplicativo entre dispositivos de forma assíncrona de forma que os erros de configuração possam não estar prontamente aparentes ao publicar as atividades de usuário. Caso o serviço falhe na recepção do arquivo JSON, seja devido a TLS ou a um erro de formatação, essas atividades publicadas serão atribuídas apenas à ID do aplicativo que publicou a atividade. No caso de atividades publicadas pelo Microsoft Graph, esta é a ID de aplicativo de conta da Microsoft usada para autorizar solicitações do Microsoft Graph. No caso de atividades publicadas por APIs do lado do cliente, activity.applicationId registrará apenas a ID do aplicativo específico da plataforma que publicou a atividade. Isso impedirá operações de leitura e gravação em atividades de outros aplicativos específicos da plataforma identificados na configuração de aplicativo entre dispositivos. 

### <a name="platform-will-not-initialize-on-android-or-ios"></a>A plataforma não inicializa no Android ou no iOS
A API de retransmissão do dispositivo no Android ou iOS precisa da configuração do aplicativo entre dispositivos para fazer instância das conexões no aplicativo Android ou iOS. Caso a plataforma não seja inicializada com êxito, certifique-se de ter identificado corretamente as IDs de aplicativo da conta Microsoft e as credenciais de notificação por push usadas para configurar seu aplicativo entre dispositivos no Centro de Desenvolvimento do Windows e configure o valor de host dos aplicativos cliente com o domínio que identifica o aplicativo entre dispositivos.
