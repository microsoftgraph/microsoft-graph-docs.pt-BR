---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 862316ba98cab7ccbbaa1c6f7cc909924e400d59
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533421"
---
# <a name="usersettings-resource-type"></a>Tipo de recurso de configurações do usuário (UserSettings)

Namespace: microsoft.graph

As atuais configurações de usuário para descoberta de conteúdo.
Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).

Esse recurso permite:

- Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.
- Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos. Isso também desabilita documentos no Office Delve.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter configurações de usuário](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| Obter as configurações de usuário e da organização. |
|[Atualizar as configurações de usuário](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| Atualize as configurações do usuário atual. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Booliano|O acesso delegado à API [mais popular](/graph/api/resources/insights-trending?view=graph-rest-beta) do usuário é desabilitada quando definido como verdadeiro. Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros. A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada quando definida como verdadeira. Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Booliano|Reflete a [configuração do nível de organização](https://support.office.com/pt-BR/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](/graph/api/resources/insights-trending?view=graph-rest-beta). A organização não tem acesso ao Office Delve quando definido como verdadeiro. A relevância do conteúdo exibido no Office 365, como em sites Sugeridos na Página Inicial do SharePoint e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização. Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|


## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
