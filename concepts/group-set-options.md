---
title: Defina os comportamentos de grupo do Microsoft 365 e opções de provisionamento
description: Usando o recurso de grupo no Microsoft Graph, você pode definir comportamentos e recursos de grupo específicos para provisionar ao criar um grupo do Microsoft 365.
author: yyuank
localization_priority: Priority
ms.openlocfilehash: 066ef0c65fa0b70fd89fc5dfc4cf14e047f1bc49
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034146"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a>Definir comportamentos de grupo do Microsoft 365 e opções de provisionamento (visualização)

Usando o recurso de [grupo](/graph/api/resources/group?view=graph-rest-beta) no Microsoft Graph, você pode definir comportamentos e recursos de grupo específicos a serem provisionados ao criar um grupo do Microsoft 365. Dependendo do recurso, alguns também podem ser provisionados na atualização do grupo.

### <a name="configuring-and-provisioning-groups"></a>Configurando e provisionando grupos

O recurso **grupo** expõe duas propriedades, **resourceBehaviorOptions** e **resourceProvisioningOptions**, para personalizar os comportamentos e recursos a serem provisionados na criação do grupo. 

> [!NOTE]
> As propriedades **resourceBehaviorOptions** e **resourceProvisioningOptions** estão disponíveis atualmente apenas no ponto de extremidade beta do Microsoft Graph. Não os use em aplicativos de produção, pois estão sujeitos a alterações sem aviso prévio.

**resourceBehaviorOptions** é uma coleção de cadeia de caracteres que especifica comportamentos de grupo para um grupo do Microsoft 365. Esses comportamentos podem ser definidos apenas na [criação do grupo](/graph/api/group-post-groups?view=graph-rest-beta) (`POST`).

| Valores com suporte para resourceBehaviorOptions   |Descrição|Padrão se não for definido|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|Somente *membros* do grupo podem postar conversas no grupo.|Todos os usuários da organização podem postar conversas no grupo.|
| HideGroupInOutlook|Este grupo está oculto nas experiências do Outlook.|Todos os grupos são visíveis e detectáveis nas experiências do Outlook.|
| SubscribeNewGroupMembers|Os membros do grupo se inscreveram para receber conversas em grupo. |Os membros do grupo não recebem conversas em grupo.|
| WelcomeEmailDisabled|Os emails de boas-vindas não serão enviados para novos membros.|Um email de boas-vindas será enviado para um novo membro do grupo.|

**resourceProvisioningOptions** é uma coleção de strings que especifica os recursos do grupo a serem provisionados como parte da criação do grupo Microsoft 365, que normalmente não fazem parte da criação do grupo padrão.

| Valores com suporte para resourceProvisioningOptions   |Descrição| Padrão se não for definido |
|:---------------|:--------|:------------|
| Teams|Provisione este grupo como uma equipe no Microsoft Teams. Além disso, esse valor pode ser adicionado à coleção de cadeia de caracteres **resourceProvisioningOptions** na [atualização do grupo](/graph/api/group-update?view=graph-rest-beta) por meio de uma operação `PATCH`, a fim de converter um grupo existente do Microsoft 365 em uma equipe.| O grupo é um grupo normal do Microsoft 365 sem recursos do Teams.|


## <a name="see-also"></a>Confira também

- [Visão geral dos grupos do Microsoft 365 no Microsoft Graph](office365-groups-concept-overview.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
