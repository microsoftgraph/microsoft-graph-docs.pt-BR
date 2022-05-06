---
title: Azure AD Graph perguntas frequentes sobre a migração do Microsoft Graph
description: Fornece respostas para perguntas frequentes sobre como migrar do Azure Active Directory (Azure AD) Graph para o Microsoft Graph.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 0605dfc2eb38f6339fe27f167599a211d1c80208
ms.sourcegitcommit: 972d83ea471d1e6167fa72a63ad0951095b60cb0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/06/2022
ms.locfileid: "65247067"
---
# <a name="azure-ad-graph-to-microsoft-graph-migration-faq"></a>Azure AD Graph perguntas frequentes sobre a migração do Microsoft Graph

Este artigo fornece respostas para perguntas frequentes sobre como migrar do Azure Active Directory (Azure AD) Graph para o [Microsoft Graph](/graph/overview).

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Como a Microsoft Graph diferente do Azure AD Graph e por que devo migrar meus aplicativos?

O Azure AD API do Graph oferece acesso apenas a Azure AD serviços. O Microsoft API do Graph oferece um único ponto de extremidade unificado para acessar serviços Azure AD e outros serviços Microsoft, como Microsoft Teams, Microsoft Exchange e Microsoft Intune.

[O Microsoft Graph](/graph/overview) também é mais seguro e resiliente do que Azure AD Graph. Por esse motivo, Azure AD Graph está em um caminho de substituição desde 30 de junho de 2020 e será desativado em um futuro próximo à medida que movermos todos os investimentos para o Microsoft Graph. Após a desativação, seus aplicativos receberão respostas de erro do Azure AD Graph ponto de extremidade. Migre para o Microsoft Graph para evitar a perda de funcionalidade.

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>Como desenvolvedor, como fazer para identificar aplicativos que usam Azure AD Graph?

Siga estas etapas para identificar aplicativos com uma dependência Azure AD Graph:

### <a name="step-1-scan-the-application-source-code"></a>Etapa 1: Examinar o código-fonte do aplicativo

Se você tiver o código-fonte de um aplicativo, pesquise o `https://graph.windows.net/` URI no código. Esse é o ponto Azure AD Graph e os aplicativos que chamam esse ponto de extremidade usam Azure AD Graph. Registre o valor da ID do aplicativo afetado.

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>Etapa 2: Verificar as permissões de API do aplicativo no portal do Azure

