---
title: Novidades do Microsoft Graph
description: O que há de novo no Microsoft Graph
author: angelgolfer-ms
ms.localizationpriority: high
ms.openlocfilehash: fb160f96c2145c22f3f0da866b1a40410d116508
ms.sourcegitcommit: 12f07c009c57db3cc9174b165b5ec30195c00996
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/30/2021
ms.locfileid: "61646997"
---
# <a name="whats-new-in-microsoft-graph"></a>Novidades do Microsoft Graph

Veja os destaques das novidades nos dois últimos meses do Microsoft Graph, [o que foi adicionado anteriormente](whats-new-earlier.md) e como você pode [compartilhar suas ideias](#want-to-stay-in-the-loop). Para obter uma lista detalhada de atualizações no nível da API, consulte o [registro de alterações da API](https://developer.microsoft.com/graph/changelog/). 

> [!IMPORTANT]
> Recursos, incluindo APIs e ferramentas, no status de _visualização_ podem mudar sem aviso prévio e alguns podem nunca ser promovidos ao status de disponibilidade geral (GA). Não utilize recursos de visualização em aplicativos de produção.


## <a name="december-2021-new-and-generally-available"></a>Dezembro de 2021: novo e disponível ao público geral

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
[Inscreva-se nas notificações de alterações](/graph/api/subscription-post-subscriptions?view=graph-rest-beta&preserve-view=true) no status de [presença](/graph/api/resources/presence) de um usuário especificado. Sempre especifique um certificado de criptografia na solicitação de assinatura, pois são [notificações avançadas que incluem dados de recursos criptografados](webhooks-with-resource-data.md).

## <a name="december-2021-new-in-preview-only"></a>Dezembro de 2021: novo apenas na visualização

### <a name="cloud-communications--presence"></a>Comunicações na nuvem | Presença
- Use a ação [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true) para definir o status de disponibilidade e atividade preferencial de um usuário. A presença do usuário se torna a presença preferencial.
- Use a ação [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true) para limpar os status de disponibilidade e atividade preferencial de um usuário.
- Use `Presence.ReadWrite` como permissão delegada com [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true)ou [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).
- Use `Presence.ReadWrite.All` como permissão de aplicativo com [setPresence](/graph/api/presence-setpresence?view=graph-rest-beta&preserve-view=true), [clearPresence](/graph/api/presence-clearpresence?view=graph-rest-beta&preserve-view=true), [setUserPreferredPresence](/graph/api/presence-setuserpreferredpresence?view=graph-rest-beta&preserve-view=true)ou [clearUserPreferredPresence](/graph/api/presence-clearuserpreferredpresence?view=graph-rest-beta&preserve-view=true).

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- [Obter](/graph/api/application-get?view=graph-rest-beta&preserve-view=true) os detalhes de certificação de um [aplicativo](/graph/api/resources/application?view=graph-rest-beta&preserve-view=true) pela propriedade de **certificação**. A propriedade é definida apenas quando o aplicativo é certificado pelo [Programa de Conformidade do Aplicativo do Microsoft 365](/microsoft-365-app-certification/docs/enterprise-app-certification-guide).  
- [Inclua](/graph/api/permissiongrantpolicy-post-includes?view=graph-rest-beta&preserve-view=true) ou [exclua](/graph/api/permissiongrantpolicy-post-excludes?view=graph-rest-beta&preserve-view=true) a certificação como uma [condição](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true) em uma [política de concessão de permissão](/graph/api/resources/permissiongrantpolicy?view=graph-rest-beta&preserve-view=true) pela propriedade **certifiedClientApplicationsOnly** de [permissionGrantConditionSet](/graph/api/resources/permissionGrantConditionSet?view=graph-rest-beta&preserve-view=true).

### <a name="search--index"></a>Pesquisa | Índice
Use a operação [atualizar](/graph/api/externalconnectors-schema-update?view=graph-rest-beta&preserve-view=true) para atualizar as propriedades dos itens em um esquema de [conexão](/graph/api/resources/externalconnectors-externalconnection?view=graph-rest-beta&preserve-view=true), incluindo seus aliases e rótulos.


## <a name="november-2021-new-and-generally-available"></a>Novembro de 2021: Novo e geralmente disponível ao público

### <a name="files"></a>Arquivos
Obtenha o estado de uma unidade a partir de um horário específico especificando o carimbo de data/hora codificado no URL correspondente. Veja um [exemplo](/graph/api/driveitem-delta#example-4-retrieving-delta-results-using-a-timestamp).

### <a name="identity-and-access--identity-and-sign-in"></a>Identidade e acesso | Identidade e login
- Execute [campanhas](/graph/api/resources/authenticationMethodsRegistrationCampaign) e [imponha os usuários a se registrarem](/graph/api/resources/registrationEnforcement) no momento da entrada para configurar os métodos de autenticação direcionados.
-  Configurar um [provedor de identidade Apple](/graph/api/resources/applemanagedidentityprovider) em um locatário do Azure AD B2C.

## <a name="november-2021-new-in-preview-only"></a>Novembro de 2021: Novo somente na pré-visualização

### <a name="cloud-communications--online-meeting"></a>Comunicações na nuvem | Reunião online
Admita automaticamente novos tipos de participantes em uma reunião online e ignore o lobby da reunião:
- Somente pessoas convidadas pelo organizador.
- Somente os participantes da mesma empresa.

### <a name="devices-and-apps--cloud-pc"></a>Dispositivos e aplicativos | Computador na nuvem
- Defina uma [configuração](/graph/api/resources/cloudPcDomainJoinConfiguration?view=graph-rest-beta&preserve-view=true) de como um dispositivo de PC na nuvem provisionado pode ingressar no Azure Active Directory (Microsoft Azure AD): somente nuvem e ingressar somente no Microsoft Azure AD, ou híbrido e ingressar no Active Directory local e no Microsoft Azure AD.
- Obtenha o [recurso de imagem da galeria](/graph/api/resources/cloudPcGalleryImage?view=graph-rest-beta&preserve-view=true) da organização atual que pode ser usado para provisionar um PC na nuvem.

### <a name="devices-and-apps--device-updates"></a>Dispositivos e aplicativos | Atualizações do dispositivo
- Use as [configurações de salvaguarda](/graph/api/resources/windowsupdates-safeguardSettings?view=graph-rest-beta&preserve-view=true) para recusar as proteções contra prováveis problemas em uma implantação.
- Suporte para um [estado de implantação](/graph/api/resources/windowsupdates-deploymentState?view=graph-rest-beta&preserve-view=true) em que uma implantação está com defeito devido ao conteúdo não ser mais implantável, por exemplo, no fim do serviço.

### <a name="identity-and-access--directory-management"></a>Identidade e acesso | Gerenciamento do diretório
- Defina e atribua [atributos de segurança personalizado ](/graph/api/resources/custom-security-attributes-overview?view=graph-rest-beta&preserve-view=true) aos objetos do Microsoft Azure AD. Use esses atributos para armazenar informações, categorizar objetos ou impor um controle de acesso refinado sobre recursos específicos do Azure. Use esses atributos com o [Controle de acesso baseado em atributo do Azure](/azure/role-based-access-control/conditions-overview) (Azure ABAC).
- [Crie um grupo dentro de uma unidade administrativa](/graph/api/administrativeunit-post-members?view=graph-rest-beta&preserve-view=true).

### <a name="reports--microsoft-365-usage-reports"></a>Relatórios | Relatórios de uso do Microsoft 365
[Os relatórios de uso do Microsoft 365](/graph/api/resources/report?view=graph-rest-beta&preserve-view=true) no tipo de saída JSON não são mais fortemente tipados e são do tipo `Edm.Stream`. Para obter mais informações, consulte [Alterações da propriedade OData na API de relatórios de uso do Microsoft 365 no Microsoft Graph](https://devblogs.microsoft.com/microsoft365dev/odata-property-changes-to-microsoft-365-usage-reports-api-in-microsoft-graph/).

### <a name="teamwork"></a>Trabalho em equipe
Marque um chat como [lido](/graph/api/chat-markChatReadForUser?view=graph-rest-beta&preserve-view=true) ou [não lido](/graph/api/chat-markchatunreadforuser?view=graph-rest-beta&preserve-view=true) para um usuário.



## <a name="want-to-stay-in-the-loop"></a>Quer ficar por dentro?

Estas são algumas maneiras de se envolver:

- Existem cenários em que você gostaria que o Microsoft Graph oferecesse suporte? Sugira e vote nos novos recursos na [Comunidade Microsoft Tech](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).
    Alguns novos recursos são originados como solicitações populares da comunidade de desenvolvedores. A equipe do Microsoft Graph avalia regularmente as necessidades dos clientes e lança novos recursos na seguinte ordem:

    1. Estreia no status de **_visualização_**. Todas as atualizações da API REST relacionadas estão no ponto de extremidade beta (`https://graph.microsoft.com/beta`).  

    2. Promovido para o status de **_disponibilidade geral_ (GA)**, se um feedback suficiente indicar a viabilidade. Todas as atualizações da API REST relacionadas serão adicionadas ao ponto de extremidade do v 1.0 (`https://graph.microsoft.com/v1.0`). 
- Seja um membro ativo da comunidade do Microsoft Graph! [Participe](https://aka.ms/microsoftgraphcall) da chamada mensal à comunidade do Microsoft Graph.
- Inscreva-se no [programa para desenvolvedores do Microsoft 365](https://developer.microsoft.com/office/dev-program), ganhe uma assinatura gratuita do Microsoft 365 e comece a desenvolver!


## <a name="see-also"></a>Confira também
- Confira o [blog de desenvolvedores do Microsoft Graph](https://developer.microsoft.com/graph/blogs/) periodicamente para comunicados de lançamentos e recursos úteis.
- Navegue pelas informações das inclusões da API do Microsoft Graph e pelas atualizações de comportamento de API no [changelog](https://developer.microsoft.com/graph/changelog/).
- Encontre [destaques de versões anteriores](whats-new-earlier.md).
- Saiba mais sobre o [controle de versão, suporte e mudanças significativas de políticas do Microsoft Graph](versioning-and-support.md).
