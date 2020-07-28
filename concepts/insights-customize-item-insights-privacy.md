---
title: Personalizando a privacidade das informações do item no Microsoft Graph
description: ''
author: simonhult
localization_priority: Priority
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: a2f4c86c5c4de0d87034e2db708adde270e1b243
ms.sourcegitcommit: 20b951f8bd245bb3a2bc7d3f5533e8619e9db084
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/27/2020
ms.locfileid: "45427491"
---
# <a name="customizing-item-insights-privacy-in-microsoft-graph-preview"></a>Personalizando a privacidade das informações do item no Microsoft Graph (visualização)

As configurações de privacidade das informações do item oferecem a capacidade de configurar a visibilidade das informações derivadas do Microsoft Graph, entre usuários e outros itens (como documentos ou sites) no Microsoft 365. Você pode desabilitar o aplicativo Delve por meio dos controles pré-existentes, mas permitir que outras experiências baseadas em informações continuem fornecendo assistência.

## <a name="background"></a>Histórico
Na época do primeiro lançamento, em 2014, o Office Graph era um serviço de back-end para o Delve. Eles compartilhavam um conjunto de controles de privacidade sobre as informações do Office Graph e a experiência do usuário do Delve. Desde então, o Office Graph evoluiu e se tornou mais independente e eficiente, como parte de todas as experiências da Microsoft 365 e do Microsoft Graph. Para oferecer um esquema coerente do Microsoft Graph, a Microsoft introduziu uma entidade [itemInsights](/graph/api/resources/itemInsights?view=graph-rest-beta), que herda todas as propriedades do recurso [officeGraphInsights](/graph/api/resources/officegraphinsights?view=graph-rest-beta) pré-existente, e mantém o **officeGraphInsights**para obter uma compatibilidade com versões anteriores. A introdução de **itemInsights** também desassocia a história de privacidade das duas partes independentes.  

Embora os aplicativos existentes possam continuar a usar o **officeGraphInsights**, esses aplicativos devem ser atualizados para **itemInsights** para obter a flexibilidade de ajustar as informações do item no Office Graph e no Delve.

## <a name="how-to-customize-item-insights"></a>Como personalizar as informações do item?
Por padrão, as informações do item estão habilitadas para uma organização. Para desabilitar as informações do item para todos os usuários da organização, defina a propriedade **isEnabledInOrganization** como `false`. Para desabilitar informações do item para um _subconjunto_ de usuários em um grupo do Azure AD, defina a propriedade **disabledForGroup** como a ID do grupo. Saiba mais sobre [criar um grupo e adicionar usuários como membros](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Essas configurações oferecem flexibilidade para que os administradores usem as ferramentas do Azure AD e desabilitem as informações do item somente para os membros do grupo especificado, não necessariamente para a organização. Configure cada uma dessas propriedades [atualizando as configurações de informações do item](/graph/api/iteminsightssettings-update?view=graph-rest-beta) em um aplicativo, no PowerShell ou em outros aplicativos com permissões pendentes.

Lembre-se de que a _função de administrador global_ é necessária para ler ou atualizar essas configurações. 

### <a name="available-configurations"></a>Configurações disponíveis
Configure as configurações de informações do item para os usuários em uma organização [atualizando](/graph/api/iteminsightssettings-update?view=graph-rest-beta) as propriedades **isEnabledInOrganization** e **disabledForGroup** de acordo.

| Como as informações do item são habilitadas | isEnabledInOrganization | disabledForGroup |
|:-------------|:------------|:------------|
| Toda a organização (padrão) | `true` | vazio |
| Desabilitado para um subconjunto de usuários na organização | `true` | ID do grupo do Azure AD que contém o subconjunto de usuários |
| Desabilitado para toda a organização | `false` | ignorado |

Lembre-se do seguinte ao atualizar as configurações de informações do item:
- As configurações de privacidade de informações do item ( recurso**itemInsightsSettings**) só estão disponíveis no ponto de extremidade beta.
- Obtenha a ID de um grupo do Azure AD no portal do Azure e verifique se o grupo existe, porque a operação de atualização não verifica a existência do grupo. Especificar um grupo inexistente no **disabledForGroup** _não_ desabilita as informações para todos os usuários da organização.
- A atualização das configurações pode levar até oito horas para ser aplicada a todas as experiências da Microsoft 365.
- Independentemente das configurações de informações do item, o Delve continua a respeitar as [configurações de privacidade](/sharepoint/delve-for-office-365-admins#control-access-to-delve-and-related-features?view=graph-rest-beta) do locatário e do usuário do Delve.


## <a name="behavior-changes-in-ui-and-apis"></a>O comportamento é alterado na IU e nas APIs
Algumas informações de [tendências](/graph/api/resources/insights-trending) ou [usadas](/graph/api/resources/insights-used) ideias podem ser afetadas conforme descrito abaixo. Ao longo do tempo, o escopo e os tipos dessas informações serão estendidos. 

- O cartão de perfil de um usuário que tiver desabilitado as informações do item não mostra seus documentos **usados**. A mesma limitação se aplica ao resultado do perfil da Pesquisa da Microsoft no Bing, em que o painel **Arquivos Recentes** fica vazio. Além disso, a precisão de expansão de acrônimo na pesquisa é reduzida.

- No Delve, um usuário que desabilitou as informações do item tem seus documentos ocultos. 

- Todos os usuários que desativarem as informações do item terão suas atividades removidas da análise de toda a organização. Normalmente, tal análise sugere informações assistenciais para os colegas do usuário em diversas experiências, desde o Outlook até o OneDrive e o SharePoint. A análise é sempre anônima independentemente das configurações, mas quando um usuário desabilita as informações, a atividade do usuário é excluída da melhoria da produtividade de outras pessoas.

- Para um usuário que tenha desabilitado as informações do item, a consulta de recursos de [tendências](/graph/api/resources/insights-trending) e [usados](/graph/api/resources/insights-used)na API do Microsoft Graph retorna `HTTP 403 Forbidden`.


## <a name="transition-period"></a>Período de transição
Para acomodar a configuração das informações do item, até o final de 2020, o Microsoft 365 respeitará as configurações do Delve e das informações sobre o item e aplicará o mais estrito, caso elas sejam diferentes. Isso significa que um usuário é considerado como excluído das informações do item, se o usuário tiver optado por excluir os controles do Delve ou as configurações de informações do item.

Após esse período de transição, as configurações do Delve controlarão apenas a experiência do Delve, e as configurações de informações do item afetarão apenas as informações do item do Microsoft Graph. Certifique-se de configurar as informações do item de acordo com os requisitos da sua organização.


> [!NOTE]
> Durante o período de transição, devido a motivos técnicos, a página inicial do SharePoint poderá fornecer sugestões obsoletas se uma organização desabilitar as informações do item para todos os usuários. Esse problema será corrigido em futuras alterações do lado do servidor. 
