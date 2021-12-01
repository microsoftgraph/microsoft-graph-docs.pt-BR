---
title: Perguntas frequentes sobre migração do Azure AD Graph Microsoft Graph migração
description: Fornece respostas para perguntas frequentes sobre como migrar do Azure Active Directory (Azure AD) Graph para o Microsoft Graph.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: 34bbf90b42d1b85acc5f768599c4b50a88b859b1
ms.sourcegitcommit: e1dd9860906e0b415fd376d70df1f928d1f3d29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/01/2021
ms.locfileid: "61241300"
---
# <a name="azure-ad-graph-to-microsoft-graph-migration-faq"></a>Perguntas frequentes sobre migração do Azure AD Graph Microsoft Graph migração

Este artigo fornece respostas para perguntas frequentes sobre como migrar do Azure Active Directory (Azure AD) Graph para o [Microsoft Graph](/graph/overview).

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Como a Microsoft Graph diferente do Azure AD Graph e por que devo migrar meus aplicativos?

A API do Azure AD Graph oferece acesso apenas aos serviços do Azure AD. A API do Microsoft Graph oferece um único ponto de extremidade unificado para acessar serviços do Azure AD e outros serviços Microsoft, como Microsoft Teams, Microsoft Exchange e Microsoft Intune.

[O Microsoft Graph](/graph/overview) também é mais seguro e resiliente do que o Azure AD Graph. Por esse motivo, o Azure AD Graph está em um caminho de deprecação desde 30 de junho de 2020 e será retirado em 30 de junho de 2022. Após 30 de junho de 2022, seus aplicativos não receberão mais respostas do ponto de extremidade do Azure AD Graph. Migre para o Microsoft Graph para evitar perda de funcionalidade.

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>Como desenvolvedor, como posso identificar aplicativos que usam o Azure AD Graph?

Siga estas etapas para identificar aplicativos com uma dependência do Azure AD Graph:

### <a name="step-1-scan-the-application-source-code"></a>Etapa 1: Examinar o código-fonte do aplicativo

Se você possuir o código-fonte de um aplicativo, procure o `https://graph.windows.net/` URI no código. Este é o ponto de extremidade do Azure AD Graph aplicativos que chamam esse ponto de extremidade usam o Azure AD Graph. Grave o valor da ID do aplicativo afetado.

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>Etapa 2: Verificar as permissões de API do aplicativo no portal do Azure

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativos,** habilita a visualização de pesquisa **registros de aplicativos**. Selecione a **guia Todos os Aplicativos** e selecione a **opção Adicionar filtros.** Escolha a **opção ID de aplicativo (cliente)** na lista de filtros disponíveis e selecione **Aplicar**.  Um filtro aparece.
1. Na caixa de texto, insira a ID do aplicativo que você recuperou na Etapa 1 e selecione **Aplicar**. A lista foi limitada ao aplicativo especificado.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Filtrar por aplicativos por ID do aplicativo." border="true":::

1. Selecione o aplicativo. Isso revela o menu do aplicativo.
1. No painel esquerdo da janela, selecione **permissões de API**. Isso revela permissões de API configuradas para seu aplicativo, incluindo permissões Graph Azure AD.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/configuredPermissions.png" alt-text="Uma lista de permissões de API de um aplicativo do portal do Azure." border="true":::


## <a name="as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph"></a>Como administrador de IT, como posso identificar aplicativos no meu locatário que usam o Azure AD Graph?

Use um dos três métodos a seguir para identificar aplicativos em seu locatário com uma dependência do Azure AD Graph.

### <a name="method-1-through-network-proxy-logs"></a>Método 1: por meio de logs de proxy de rede

Verifique os logs de tráfego do servidor de rede por meio de um proxy de filtro para todos os aplicativos que chamam o `https://graph.windows.net/` ponto de extremidade. Esses aplicativos usam o Azure AD Graph.

### <a name="method-2-use-the-app-registrations-menu-of-the-azure-portal"></a>Método 2: Usar o menu Registros de aplicativos do portal do Azure

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativos,** habilita a visualização de pesquisa **registros de aplicativos**. Selecione a **guia Todos os Aplicativos** e selecione a **opção Adicionar filtros.** Escolha a **opção API Solicitada** na lista de filtros disponíveis e selecione **Aplicar**. O **filtro API Solicitado** é apasado.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="Filtrar aplicativos pela API solicitada." border="true":::

