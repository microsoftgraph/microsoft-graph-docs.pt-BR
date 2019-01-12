---
title: tipo de recurso de configurações
description: 'As configurações do usuário atual. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 7beddf0c0ac1d6279d5e6e53b8a87844f19efba6
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967970"
---
# <a name="settings-resource-type"></a>tipo de recurso de configurações

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

As configurações do usuário atual. Para saber como obter ou atualizar as configurações de usuário, consulte [obter configurações](../api/user-get-settings.md) e [configurações de atualização](../api/user-update-settings.md).

Esse recurso permite:

- Verificando se um usuário e a organização do usuário contribuem para detecção de conteúdo.
- Desativando ou habilitando a descoberta de conteúdo para usuários específicos. Isso também desabilita documentos no Office me aprofundar.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter configurações de usuário](../api/user-get-settings.md) |[Configurações](../resources/user-settings.md)| Obtenha as configurações de usuário e da organização. |
|[Atualizar configurações de usuário](../api/user-update-settings.md) |[Configurações](../resources/user-settings.md)| Atualize as configurações de usuário atual. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Booliano|API [de tendências](insights-trending.md) quando definido como true, o acesso de representante para o usuário está desabilitado. Quando definido como true, documentos no Office de me aprofundar o usuário estão desabilitadas. Quando definido como true, a relevância do conteúdo exibido no Office 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business é afetado. Os usuários podem controlar essa configuração no [Office me aprofundar](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Booliano|Reflete a [configuração de nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlar o acesso de representante para a [análise de tendências](insights-trending.md) API. Quando definido como true, a organização não tem acesso ao Office me aprofundar. A relevância do conteúdo exibido no Office 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de descoberta no OneDrive for Business será afetada para toda a organização. Essa configuração é somente leitura e só pode ser alterada pelos administradores, no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