1. Entre [no portal do Azure como](https://portal.azure.com) administrador global.
1. Pesquise e selecione **Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativo**, habilite a **visualização Registros de aplicativo pesquisa.** Selecione a **guia Todos os Aplicativos** e, em seguida **, selecione a opção Adicionar filtros** . Escolha a **opção de ID do aplicativo (cliente)** na lista de filtros disponíveis e selecione **Aplicar**.  Um filtro é exibido.
1. Na caixa de texto, insira a ID do aplicativo que você recuperou na Etapa 1 e selecione **Aplicar**. A lista foi restringida ao aplicativo especificado.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Filtrar por aplicativos por ID do aplicativo." border="true":::

1. Selecione o aplicativo. Isso revela o menu do aplicativo.
1. No painel esquerdo da janela, selecione permissões **de API**. Isso revela permissões de API configuradas para seu aplicativo, incluindo Azure AD Graph permissões.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/configuredPermissions.png" alt-text="A lista de permissões de API de um aplicativo do portal do Azure." border="true":::


## <a name="as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph"></a>Como administrador de TI, como faço para identificar aplicativos em meu locatário que usam Azure AD Graph?

Use um dos três métodos a seguir para identificar aplicativos em seu locatário com uma dependência de Azure AD Graph.

### <a name="method-1-through-network-proxy-logs"></a>Método 1: por meio de logs de proxy de rede

Verifique os logs de tráfego do servidor de rede por meio de um proxy de filtro para todos os aplicativos que chamam o ponto `https://graph.windows.net/` de extremidade. Esses aplicativos usam Azure AD Graph.

### <a name="method-2-use-the-app-registrations-menu-of-the-azure-portal"></a>Método 2: usar o menu Registros de aplicativo do portal do Azure

1. Entre [no portal do Azure como](https://portal.azure.com) administrador global.
1. Pesquise e selecione **Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativo**, habilite a **visualização Registros de aplicativo pesquisa.** Selecione a **guia Todos os Aplicativos** e, em seguida **, selecione a opção Adicionar filtros** . Escolha a **opção API Solicitada** na lista de filtros disponíveis e selecione **Aplicar**. O **filtro de API** Solicitado é exibido.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="Filtre aplicativos por sua API solicitada." border="true":::

5. Selecione **AS APIs da Microsoft**. Selecione a **lista suspensa Por favor, selecione uma API** e escolha **Azure Active Directory Graph**. Selecione **Aplicar**. Isso lista todos os aplicativos com uma dependência Azure AD Graph.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="Filtrar aplicativos que usam Azure AD Graph." border="true":::

### <a name="method-3-use-a-powershell-script"></a>Método 3: Usar um script do PowerShell

Baixe e execute [este script do PowerShell](https://github.com/microsoft/AzureADGraphApps). Use esse método para recuperar aplicativos com seu diretório base em seu locatário e aplicativos com seus diretórios base em outros locatários.


## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>A Microsoft me enviou um email com uma lista de IDs de aplicativo para aplicativos usando Azure AD Graph. Como fazer encontrar os detalhes de cada aplicativo, incluindo seu proprietário?

1. Entre [no portal do Azure como](https://portal.azure.com) administrador global.
1. Pesquise e selecione **Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativo**, habilite a **visualização Registros de aplicativo pesquisa.** Selecione a **guia Todos os Aplicativos** e, em seguida **, selecione a opção Adicionar filtros** . Escolha a **opção de ID do aplicativo (cliente)** na lista de filtros disponíveis e selecione **Aplicar**.  Um filtro é exibido.
1. Insira uma ID do aplicativo na caixa de texto e selecione **Aplicar**. A lista foi restringida ao aplicativo especificado.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Filtrar por aplicativos por ID do aplicativo." border="true":::

6. Selecione o aplicativo. Isso revela o menu do aplicativo. No painel esquerdo da janela, opções de menu, como Proprietários, permitem que você recupere os detalhes do aplicativo.

## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-are-these-all-the-affected-apps"></a>A Microsoft me enviou um email com uma lista de IDs de aplicativo para aplicativos usando Azure AD Graph. Esses são todos os aplicativos afetados?

Essa lista captura apenas os aplicativos usados nos últimos 28 dias e que chamaram o ponto Azure AD Graph ponto de extremidade. Como alguns aplicativos podem ter uso sazonal, a ID do aplicativo pode ser capturada na lista de um mês, mas não em outra. Para recuperar a lista completa de aplicativos afetados, recomendamos que você siga um dos [três métodos listados](#as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph) anteriormente.

## <a name="im-a-subscription-owner-and-microsoft-sent-me-an-email-about-azure-ad-graph-deprecation-with-a-list-of-app-ids-what-should-i-do"></a>Sou proprietário da assinatura e a Microsoft me enviou um email sobre Azure AD Graph substituição com uma lista de IDs de aplicativo. O que devo fazer?

O email recebido inclui as IDs de locatário vinculadas às IDs do aplicativo. Siga estas etapas para recuperar os detalhes de contato técnico para os locatários específicos.
1. Entre [no portal do Azure como](https://portal.azure.com) administrador.
1. Se você for um proprietário de assinatura em vários locatários Azure AD, primeiro alterne para o locatário ou diretório relevante.
    1. No canto superior direito da janela, selecione o ícone de perfil e escolha **Alternar diretório**. Isso revela as **configurações do portal | Janela Diretórios + assinaturas** . 
    1. Na lista, use a guia **Alternar** para alternar para o diretório cuja ID de Diretório corresponde à ID de locatário que você recebeu no email. O active directory está marcado como **Atual**.
    1. Feche a janela.
1. No diretório relevante, pesquise e selecione **Azure Active Directory**. Isso revela um menu para seu locatário ativo. 
1. No painel esquerdo da janela, em **Gerenciar, selecione** **Propriedades**.
1. Na janela **Propriedades do locatário** , primeiro verifique se o valor da ID do Locatário corresponde a uma ID de locatário que você recebeu no email. Recupere os **detalhes do contato** técnico para entrar em contato com o locatário para que ele possa estar ciente da substituição.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/tenantTechnicalContact.png" alt-text="Localize o contato técnico de um locatário." border="true":::

## <a name="i-know-apps-that-are-using-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph"></a>Conheço aplicativos que estão usando Azure AD Graph. Como fazer migrá-los para o Microsoft Graph?

Para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph, siga a lista de verificação [de planejamento de migração de aplicativos](migrate-azure-ad-graph-planning-checklist.md).

## <a name="i-dont-own-some-apps-in-my-tenant-but-they-use-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph-api-can-i-find-the-owner-of-such-apps"></a>Não tenho alguns aplicativos em meu locatário, mas eles usam Azure AD Graph. Como fazer migrá-los para o Microsoft API do Graph? Posso encontrar o proprietário desses aplicativos?

Primeiro, confirme a lista completa de aplicativos pertencentes a seu locatário ou aplicativos de terceiros integrados ao seu locatário.

1. Entre [no portal do Azure como](https://portal.azure.com) administrador.
1. Pesquise e selecione **Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela Registros de aplicativo, selecione a **guia Todos os Aplicativos**.
1. Selecione o aplicativo. Isso revela o menu do aplicativo.
1. No painel esquerdo da janela, as opções de menu revelam os detalhes do aplicativo, incluindo seus Proprietários.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppOwners.png" alt-text="Localize os proprietários do aplicativo." border="true":::


## <a name="my-organization-runs-azure-stack-hub-what-actions-should-i-take"></a>Minha organização executa o Azure Stack Hub. Quais ações devo tomar?

Se sua organização executar o Azure Stack Hub, a ação mais importante será seguir a política de [manutenção do Azure Stack Hub](/azure-stack/operator/azure-stack-servicing-policy).

Para migrar, os clientes serão notificados por meio do portal de administração do Azure Stack Hub para atualizar seus diretórios de locatários hospedados e convidados. A migração para o Microsoft Graph será gerenciada pela experiência de atualização integrada do sistema.

## <a name="i-need-to-add-new-azure-ad-graph-permissions-to-my-app-but-i-cant-select-azure-ad-graph-as-a-required-permission-for-my-app-registration-how-can-i-add-the-azure-ad-graph-permissions"></a>Preciso adicionar novas Azure AD Graph novas permissões ao meu aplicativo, mas não consigo selecionar Azure AD Graph como uma permissão necessária para o registro do meu aplicativo. Como posso adicionar as permissões Azure AD Graph dados?

Primeiro, recomendamos que você siga [a lista de](migrate-azure-ad-graph-planning-checklist.md) verificação de planejamento de migração de aplicativos para ajudá-lo a fazer a transição de seus aplicativos para o Microsoft API do Graph.

Se você identificou uma lacuna em que o Microsoft Graph não dá suporte a um recurso disponível no Azure AD Graph, informe-nos por meio do Microsoft Q&A usando a marca [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

Se você ainda precisar configurar Azure AD Graph permissões para seus aplicativos, use uma das soluções alternativas a seguir.

+ Use o portal do Azure para localizar as APIs que sua organização usa
+ Atualizar o manifesto do aplicativo no portal do Azure
+ Usar [a](/graph/api/resources/application) API do aplicativo no Microsoft Graph atualizar o [objeto requiredResourceAccess](/graph/api/resources/requiredresourceaccess)
+ Usar o [Update-MgApplicationcmdlet](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)  no Microsoft Graph SDK do PowerShell

Para obter exemplos usando as soluções alternativas listadas, consulte Usar o Microsoft Graph para configurar as permissões Azure AD Graph necessárias [para um registro de aplicativo](migrate-azure-ad-graph-configure-permissions.md)

>**Nota:** Não haverá Azure AD Graph permissões de uso dessas soluções alternativas após a desativação do Azure AD Graph. Qualquer aplicativo usando Azure AD Graph ainda vai parar de funcionar após a desativação.



## <a name="see-also"></a>Confira também

+ [Lista de verificação para migração de aplicativos](migrate-azure-ad-graph-request-differences.md)
