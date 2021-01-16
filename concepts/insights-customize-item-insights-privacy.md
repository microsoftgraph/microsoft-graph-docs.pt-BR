---
title: Personalizando a privacidade das informações do item no Microsoft Graph
description: ''
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: f4f143b66ba93b488c747eebfda7777e9800aea5
ms.sourcegitcommit: 1d2adc4062c8e83d23768682cf66a731bccd313c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/16/2021
ms.locfileid: "49883043"
---
# <a name="customizing-item-insights-privacy-in-microsoft-graph-preview"></a>Personalizando a privacidade das informações do item no Microsoft Graph (visualização)

As configurações de privacidade das informações do item oferecem a capacidade de configurar a visibilidade das informações derivadas do Microsoft Graph, entre usuários e outros itens (como documentos ou sites) no Microsoft 365. Você pode desabilitar o aplicativo Delve por meio dos controles pré-existentes, mas permitir que outras experiências baseadas em informações continuem fornecendo assistência.

## <a name="background"></a>Histórico
Na época do primeiro lançamento, em 2014, o Office Graph era um serviço de back-end para o Delve. Eles compartilhavam um conjunto de controles de privacidade sobre as informações do Office Graph e a experiência do usuário do Delve. Desde então, o Office Graph evoluiu e se tornou mais independente e eficiente, como parte de todas as experiências da Microsoft 365 e do Microsoft Graph. Para oferecer um esquema coerente do Microsoft Graph, a Microsoft introduziu uma entidade [itemInsights](/graph/api/resources/iteminsights?view=graph-rest-beta&preserve-view=true), que herda todas as propriedades do recurso [officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-beta&preserve-view=true) pré-existente, e mantém o **officeGraphInsights** para obter uma compatibilidade com versões anteriores. A introdução de **itemInsights** também desassocia a história de privacidade das duas partes independentes.  

Embora os aplicativos existentes possam continuar a usar o **officeGraphInsights**, esses aplicativos devem ser atualizados para **itemInsights** para obter a flexibilidade de ajustar as informações do item no Office Graph e no Delve.

## <a name="how-to-customize-item-insights"></a>Como personalizar as informações do item?

As configurações das informações do item fornecem flexibilidade para os administradores usarem as ferramentas do Microsoft Azure AD. Os administradores podem desabilitar as informações do item para toda a organização ou apenas para membros de um grupo específico do Microsoft Azure AD. Configure as informações do item usando o SDK do PowerShell ou a API REST do Microsoft Graph com as devidas permissões. Lembre-se de que a _função de administrador global_ é necessária. 

