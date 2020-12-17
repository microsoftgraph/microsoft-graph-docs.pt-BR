---
title: Revisões do Azure AD Access-associações de grupo
description: Você pode usar as revisões do Azure AD Access para configurar revisões de acesso de uso único ou recorrente para atestado dos direitos de acesso do usuário. Esta documentação serve para a 2ª versão das APIs.
localization_priority: Normal
author: isabelleatmsft
ms.prod: microsoft-identity-platform
doc_type: conceptualPageType
ms.openlocfilehash: 5c5cbe43c75e5f0ac0ea552c380b294c7725907e
ms.sourcegitcommit: ee9e594ad64bef5bc839cf813c0854d083c00aef
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/17/2020
ms.locfileid: "49705951"
---
# <a name="azure-ad-access-reviews-group-memberships"></a>Revisões do Azure AD Access (associações de grupo)

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>Esta documentação se aplica às revisões de acesso de associações de grupo. Para obter revisões de acesso em todos os outros tipos de recurso suportados, consulte [Access Reviews (All resources)](accessreviews-root.md).
>
>Atualmente, essa API só dá suporte a revisões de acesso de associações de grupo.

Você pode usar as [revisões do Azure ad Access](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar revisões de acesso de uso único ou recorrente para atestado dos direitos de acesso do usuário.

Cenários de cliente típicos para revisões de acesso de associações de grupo e acesso de aplicativo são:

- Os clientes podem revisar e certificar o acesso de usuário convidado usando revisões de acesso de seu acesso a aplicativos e associações de grupos. Os revisores podem usar os insights fornecidos para decidir de forma eficiente se os convidados devem ter acesso contínuo.

- Os clientes podem analisar e certificar o acesso do funcionário aos aplicativos e às associações de grupo com as revisões do Access.

- Os clientes podem coletar controles de revisão de acesso em programas que são relevantes para a sua organização para rastrear as revisões de conformidade ou aplicativos sensíveis a riscos.

Há também um recurso relacionado para os clientes revisar e certificar as atribuições de função de usuários administrativos atribuídos às funções do Azure AD, como administrador global ou funções de assinatura do Azure.  Esse recurso está incluído no [Gerenciamento de identidade privilegiado do Azure ad](privilegedidentitymanagement-root.md).

Observe que o recurso de revisões de acesso, incluindo a API, está incluído no Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida adquirida ou de avaliação do Azure AD Premium P2 ou EMS e5.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão do Access.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | coleção [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista cada `accessReviewScheduleDefinition` . Não inclui instâncias associadas `accessReviewInstance` em listagens. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obtenha um `accessReviewScheduleDefinition` com uma ID especificada. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Criar uma página `accessReviewScheduleDefinition`. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Excluir um `accessReviewScheduleDefinition` com uma ID especificada. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualize as propriedades de um `accessReviewScheduleDefinition` com uma ID especificada. |
|[Listar accessReviewInstance](../api/accessreviewinstance-list.md) | coleção [accessReviewInstance](accessreviewinstance.md) | Lista cada `accessReviewInstance` um específico `accessReviewScheduleDefinition` . Não inclui s associados `accessReviewInstanceDecisionItem` em listagens. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Retorna `accessReviewInstance` para um `accessReviewScheduleDefinition` . Não inclui s associados `accessReviewInstanceDecisionItem` no objeto. |
|[Listar accessReviewInstances pendente de aprovação](../api/accessreviewinstance-pendingaccessreviewinstances.md) | coleção [accessReviewInstance](accessreviewinstance.md) . | Obtenha todas as `accessReviewInstance` atribuições para o usuário de chamada. |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete para os revisores de um `accessReviewInstance` . |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Interromper manualmente um `accessReviewInstance` . |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada não revisado `accessReviewInstanceDecisionItem` que é o revisor para um específico `accessReviewInstance` . |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar manualmente a decisão em um `accessReviewInstance` . |
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Lista cada `accessReviewInstanceDecisionItem` um específico `accessReviewInstance` . |
|[Listar accessReviewInstanceDecisionItems pendente de aprovação](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | coleção [accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Obtenha todos os `accessReviewInstanceDecisionItems` atribuídos ao usuário de chamada, para um específico `accessReviewInstance` . |
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer `accessReviewInstanceDecisionItems` um dos quais o usuário de chamada tenha atribuído um revisor, o usuário de chamada pode gravar uma decisão corrigindo o objeto de decisão. |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de permissão de aplicativo e função

As funções de diretório a seguir são necessárias para um usuário de chamada gerenciar revisões do Access. Observe que, no momento, há suporte apenas para revisões de acesso em grupos por meio das APIs do Microsoft Graph.

| Operação | Permissões de aplicativos | Função de diretório necessária do usuário de chamada |
|:------------------|:------------|:--------------------------------------------|
| Ler | AccessReview. Read. All ou AccessReview. ReadWrite. All | Administrador global, leitor global, administrador de segurança, leitor de segurança ou administrador de usuários |
| Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador global ou administrador de usuário |

Além disso, um usuário que é um revisor atribuído de uma revisão do Access pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com as revisões do Azure AD Access](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com as revisões do Azure AD Access](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


<!--
{
  "type": "#page.annotation",
  "description": "Service root",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


