---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 12c75691b5b0515fbf8ef49b54ce1e4a0b806c2c
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761769"
---
# <a name="usersettings-resource-type"></a>Tipo de recurso de configurações do usuário (UserSettings)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações que representam as preferências de um usuário para localidade [regional](../resources/regionalandlanguagesettings.md)e idiomas, para agendamento de turnos [e](../resources/shiftpreferences.md)para informações e descoberta de [conteúdo.](../resources/officegraphinsights.md)

Gerenciar as preferências baseadas na localidade do usuário: 
  - Determinando com qual idioma e formatação regional um usuário prefere exibir aplicativos.
  - Atualizando o idioma de um usuário e as preferências de formatação regional.

Gerenciar as preferências de turno de trabalho do usuário: 
  - Verificar se um usuário pode ser atribuído a turnos em um cronograma.
  - Atualizando as preferências de turno de um usuário.
  
Habilitar a descoberta de conteúdo e informações centradas em documentos:
  - Verificar se um usuário e a organização do usuário contribuem para a descoberta de conteúdo.
  - Habilitar ou desabilitar a descoberta de conteúdo para usuários específicos. Isso também desabilita documentos no Office Delve.

Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).

> [!NOTE]
> Esse ponto de extremidade só funciona com usuários. Você não pode usar esse ponto de extremidade com os contatos.

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter configurações de usuário](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| Obter as configurações de usuário e da organização. |
|[Atualizar as configurações de usuário](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| Atualize as configurações do usuário atual. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Booliano|O acesso delegado à API [mais popular](insights-trending.md) do usuário é desabilitada quando definido como verdadeiro. Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros. Quando definida como verdadeira, a relevância do conteúdo exibido no Microsoft 365, como em sites Sugeridos na Página Inicial do Microsoft Office SharePoint Online e o modo de exibição Descobrir no OneDrive for Business é afetada. Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/en-us/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Booliano|Reflete a [configuração do nível de organização](https://support.office.com/en-us/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff) controlando o acesso delegado à API [mais popular](insights-trending.md). A organização não tem acesso ao Office Delve quando definido como verdadeiro. A relevância do conteúdo exibido no Microsoft 365, como em sites Sugeridos na Página Inicial do Microsoft Office SharePoint Online e o modo de exibição Descobrir no OneDrive for Business é afetada para toda a organização. Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|shiftPreferences|[shiftPreferences](shiftpreferences.md)| As preferências de turno para o usuário. |
|regionalAndLanguageSettings|[regionalAndLanguageSettings](regionalandlanguagesettings.md)| Preferências do usuário para idiomas, localidade regional e formatação de data/hora. |

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userSettings",
  "baseType": "microsoft.graph.entity"
}-->
```json
{
  "contributionToContentDiscoveryDisabled": false,
  "contributionToContentDiscoveryAsOrganizationDisabled": false
}

```


