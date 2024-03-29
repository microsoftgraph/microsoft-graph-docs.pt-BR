---
title: Personalizar a privacidade das informações do item no Microsoft Graph (visualização)
description: Configurar a visibilidade dos insights derivados do Microsoft Graph usando o Centro de administração da Microsoft, o PowerShell ou o recurso userInsightsSettings da API REST.
author: simonhult
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: b495564ecbb67483a5a21a8f5490f92991ef682f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66444919"
---
# <a name="customize-item-insights-privacy-in-microsoft-graph-preview"></a>Personalizar a privacidade das informações do item no Microsoft Graph (visualização)

Insights do item são relações que a Microsoft calcula usando técnicas avançadas de aprendizagem de máquinas. Quando os usuários colaboram sobre documentos, sites e listas Microsoft Office SharePoint Online, chats e canais das Teams, a Microsoft agrega estas atividades como sinais. A partir dos sinais, a Microsoft obtém insights para fazer recomendações de conteúdo centradas no usuário para os usuários de uma organização.

Os insights do item podem ajudar os usuários a encontrar rapidamente arquivos que são importantes para eles, como na experiência **Recomendada** no Office.com e no Delve. Os usuários podem descobrir na área **Descobrir** no Outlook Mobile conteúdo potencialmente útil ao qual eles têm acesso, mas que podem não ter visto antes. A partir de insights personalizadas como **Arquivos recentes** em um cartão pessoal no Bing e **Recentes** em aplicativos Microsoft 365, os usuários podem facilmente descobrir seus arquivos recentes.

Esses item de insights refletem apenas o conteúdo ao qual os usuários têm acesso. Nenhum usuário recebe recomendações de conteúdo que não possa acessar.

> [!NOTE]
> Este artigo não aborda outras experiências baseadas em insights no Microsoft 365, como Viva Insights, o suplemento Insights para Outlook, recurso WorkWith, MyAnalytics e painel Insights.

## <a name="item-insights-privacy"></a>Privacidade de insights de item

As configurações de privacidade das informações do item oferecem a capacidade de configurar a visibilidade das informações derivadas do Microsoft Graph entre usuários e outros itens (como documentos ou sites) no Microsoft 365. Você pode desabilitar o aplicativo Delve por meio dos controles pré-existentes, mas permitir que outras experiências baseadas em informações continuem fornecendo assistência.

Este artigo descreve a personalização da privacidade dos insights de itens em uma organização. Para personalizar as percepções do item para um usuário, confira o recurso [userInsightsSettings](/graph/api/resources/userinsightssettings?view=graph-rest-beta&preserve-view=true). Essas configurações centradas no usuário são expostas por meio de uma propriedade de navegação chamada **itemInsights** no recurso [userSettings](/graph/api/resources/usersettings?view=graph-rest-beta&preserve-view=true).

## <a name="background"></a>Histórico

Na época do primeiro lançamento, em 2014, o Office Graph era um serviço de back-end para o Delve. Eles compartilhavam um conjunto de controles de privacidade sobre as informações do Office Graph e a experiência do usuário do Delve. Desde então, o Office Graph evoluiu e se tornou mais independente e eficiente, como parte de todas as experiências da Microsoft 365 e do Microsoft Graph. Para oferecer um esquema coerente do Microsoft Graph, a Microsoft introduziu uma entidade [itemInsights](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true), que herda todas as propriedades do recurso [officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-beta&preserve-view=true) pré-existente, e mantém o **officeGraphInsights** para obter uma compatibilidade com versões anteriores. A introdução de **itemInsights** também desassocia a história de privacidade das duas partes independentes.  

Embora os aplicativos existentes possam continuar a usar o **officeGraphInsights**, esses aplicativos devem ser atualizados para **itemInsights** para obter a flexibilidade de ajustar as informações do item no Office Graph e no Delve.

## <a name="how-to-customize-item-insights"></a>Como personalizar as informações do item

