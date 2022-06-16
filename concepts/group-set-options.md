---
title: Defina os comportamentos de grupo do Microsoft 365 e opções de provisionamento
description: Use o recurso de grupo no Microsoft Graph para definir comportamentos e recursos de grupo específicos a serem provisionados ao criar um grupo do Microsoft 365.
author: psaffaie
ms.localizationpriority: high
ms.openlocfilehash: 82349bfa47d0df9ed81384bf4af4108f18726f40
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096200"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options"></a>Defina os comportamentos de grupo do Microsoft 365 e opções de provisionamento

Usando o recurso de [grupo](/graph/api/resources/group) no Microsoft Graph, você pode definir comportamentos e recursos de grupo específicos a serem provisionados ao criar um grupo do Microsoft 365. Dependendo do recurso, alguns também podem ser provisionados na atualização do grupo.

O recurso **grupo** expõe duas propriedades, **resourceBehaviorOptions** e **resourceProvisioningOptions**, para personalizar os comportamentos e recursos a serem provisionados na criação do grupo.

## <a name="configure-groups"></a>Configurar grupos

**resourceBehaviorOptions** é uma coleção de cadeia de caracteres que especifica comportamentos de grupo para um grupo do Microsoft 365. Esses comportamentos podem ser definidos apenas na [criação do grupo](/graph/api/group-post-groups) (`POST`).

| Valores com suporte para resourceBehaviorOptions | Descrição                                                  | Padrão se não for definido                                                |
| :------------------------------------------- | :----------------------------------------------------------- | :---------------------------------------------------------------- |
| AllowOnlyMembersToPost                       | Somente _membros_ do grupo podem postar conversas no grupo.    | Todos os usuários da organização podem postar conversas no grupo. |
| HideGroupInOutlook                           | Este grupo está oculto nas experiências do Outlook.                 | Todos os grupos são visíveis e detectáveis nas experiências do Outlook.   |
| SubscribeNewGroupMembers                     | Os membros do grupo se inscreveram para receber conversas em grupo. | Os membros do grupo não recebem conversas em grupo.                 |
| WelcomeEmailDisabled                         | Os emails de boas-vindas não serão enviados para novos membros.                  | Um email de boas-vindas será enviado para um novo membro do grupo.     |

## <a name="provision-groups"></a>Provisionar grupos

**resourceProvisioningOptions** é uma coleção de cadeia de caracteres que especifica os recursos do grupo a serem provisionados como parte do grupo Microsoft 365. Esses recursos podem ser especificados durante a criação ou atualização do grupo.

| Valores com suporte para resourceProvisioningOptions | Descrição                                              | Padrão se não for definido                                                |
| :----------------------------------------------- | :------------------------------------------------------- | :---------------------------------------------------------------- |
| Equipe                                             | Provisione este grupo como uma equipe no Microsoft Teams. Além disso, esse valor também pode ser adicionado na [atualização do grupo](/graph/api/group-update) por meio de uma operação `PATCH`, a fim de provisionar uma equipe de um grupo Microsoft 365 existente. | O grupo é um grupo normal do Microsoft 365 sem recursos do Teams. |

## <a name="see-also"></a>Confira também

- [Visão geral dos grupos do Microsoft 365 no Microsoft Graph](office365-groups-concept-overview.md)
- [Visão geral da API do Microsoft Teams](teams-concept-overview.md)