5. Selecione **APIs da Microsoft**. Selecione o **drop-down Por favor, selecione** uma API e escolha **Azure Active Directory Graph**. Selecione **Aplicar**. Isso lista todos os aplicativos com uma dependência do Azure AD Graph.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="Filtrar aplicativos que usam o Azure AD Graph." border="true":::

### <a name="method-3-use-a-powershell-script"></a>Método 3: usar um script do PowerShell

Baixe e execute [este script do PowerShell.](https://github.com/microsoft/AzureADGraphApps)



## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>A Microsoft me enviou um email com uma lista de IDs de aplicativos para aplicativos usando o Azure AD Graph. Como encontro os detalhes de cada aplicativo, incluindo seu proprietário?

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativos,** habilita a visualização de pesquisa **registros de aplicativos**. Selecione a **guia Todos os Aplicativos** e selecione a **opção Adicionar filtros.** Escolha a **opção ID de aplicativo (cliente)** na lista de filtros disponíveis e selecione **Aplicar**.  Um filtro aparece.
1. Insira uma ID de aplicativo na caixa de texto e selecione **Aplicar**. A lista foi limitada ao aplicativo especificado.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppClientIDFilter.png" alt-text="Filtrar por aplicativos por ID do aplicativo." border="true":::

6. Selecione o aplicativo. Isso revela o menu do aplicativo. No painel esquerdo da janela, opções de menu como **Proprietários** permitem recuperar os detalhes do aplicativo.

## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-are-these-all-the-affected-apps"></a>A Microsoft me enviou um email com uma lista de IDs de aplicativos para aplicativos usando o Azure AD Graph. São todos os aplicativos afetados?

Essa lista captura apenas aplicativos usados nos últimos 28 dias e que chamaram o ponto de extremidade do Azure AD Graph endpoint. Como alguns aplicativos podem ter uso sazonal, a ID do aplicativo pode ser capturada na lista de um mês, mas não em outra. Para recuperar a lista completa de aplicativos afetados, recomendamos que você siga um dos três métodos [listados](#as-an-it-admin-how-do-i-identify-apps-in-my-tenant-that-use-azure-ad-graph) anteriormente.

## <a name="im-a-subscription-owner-and-microsoft-sent-me-an-email-about-azure-ad-graph-deprecation-with-a-list-of-app-ids-what-should-i-do"></a>Sou proprietário de assinatura e a Microsoft me enviou um email sobre o Graph do Azure AD com uma lista de IDs de aplicativo. O que devo fazer?

O email recebido inclui as IDs de locatário vinculadas às IDs do aplicativo. Siga estas etapas para recuperar os detalhes de contato técnicos para os locatários específicos.
1. Entre no [portal do Azure](https://portal.azure.com) como administrador.
1. Se você for um proprietário de assinatura em vários locatários do Azure AD, alterna primeiro para o locatário ou diretório relevante.
    1. Na parte superior direita da janela, selecione seu ícone de perfil e escolha **Alternar diretório**. Isso revela as **configurações do Portal | Janela Diretórios + assinaturas.** 
    1. Na lista, use a guia **Alternar** para o diretório cuja ID de Diretório corresponde à ID de locatário que você recebeu no email. O active directory está marcado **como Current**.
    1. Feche a janela.
1. No diretório relevante, pesquise e **selecione Azure Active Directory**. Isso revela um menu para seu locatário ativo. 
1. No painel esquerdo da janela, em **Gerenciar**, selecione **Propriedades**.
1. Na janela **Propriedades do** locatário, primeiro verifique se o valor da ID do Locatário corresponde a uma ID de locatário que você recebeu no email. Recupere os **detalhes de contato** técnicos para entrar em contato com o locatário para que ele possa estar ciente da precarização.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/tenantTechnicalContact.png" alt-text="Encontre contato técnico de um locatário." border="true":::

## <a name="i-know-apps-that-are-using-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph"></a>Eu sei que aplicativos que estão usando o Azure AD Graph. Como migrá-los para o Microsoft Graph?

Para migrar seus aplicativos do Azure AD Graph para o Microsoft Graph, siga a lista de verificação planejamento [de migração de aplicativos.](migrate-azure-ad-graph-planning-checklist.md)

## <a name="i-dont-own-some-apps-in-my-tenant-but-they-use-azure-ad-graph-how-do-i-migrate-them-to-microsoft-graph-api-can-i-find-the-owner-of-such-apps"></a>Não tenho alguns aplicativos no meu locatário, mas eles usam o Azure AD Graph. Como migrá-los para a API Graph Microsoft? Posso encontrar o proprietário desses aplicativos?

Primeiro, confirme a lista completa de aplicativos pertencentes ao seu locatário ou aplicativos de terceiros integrados ao seu locatário.

1. Entre no [portal do Azure](https://portal.azure.com) como administrador.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela Registros de aplicativo, selecione a **guia Todos os Aplicativos.**
1. Selecione o aplicativo. Isso revela o menu do aplicativo.
1. No painel esquerdo da janela, as opções de menu revelam os detalhes do aplicativo, incluindo seus Proprietários.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/AppOwners.png" alt-text="Encontre proprietários de aplicativos." border="true":::


## <a name="can-i-request-for-an-exception-if-im-unable-to-meet-the-june-30-2022-migration-deadline"></a>Posso solicitar uma exceção se não conseguir cumprir o prazo de migração de 30 de junho de 2022?  

Não há exceções para essa precarização. Seus aplicativos não receberão mais respostas do ponto de extremidade do Azure AD Graph após 30 de junho de 2022.

## <a name="my-organization-runs-azure-stack-hub-what-actions-should-i-take"></a>Minha organização executa o Azure Stack Hub. Quais ações devo tomar?

Se sua organização executa o Azure Stack Hub, a ação mais importante é seguir a política de manutenção do Hub de Pilha do [Azure.](/azure-stack/operator/azure-stack-servicing-policy)

Se necessário, o Azure Stack Hub continuará usando o Azure AD Graph além de 30 de junho de 2022, para garantir que todos os sistemas migrem para o uso do Microsoft Graph. Para migrar, os clientes serão notificados por meio do portal de administração do Hub de Pilha do Azure para atualizar seus diretórios de locatários de residência e convidados. A migração para o Microsoft Graph será gerenciada pela experiência de atualização integrada do sistema.

## <a name="i-need-to-add-new-azure-ad-graph-permissions-to-my-app-but-i-cant-select-azure-ad-graph-as-a-required-permission-for-my-app-registration-how-can-i-add-the-azure-ad-graph-permissions"></a>Preciso adicionar novas permissões do Azure AD Graph ao meu aplicativo, mas não posso selecionar o Azure AD Graph como uma permissão necessária para o registro do meu aplicativo. Como posso adicionar as permissões do Azure AD Graph?

Primeiro, recomendamos que você siga a [lista](migrate-azure-ad-graph-planning-checklist.md) de verificação planejamento de migração de aplicativos para ajudá-lo a fazer a transição de seus aplicativos para a API Graph Microsoft.

Se você identificou uma lacuna em que o Microsoft Graph não dá suporte a um recurso disponível no Azure AD Graph, nos avise por meio do Microsoft Q&A usando a marca [azure-ad-graph-deprecation](/answers/topics/azure-ad-graph-deprecation.html).

Se você ainda precisar configurar as permissões do Azure AD Graph seus aplicativos, use uma das seguintes soluções alternativas.

+ Use a API [de](/graph/api/resources/application) aplicativo no Microsoft Graph atualizar [o objeto requiredResourceAccess](/graph/api/resources/requiredresourceaccess)
+ Use o cmdlet [Update-MgApplication](/powershell/module/microsoft.graph.applications/update-mgapplication?view=graph-powershell-1.0&preserve-view=true)   no Microsoft Graph PowerShell

Para exemplos usando as soluções alternativas listadas, consulte Usar o Microsoft Graph para configurar permissões necessárias do [Azure AD Graph](migrate-azure-ad-graph-configure-permissions.md) para um registro de aplicativo

>**Observação:** A adição Graph permissões do Azure AD usando essas soluções alternativas não será suportada após 30 de junho de 2022. Qualquer aplicativo usando o Azure AD Graph ainda irá parar de funcionar após 30 de junho de 2022.



## <a name="see-also"></a>Confira também

+ [Lista de verificação para migração de aplicativos](migrate-azure-ad-graph-request-differences.md)
