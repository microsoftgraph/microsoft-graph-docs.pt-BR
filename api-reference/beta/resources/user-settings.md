---
title: tipo de recurso configurações
description: 'As configurações do usuário atual. '
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 208d232af609f92d5924267ae26831b9929e357a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554258"
---
# <a name="settings-resource-type"></a>tipo de recurso configurações

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

As configurações do usuário atual. Para saber como obter ou atualizar as configurações do usuário, consulte [Get Settings](../api/user-get-settings.md) and [Update Settings](../api/user-update-settings.md).

Esse recurso permite:

- Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.
- Desabilitar ou habilitar a descoberta de conteúdo para usuários específicos. Isso também desabilita documentos no Office Delve.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter configurações do usuário](../api/user-get-settings.md) |[settings](../resources/user-settings.md)| Obter as configurações do usuário e da organização. |
|[Atualizar configurações do usuário](../api/user-update-settings.md) |[settings](../resources/user-settings.md)| Atualize as configurações atuais do usuário. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Booliano|Quando definido como true, o acesso de representante para a API de [tendência](insights-trending.md) do usuário é desabilitado. Quando definido como true, os documentos no Office Delve do usuário estão desabilitados. Quando definido como true, a relevância do conteúdo exibido no Office 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business são afetados. Os usuários podem controlar essa configuração no [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Booliano|Reflete a [configuração de nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) que controla o acesso de representante à API de [tendência](insights-trending.md) . Quando definido como true, a organização não tem acesso ao Office Delve. A relevância do conteúdo exibido no Office 365, por exemplo, em sites sugeridos na página inicial do SharePoint e o modo de exibição de descoberta no OneDrive for Business, é afetada para toda a organização. Essa configuração é somente leitura e só pode ser alterada por administradores no centro de [Administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.

```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/user-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