A próxima seção descreve o uso de cmdlets do PowerShell para definir as configurações das informações. Se você estiver usando a API REST, pule a próxima seção e continue em [Configurar informações do item usando a API REST](#configure-item-insights-using-rest-api). Em seguida, confira as operações REST [ler](/graph/api/iteminsightssettings-get?view=graph-rest-beta&preserve-view=true) ou [atualizar](/graph/api/iteminsightssettings-update?view=graph-rest-beta&preserve-view=true) para obter mais informações.

### <a name="how-to-configure-item-insights-setting-via-powershell"></a>Como definir a configuração das informações do item pelo PowerShell?
Confirme os pré-requisitos adicionais a seguir. Em seguida, você pode usar o [Microsoft Graph PowerShell SDK](./powershell/installation.md) para definir informações do item para toda a organização ou para grupos específicos.

#### <a name="additional-prerequisites"></a>Pré-requisitos adicionais
* **Módulo do PowerShell** - Instale a [versão do módulo 0.9.1 ou superior](https://www.powershellgallery.com/packages/Microsoft.Graph).
* **.NET Framework** - Instale o [.NET Framework 4.7.2](https://dotnet.microsoft.com/download/dotnet-framework) ou uma versão superior.

#### <a name="command-examples"></a>Exemplos de comando
> [!NOTE]
> Como os comandos de insights de itens estão disponíveis apenas em beta, alterne para o perfil beta antes de chamá-lo.
> ```powershell
>    Select-MgProfile beta
> ```
Para obter a configuração das informações do item de uma organização, use o módulo Microsoft Graph PowerShell e o seguinte comando, onde você substitui `$OrgID` pela ID aplicável da sua organização:
```powershell
   Get-MgOrganizationSettingItemInsight -OrganizationId $OrgID
```

Por padrão, as informações do item estão habilitadas para toda a organização. É possível usar o módulo Microsoft Graph Windows PowerShell para alterar isso e desabilitar as percepções do item para todos na organização. 
> [!NOTE]
> O método de atualização requer permissões `User.ReadWrite` adicionais. Para criar uma sessão do Microsoft Graph com um escopo específico necessário, use o seguinte comando e concorde com as permissões solicitadas.
> ```powershell
>    Connect-MgGraph -Scopes "User.Read","User.ReadWrite"
> ```

Use o seguinte comando, onde você substitui `$OrgID` pelo ID da sua organização e especifica `-IsEnabledInOrganization` como `false`.
```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $OrgID -IsEnabledInOrganization:$false
```
Como alternativa, você pode alterar o padrão e desabilitar as informações do item para um grupo específico do Microsoft Azure AD. Use o seguinte comando, onde você substitui `$OrgID` pela ID da sua organização e `$GroupID` como a ID do grupo do Microsoft Azure AD.
```powershell
   Update-MgOrganizationSettingItemInsight -OrganizationId $OrgID -DisabledForGroup $GroupId
```

### <a name="configure-item-insights-using-rest-api"></a>Configurar as informações do item usando a API REST
Conforme declarado anteriormente, por padrão, as configurações de privacidade das informações do item são habilitadas para toda a organização. Você pode alterar o padrão de duas maneiras:

- Desabilite as informações do item para todos os usuários na organização, definindo a propriedade **isEnabledInOrganization** do recurso [itemInsightsSettings](/graph/api/resources/iteminsightssettings?view=graph-rest-beta&preserve-view=true) como `false`. 
- Desabilite as informações do item para um _subconjunto_ de usuários, atribuindo esses usuários em um grupo do Microsoft Azure AD e definindo a propriedade **disabledForGroup** como a ID do grupo. Saiba mais sobre o [criar um grupo e adicionar usuários como membros](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Use a operação de [atualização](/graph/api/iteminsightssettings-update?view=graph-rest-beta&preserve-view=true) para definir as propriedades **isEnabledInOrganization** e **disabledForGroup** de acordo.

| Como as informações do item são habilitadas | isEnabledInOrganization | disabledForGroup |
|:-------------|:------------|:------------|
| Toda a organização (padrão) | `true` | vazio |
| Desabilitado para um subconjunto de usuários na organização | `true` | ID do grupo do Azure AD que contém o subconjunto de usuários |
| Desabilitado para toda a organização | `false` | ignorado |

Lembre-se do seguinte ao atualizar as configurações de informações do item:
- [As configurações de informações do item](/graph/api/resources/iteminsightssettings?view=graph-rest-beta&preserve-view=true) estão disponíveis apenas no ponto de extremidade beta.
- Obtenha a ID de um grupo do Azure AD no portal do Azure e verifique se o grupo existe, porque a operação de atualização não verifica a existência do grupo. Especificar um grupo inexistente no **disabledForGroup** _não_ desabilita as informações para todos os usuários da organização.
- A atualização das configurações pode levar até oito horas para ser aplicada a todas as experiências da Microsoft 365.
- Independentemente das configurações de informações do item, o Delve continua a respeitar as [configurações de privacidade](/sharepoint/delve-for-office-365-admins#control-access-to-delve-and-related-features?view=graph-rest-beta&preserve-view=true) do locatário e do usuário do Delve.


## <a name="behavior-changes-in-ui-and-apis"></a>O comportamento é alterado na IU e nas APIs
Algumas informações de [tendências](/graph/api/resources/insights-trending) ou [usadas](/graph/api/resources/insights-used) ideias podem ser afetadas conforme descrito abaixo. Ao longo do tempo, o escopo e os tipos dessas informações serão estendidos. 

- O cartão de perfil de um usuário que tiver desabilitado as informações do item não mostra seus documentos **usados**. A mesma limitação se aplica ao resultado do perfil da Pesquisa da Microsoft no Bing, em que o painel **Arquivos Recentes** fica vazio. Além disso, a precisão de expansão de acrônimo na pesquisa é reduzida.

- A desativação dos insights do item irá parar[horário de reunião sugerido](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1?ui=en-US&rs=en-US&ad=US)de ser calculado e mostrado ao usuário em seu cartão de perfil. 

- No Delve, um usuário que desabilitou as informações do item tem seus documentos ocultos. 

- Todos os usuários que desativarem as informações do item terão suas atividades removidas da análise de toda a organização. Normalmente, tal análise sugere informações assistenciais para os colegas do usuário em diversas experiências, desde o Outlook até o OneDrive e o SharePoint. A análise é sempre anônima independentemente das configurações, mas quando um usuário desabilita as informações, a atividade do usuário é excluída da melhoria da produtividade de outras pessoas.

- Para um usuário que tenha desabilitado as informações do item, a consulta de recursos de [tendências](/graph/api/resources/insights-trending) e [usados](/graph/api/resources/insights-used)na API do Microsoft Graph retorna `HTTP 403 Forbidden`.

- Onde a seção **Descobrir** é habilitada para um usuário que pesquisa no Outlook Mobile, desabilitar as informações do item para esse usuário ocultaria, na seção **Descobrir**, documentos populares para ele. Caso contrário, os documentos populares são recomendados e exibidos com base em outras atividades do usuário.


## <a name="transition-period"></a>Período de transição
Para acomodar a configuração das informações do item, até o final de 2020, o Microsoft 365 respeitará as configurações do Delve e das informações sobre o item e aplicará o mais estrito, caso elas sejam diferentes. Isso significa que um usuário é considerado como excluído das informações do item, se o usuário tiver optado por excluir os controles do Delve ou as configurações de informações do item.

Após esse período de transição, as configurações do Delve controlarão apenas a experiência do Delve, e as configurações de informações do item afetarão apenas as informações do item do Microsoft Graph. Certifique-se de configurar as informações do item de acordo com os requisitos da sua organização.


> [!NOTE]
> Durante o período de transição, devido a motivos técnicos, a página inicial do SharePoint poderá fornecer sugestões obsoletas se uma organização desabilitar as informações do item para todos os usuários. Esse problema será corrigido em futuras alterações do lado do servidor. 

## <a name="see-also"></a>Confira também
Saiba mais sobre o Delve e como usar as configurações de recursos do Delve para controlar os documentos que aparecem no feed **Discover**: 
- [Conectar-se e colaborar no Office Delve](https://support.microsoft.com/office/connect-and-collaborate-in-office-delve-46f92806-b52c-4187-b60e-b3bf8d25f73e)
- [Meus documentos estão seguros no Office Delve?](https://support.microsoft.com/office/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3)
- [Delve para administradores](/sharepoint/delve-for-office-365-admins)