As configurações das informações do item fornecem flexibilidade para os administradores usarem as ferramentas do Microsoft Azure AD. Os administradores podem desabilitar as informações do item para toda a organização ou apenas para membros de um grupo específico do Microsoft Azure AD. Eles podem configurar as insights dos itens no Centro de administração do Microsoft 365, ou usando o PowerShell SDK ou Microsoft Graph REST API com as devidas permissões. Lembre-se de que a _função de administrador global_ é necessária.

A próxima seção descreve o uso do centro administrativo, e é seguida pela seção sobre PowerShell cmdlets. Se você estiver usando a API REST, pule as duas próximas seções e continue com [Definir as configurações de insights do item usando a API REST.](#configure-item-insights-settings-using-the-rest-api) Em seguida, confira as operações REST [ler](/graph/api/organizationsettings-list-iteminsights?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) para obter mais informações.

### <a name="configure-item-insights-settings-via-microsoft-admin-center"></a>Configurar as configurações de item de insights através do centro administrativo da Microsoft

Um administrador com o _papel de administrador global_ pode afinar as configurações de privacidade dos itens através de botões de alternância. Para fazer isso, no Centro de administração do Microsoft 365, expanda **Configurações**, selecione **Pesquisa e inteligência** e, em **Informações do item**, escolha **Alterar configurações**.
![imagem](https://user-images.githubusercontent.com/54312959/117024482-b39eca00-ad02-11eb-9a11-e6a01039822e.png)


### <a name="configure-item-insights-settings-via-powershell"></a>Configurar as configurações de item de insights via PowerShell

Confirme os seguintes pré-requisitos adicionais. Em seguida, você pode usar o [Microsoft Graph PowerShell SDK](/powershell/microsoftgraph/installation.md) para definir insights de item para toda a organização ou para grupos específicos.

#### <a name="additional-prerequisites"></a>Pré-requisitos adicionais

* **Módulo do PowerShell** - Instale a [versão do módulo 0.9.1 ou superior](https://www.powershellgallery.com/packages/Microsoft.Graph).
* **.NET Framework** - Instale o [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework) ou uma versão superior.

#### <a name="command-examples"></a>Exemplos de comando

> [!NOTE]
> Como os comandos de insights de itens estão disponíveis apenas em beta, alterne para o perfil beta antes de chamá-lo.
> ```powershell
>    Select-MgProfile beta
> ```

Para obter a configuração de insights do item para uma organização, use o módulo Microsoft Graph Windows PowerShell e o comando a seguir, onde você substitui `$TenantId` por sua ID de locatário do Azure Active Directory. Você pode recuperar essa ID na página de visão geral do Azure Active Directory.

```powershell
   Get-MgOrganizationSettingItemInsight -OrganizationId $TenantId
```

Por padrão, as informações do item estão habilitadas para toda a organização. É possível usar o módulo Microsoft Graph Windows PowerShell para alterar isso e desabilitar as percepções do item para todos na organização.

> [!NOTE]
> O método de atualização requer permissões `User.ReadWrite.All` adicionais. Para criar uma sessão do Microsoft Graph com um escopo necessário específico, use o comando a seguir e o consentimento para as permissões solicitadas.
> ```powershell
>    Connect-MgGraph -Scopes "User.Read.All","User.ReadWrite.All"
> ```

Usar o seguinte comando, em que você substitui `$TenantId`por sua ID de locatário do Azure Active Directory e especifica`-IsEnabledInOrganization` como `false`.

```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $TenantId -IsEnabledInOrganization:$false
```

Como alternativa, você pode alterar o padrão e desabilitar as informações do item para um grupo específico do Microsoft Azure AD. Usar o seguinte comando, onde você substitui `$TenantId` por sua ID de locatário do Azure Active Directory e `$GroupID` pela ID de grupo do Azure Active Directory.

```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $TenantId -DisabledForGroup $GroupId
```

### <a name="configure-item-insights-settings-using-the-rest-api"></a>Definir as configurações de insights do item usando a API REST

Conforme declarado anteriormente, por padrão, as configurações de privacidade das informações do item são habilitadas para toda a organização. Essas configurações são expostas por meio de uma propriedade de navegação chamada **itemInsights** em [organizationSettings](/graph/api/resources/organizationsettings?view=graph-rest-beta&preserve-view=true). Você pode alterar o padrão de duas maneiras:

- Desative os insights de itens para todos os usuários da organização, definindo a propriedade **isEnabledInOrganization** do recurso [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) como `false`. 
- Desabilite os insights de item para um _subconjunto_ de usuários, atribuindo esses usuários em um grupo do Microsoft Azure Active Directory e definindo a propriedade **disabledForGroup** para a ID desse grupo. Saiba mais sobre como [criar um grupo e adicionar usuários como membros](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Use a operação de [atualização](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) para definir as propriedades **isEnabledInOrganization** e **disabledForGroup** de acordo.

| Como as informações do item são habilitadas | isEnabledInOrganization | disabledForGroup |
|:-------------|:------------|:------------|
| Toda a organização (padrão) | `true` | vazio |
| Desabilitado para um subconjunto de usuários na organização | `true` | ID do grupo do Azure AD que contém o subconjunto de usuários |
| Desabilitado para toda a organização | `false` | ignorado |

Lembre-se do seguinte ao atualizar as configurações de informações do item:
- As [configurações de insights](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) estão disponíveis somente no ponto de extremidade beta.
- Obtenha a ID de um grupo do Azure AD no portal do Azure e verifique se o grupo existe, porque a operação de atualização não verifica a existência do grupo. Especificar um grupo inexistente no **disabledForGroup** _não_ desabilita as informações para todos os usuários da organização.
- Atualização das configurações pode levar até 24 horas para ser aplicada em todas as experiências Microsoft 365.
- Independentemente das configurações de informações do item, o Delve continua a respeitar as [configurações de privacidade](/sharepoint/delve-for-office-365-admins#control-access-to-delve-and-related-features?view=graph-rest-beta&preserve-view=true) do locatário e do usuário do Delve.


## <a name="behavior-changes-in-ui-and-apis"></a>O comportamento é alterado na IU e nas APIs
Para obter uma lista completa de experiências afetadas ao desabilitar os insights de itens, confira [Visão geral dos insights de itens](item-insights-overview.md#disabling-item-insights). 

## <a name="transition-period"></a>Período de transição
Para acomodar a configuração das informações do item, até o final de 2020, o Microsoft 365 respeitará as configurações do Delve e das informações sobre o item e aplicará o mais estrito, caso elas sejam diferentes. Isso significa que um usuário é considerado como excluído das informações do item, se o usuário tiver optado por excluir os controles do Delve ou as configurações de informações do item.

Após esse período de transição, as configurações do Delve controlarão apenas a experiência do Delve, e as configurações de informações do item afetarão apenas as informações do item do Microsoft Graph. Certifique-se de configurar as informações do item de acordo com os requisitos da sua organização.


> [!NOTE]
> Durante o período de transição, devido a razões técnicas, a página inicial do Microsoft Office SharePoint Online pode fornecer sugestões obsoletas se uma organização desabilitar a percepção dos itens para todos os usuários. Esta questão será abordada nas próximas mudanças do lado do servidor. 

## <a name="see-also"></a>Confira também
Saiba mais sobre o Delve e como usar as configurações de recursos do Delve para controlar os documentos que aparecem no feed **Discover**: 
- [Conectar-se e colaborar no Office Delve](https://support.microsoft.com/office/connect-and-collaborate-in-office-delve-46f92806-b52c-4187-b60e-b3bf8d25f73e)
- [Meus documentos estão seguros no Office Delve?](https://support.microsoft.com/office/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3)
- [Delve para administradores](/sharepoint/delve-for-office-365-admins)
