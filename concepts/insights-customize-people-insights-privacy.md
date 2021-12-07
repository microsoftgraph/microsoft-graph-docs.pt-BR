---
title: Personalização da privacidade das percepções das pessoas no Microsoft Graph
description: Aprenda como personalizar as percepções das pessoas no nível da organização usando a API do Microsoft Graph.
author: anthona
ms.localizationpriority: high
ms.prod: insights
ms.custom: scenarios:getting-started
ms.openlocfilehash: e0495f4206023c6d7c8a46f094172e5732c08df4
ms.sourcegitcommit: f65eee432cc903324b5f9b31710fdc6100590f36
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/07/2021
ms.locfileid: "61322720"
---
# <a name="customizing-people-insights-privacy-in-microsoft-graph-preview"></a>Personalização da privacidade das percepções das pessoas no Microsoft Graph (visualização)

Os insights de pessoas representam conexões de pessoas que são [ relevantes ou trabalham ](people-example.md#including-a-person-as-relevant-or-working-with) umas com as outras na mesma organização, com base nas relações públicas entre as pessoas. Esses insights podem ser exibidos no Delve e no cartão de perfil, e retornados pela [API de pessoas](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true).


## <a name="customizing-people-insights-for-an-organization"></a>Personalização de percepções de pessoas para uma organização

Por padrão, a exibição ou retorno de insights de pessoas está habilitado para uma organização. Os administradores com a função de administrador global podem personalizar esse comportamento para uma organização usando APIs REST e as permissões apropriadas. Eles podem personalizar definindo propriedades do recurso [insightsSettings](/graph/api/resources/insightssettings?view=graph-rest-beta&preserve-view=true) das seguintes maneiras:

- Desabilite as percepções de pessoas para todos os usuários na organização, definindo a propriedade **isEnabledInOrganization** do recurso **insightsSettings** como `false`. (Por padrão, a propriedade **isEnabledInOrganization** é `true`.)

- Desabilite as percepções de pessoas para um subconjunto de usuários, atribuindo esses usuários a um grupo do Azure Active Directory (Azure AD) e definindo a propriedade **disabledForGroup** para a ID desse grupo. Saiba mais sobre o [criar um grupo e adicionar usuários como membros](/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal). 

Use a operação [atualizar](/graph/api/insightssettings-update?view=graph-rest-beta&preserve-view=true) para definir as propriedades **isEnabledInOrganization** ou **disabledForGroup** de acordo com os insights das pessoas. 

Lembre-se do seguinte ao atualizar as configurações de informações do item: 
* As configurações de insights de pessoas estão disponíveis apenas no ponto de extremidade beta. 
* A operação de atualização não verifica se um grupo existe. Certifique-se de obter a ID correta do grupo do Azure Active Directory no portal do Azure, verifique se o grupo existe e se os usuários pretendidos foram adicionados ao grupo. Se o grupo não existir, nenhuma alteração será feita para nenhum usuário da organização. 
* A atualização de **insightsSettings** pode levar até 24 horas para que as alterações sejam refletidas e, às vezes, pode demorar mais. 

## <a name="behavior-changes-in-the-microsoft-365-ui-and-people-api"></a>Alterações de comportamento na interface de usuário do Microsoft 365 e API de pessoas 

Desabilitar as percepções de pessoas significa que os dados não são gerados para um usuário especificado. Não afeta a pesquisa e a classificação dos resultados.

Ao personalizar a privacidade para percepções de pessoas, você pode observar mudanças comportamentais nas seguintes áreas:
* Cartão de perfil do [Microsoft 365](https://support.microsoft.com/office/profile-cards-in-microsoft-365-e80f931f-5fc4-4a59-ba6e-c1e35a85b501)
* Perfil de usuário em Delve
* [Listando pessoas relevantes](/graph/api/user-list-people?view=graph-rest-beta&preserve-view=true).

