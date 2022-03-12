---
title: Tipo de recurso de configurações do usuário (UserSettings)
description: 'As atuais configurações de usuário para descoberta de conteúdo. '
author: jpettere
ms.localizationpriority: medium
ms.prod: users
doc_type: resourcePageType
ms.openlocfilehash: 64454a7004946d354e83467d94aa5148438791e6
ms.sourcegitcommit: 6950d15d8cce5e04733738b8debb92cd8c1d63fe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/12/2022
ms.locfileid: "63451456"
---
# <a name="usersettings-resource-type"></a>Tipo de recurso de configurações do usuário (UserSettings)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Configurações que representam as preferências de um usuário para o seguinte:
- Acesso ao Delve
- [Insights de item](../resources/officegraphinsights.md)
- [Localidade regional e idiomas](../resources/regionalandlanguagesettings.md)
- [Agendamento de turnos](../resources/shiftpreferences.md)
- [Sugestões para mesclar contatos duplicados](../resources/contactmergesuggestions.md).

Gerenciar Delve acessibilidade:
  - Verificar se um usuário e a organização do usuário têm acesso a Office Delve.
  - Desabilitando ou habilitando documentos em Office Delve para usuários específicos. 

Configure a visibilidade dos [insights de itemInsights](../resources/iteminsights.md) e [de horas de reunião](https://support.microsoft.com/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1). ItemInsights são derivados entre usuários e outros itens (como documentos ou sites) em Microsoft 365:
  - Verificando se os insights de item e horário de reunião de um usuário estão habilitados.
  - Desabilitando ou habilitando informações de item e horas de reunião para um usuário específico.

Gerenciar as preferências baseadas na localidade do usuário: 
  - Determinando com qual idioma e formatação regional um usuário prefere exibir aplicativos.
  - Atualizando o idioma de um usuário e as preferências de formatação regional.

Gerenciar as preferências de turno de trabalho do usuário: 
  - Verificar se um usuário pode ser atribuído a turnos em um cronograma.
  - Atualizando as preferências de turno de um usuário.
  
Configurar [contactMergeSuggestions](../resources/contactmergesuggestions.md):
  - Determinar se a sugestão para mesclar contatos duplicados para um usuário está habilitada.
  - Desabilitando ou habilitando sugestões para mesclar contatos duplicados para um usuário.

Herda de [entidade](entity.md). Para saber como obter ou atualizar as configurações de usuário, confira [Obter configurações](../api/usersettings-get.md) e [Atualizar configurações](../api/usersettings-update.md).

> [!NOTE]
> Esse ponto de extremidade funciona apenas com o [recurso do](user.md) usuário. 

## <a name="methods"></a>Métodos
| Método       | Tipo de retorno  |Descrição|
|:---------------|:--------|:----------|
|[Obter configurações de usuário](../api/usersettings-get.md) |[userSettings](../resources/usersettings.md)| Obter as configurações de usuário e da organização. |
|[Atualizar as configurações de usuário](../api/usersettings-update.md) |[userSettings](../resources/usersettings.md)| Atualize as configurações do usuário atual. |

## <a name="properties"></a>Propriedades

| Propriedade     | Tipo   |Descrição|
|:---------------|:--------|:----------|
|contributionToContentDiscoveryDisabled|Booliano|Os documentos do usuário do Office Delve serão desativados quando definidos como verdadeiros. Os usuários podem controlar essa configuração em [Office Delve](https://support.office.com/article/are-my-documents-safe-in-office-delve-f5f409a2-37ed-4452-8f61-681e5e1836f3?ui=en-US&rs=en-US&ad=US#bkmk_optout). |
|contributionToContentDiscoveryAsOrganizationDisabled|Booliano|Reflete a configuração [Office Delve nível da organização](https://support.office.com/article/office-delve-for-office-365-admins-54f87a42-15a4-44b4-9df0-d36287d9531b#bkmk_delveonoff). A organização não tem acesso ao Office Delve quando definido como verdadeiro. Essa configuração é somente leitura e pode ser alterada somente por administradores no [Centro de administração do SharePoint](https://support.office.com/article/about-the-office-365-admin-center-758befc4-0888-4009-9f14-0d147402fd23?ui=en-US&rs=en-US&ad=US).|
|id|Cadeia de caracteres|Identificador exclusivo da configuração do usuário. Somente leitura. Herdado da [entidade](entity.md).|

## <a name="relationships"></a>Relações

| Relação | Tipo | Descrição |
|:---------------|:--------|:----------|
|contactMergeSuggestions|[contactMergeSuggestions](contactmergesuggestions.md)| As configurações do usuário para a visibilidade da sugestão de mesclagem para os contatos duplicados na lista de contatos do usuário.|
|itemInsights|[userInsightsSettings](userinsightssettings.md)| As configurações do usuário para a visibilidade de insights de hora de reunião e percepções derivadas entre um usuário e outros itens no Microsoft 365, como documentos ou sites. [Obter userInsightsSettings](../api/userinsightssettings-get.md) por meio dessa propriedade de navegação. |
|regionalAndLanguageSettings|[regionalAndLanguageSettings](regionalandlanguagesettings.md)| Preferências do usuário para idiomas, localidade regional e formatação de data/hora. |
|shiftPreferences|[shiftPreferences](shiftpreferences.md)| As preferências de turno para o usuário. |



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


