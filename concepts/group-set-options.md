---
title: Definir opções de provisionamento e comportamentos de grupo do Microsoft 365
description: Usando o recurso de grupo no Microsoft Graph, você pode definir comportamentos e recursos de grupo específicos para provisionar ao criar um grupo do Microsoft 365.
author: yyuank
localization_priority: Priority
ms.openlocfilehash: 9df8f3d4fadea93e45089870351531619cd2fde9
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345783"
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
| WelcomeEmailDisabled|Um email de boas-vindas é enviado para um novo membro do grupo.|Os emails de boas-vindas não são enviados para novos membros.|

**resourceProvisioningOptions** é uma coleção de cadeia de caracteres que especifica os recursos de grupo a serem provisionados como parte da criação do grupo Microsoft 365, que normalmente não fazem parte da criação de grupo padrão.

| Valores com suporte para resourceProvisioningOptions   |Descrição| Padrão se não for definido |
|:---------------|:--------|:------------|
| Teams|Provisione esse grupo como uma equipe no Microsoft Teams. Além disso, esse valor pode ser adicionado à coleção de cadeias de caracteres **resourceProvisioningOptions** na [atualização de grupo](/graph/api/group-update?view=graph-rest-beta) por meio de uma `PATCH` operação, a fim de converter um grupo existente do Microsoft 365 em uma equipe.| O grupo é um grupo normal do Microsoft 365 sem recursos do teams.|


## <a name="see-also"></a>Confira também

- [Visão geral dos grupos do Microsoft 365 no Microsoft Graph](office365-groups-concept-overview.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
