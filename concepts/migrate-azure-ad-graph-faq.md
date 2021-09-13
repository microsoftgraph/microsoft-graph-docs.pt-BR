---
title: Azure Active Directory (Azure AD) Graph perguntas frequentes sobre Graph migração da Microsoft
description: Azure Active Directory (Azure AD) Graph perguntas frequentes sobre Graph migração da Microsoft.
author: FaithOmbongi
ms.localizationpriority: medium
ms.prod: applications
ms.openlocfilehash: fce5d843994526f5546375c72c1d6b536352b4f6
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59139160"
---
# <a name="azure-active-directory-azure-ad-graph-to-microsoft-graph-migration-faq"></a>Azure Active Directory (Azure AD) Graph perguntas frequentes sobre Graph migração da Microsoft

Este artigo fornece respostas para perguntas frequentes sobre como migrar do Azure AD Graph para o Microsoft Graph.

## <a name="how-is-microsoft-graph-different-from-azure-ad-graph-and-why-should-i-migrate-my-apps"></a>Como a Microsoft Graph diferente do Azure AD Graph e por que devo migrar meus aplicativos?

A API do Azure AD Graph oferece acesso apenas aos serviços do Azure AD. A API do Microsoft Graph oferece um único ponto de extremidade unificado para acessar serviços do Azure AD e outros serviços Microsoft, como Microsoft Teams, Microsoft Exchange e Microsoft Intune.

O Microsoft Graph também é mais seguro e resiliente do que o Azure AD Graph. Por esse motivo, o Azure AD Graph está em um caminho de deprecação desde 30 de junho de 2020 e será retirado em 30 de junho de 2022. Após 30 de junho de 2022, seus aplicativos não receberão mais respostas do ponto de extremidade do Azure AD Graph. Migre para o Microsoft Graph para evitar perda de funcionalidade.

## <a name="as-a-developer-how-do-i-identify-apps-that-use-azure-ad-graph"></a>Como desenvolvedor, como posso identificar aplicativos que usam o Azure AD Graph?

Siga estas etapas para identificar aplicativos com uma dependência do Azure AD Graph:

### <a name="step-1-scan-the-application-source-code"></a>Etapa 1: Examinar o código-fonte do aplicativo

Se você possuir o código-fonte de um aplicativo, procure o `https://graph.windows.net/` URI no código. Este é o ponto de extremidade do Azure AD Graph aplicativos que chamam esse ponto de extremidade usam o Azure AD Graph. Grave o valor da ID do aplicativo afetado.

### <a name="step-2-check-the-apps-api-permissions-on-the-azure-portal"></a>Etapa 2: Verificar as permissões de API do aplicativo no portal do Azure

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela **Registros de aplicativo,** selecione a guia Todos os **Aplicativos** e selecione a **opção Adicionar filtros.** Escolha a **opção ID de aplicativo (cliente)** na lista de filtros disponíveis e selecione **Aplicar**.  Um filtro aparece.
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
1. Na janela Registros de aplicativo, selecione a guia **Todos os Aplicativos** e selecione a **opção Adicionar filtros.** Escolha a **opção API Solicitada** na lista de filtros disponíveis e selecione **Aplicar**. O **filtro API Solicitado** é apasado.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI.png" alt-text="Filtrar aplicativos pela API solicitada." border="true":::

5. Selecione **APIs da Microsoft**. Selecione o **drop-down Por favor, selecione** uma API e escolha **Azure Active Directory Graph**. Selecione **Aplicar**. Isso lista todos os aplicativos com uma dependência do Azure AD Graph.

    :::image type="content" source="/graph/images/aadgraph-to-msgraph-migration/RequestedAPI-AAD.png" alt-text="Filtrar aplicativos que usam o Azure AD Graph." border="true":::

### <a name="method-3-use-a-powershell-script"></a>Método 3: usar um script do PowerShell

Baixe e execute [este script do PowerShell.](https://github.com/microsoft/AzureADGraphApps)



## <a name="microsoft-sent-me-an-email-with-a-list-of-app-ids-for-apps-using-azure-ad-graph-how-do-i-find-the-details-of-each-app-including-its-owner"></a>A Microsoft me enviou um email com uma lista de IDs de aplicativos para aplicativos usando o Azure AD Graph. Como encontro os detalhes de cada aplicativo, incluindo seu proprietário?

1. Entre no [portal do Azure](https://portal.azure.com) como administrador global.
1. Pesquise e **selecione Azure Active Directory**.
1. Em **Gerenciar**, selecione **Registros de aplicativo**.
1. Na janela Registros de aplicativos, selecione a guia **Todos os Aplicativos** e selecione **Adicionar filtros.** Escolha a **opção ID de aplicativo (cliente)** na lista de filtros disponíveis e selecione **Aplicar**.  Um filtro aparece.
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

## <a name="i-need-to-create-new-apps-to-use-azure-ad-graph-but-the-azure-ad-graph-api-permission-sign-up-is-closed-how-can-i-create-my-app"></a>Preciso criar novos aplicativos para usar o Azure AD Graph mas a assinatura de permissão da API do Azure AD Graph está fechada. Como posso criar meu aplicativo?

Primeiro, recomendamos que você siga a [lista](migrate-azure-ad-graph-planning-checklist.md) de verificação planejamento de migração de aplicativos para ajudá-lo a fazer a transição de seus aplicativos para a API Graph Microsoft. 

Se você tiver identificado uma lacuna em que o Microsoft Graph não dá suporte a um recurso suportado pelo Azure AD Graph, trabalhe com o administrador do locatário ou o proprietário da assinatura para relatar a lacuna. Quando verificarmos se essa é realmente uma lacuna que a API do Microsoft Graph não atende, ajudaremos você a criar o aplicativo. No entanto, isso não significa uma exceção à depreciação. O aplicativo que usa o Azure AD Graph ainda vai parar de funcionar após 30 de junho de 2022.


## <a name="see-also"></a>Confira também

+ [Lista de verificação para migração de aplicativos](migrate-azure-ad-graph-request-differences.md)
