---
title: Definir opções de provisionamento e comportamentos de grupo do Microsoft 365
description: Usando o recurso de grupo no Microsoft Graph, você pode definir comportamentos e recursos de grupo específicos para provisionar ao criar um grupo do Microsoft 365.
author: yyuank
localization_priority: Priority
ms.openlocfilehash: fd276dcdc42b70f6ed3aeb2e43095e6b5d76e2d4
ms.sourcegitcommit: a1a57e803c334e11316dd571ad1b54c95406740e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/29/2020
ms.locfileid: "44413494"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a>Definir opções de provisionamento e comportamentos de grupo da Microsoft 365 (versão prévia)

Usando o recurso de [grupo](/graph/api/resources/group?view=graph-rest-beta) no Microsoft Graph, você pode definir comportamentos e recursos de grupo específicos para provisionar ao criar um grupo do Microsoft 365. Dependendo do recurso, alguns também podem ser provisionados na atualização do grupo.

### <a name="configuring-and-provisioning-groups"></a>Configurando e provisionando grupos

O recurso de **grupo** expõe duas propriedades, **resourceBehaviorOptions** e **resourceProvisioningOptions**, para personalizar os comportamentos e recursos a serem provisionados na criação de grupos. 

> [!NOTE]
> As propriedades **resourceBehaviorOptions** e **resourceProvisioningOptions** estão atualmente disponíveis somente no ponto de extremidade beta do Microsoft Graph. Não os use em aplicativos de produção, pois eles estão sujeitos a alterações sem aviso prévio.

**resourceBehaviorOptions** é uma coleção de cadeia de caracteres que especifica comportamentos de grupo para um grupo do Microsoft 365. Esses bahaviors podem ser definidos apenas na [criação de grupos](/graph/api/group-post-groups?view=graph-rest-beta) ( `POST` ).

| Valores com suporte para resourceBehaviorOptions   |Descrição|Padrão se não for definido|
|:---------------|:--------|:-----------|
| AllowOnlyMembersToPost|Somente *membros* do grupo podem postar conversas no grupo.|Todos os usuários da organização podem postar conversas no grupo.|
| HideGroupInOutlook|Esse grupo está oculto nas experiências do Outlook.|Todos os grupos são visíveis e podem ser descobertos em experiências do Outlook.|
| SubscribeNewGroupMembers|Os membros do grupo se inscreveram para receber conversas em grupo. |Os membros do grupo não recebem conversas em grupo.|
| WelcomeEmailDisabled|Os emails de boas-vindas não são enviados para novos membros.|Um email de boas-vindas é enviado para um novo membro do grupo.|

**resourceProvisioningOptions** é uma coleção de cadeia de caracteres que especifica os recursos de grupo a serem provisionados como parte da criação do grupo Microsoft 365, que normalmente não fazem parte da criação de grupo padrão.

| Valores com suporte para resourceProvisioningOptions   |Descrição| Padrão se não for definido |
|:---------------|:--------|:------------|
| Teams|Provisione esse grupo como uma equipe no Microsoft Teams. Além disso, esse valor pode ser adicionado à coleção de cadeias de caracteres **resourceProvisioningOptions** na [atualização de grupo](/graph/api/group-update?view=graph-rest-beta) por meio de uma `PATCH` operação, a fim de converter um grupo existente do Microsoft 365 em uma equipe.| O grupo é um grupo normal do Microsoft 365 sem recursos do teams.|


## <a name="see-also"></a>Confira também

- [Visão geral dos grupos do Microsoft 365 no Microsoft Graph](office365-groups-concept-overview.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
