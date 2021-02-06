---
title: Revisões de acesso do Azure AD – associações de grupo
description: Você pode usar as revisões de acesso do Azure AD para configurar revisões de acesso única ou recorrentes para atestado dos direitos de acesso do usuário. Esta documentação atende à segunda versão das APIs.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: b26bd7e42746b74a14d08849e9454864512ceca8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50133396"
---
# <a name="azure-ad-access-reviews-for-groups"></a>Revisões de acesso do Azure AD para grupos

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

>[!NOTE]
>As APIs de revisão de acesso nesta seção se aplicam somente a associações de grupo. Para ver revisões de acesso em todos os outros tipos de recursos com suporte, consulte [As revisões do Access.](accessreviews-root.md)


Você pode usar as revisões de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar revisões de acesso única ou recorrentes para atestado dos direitos de acesso do usuário.

Cenários típicos de clientes para revisões de acesso de associações de grupo e acesso a aplicativos são:

- Os clientes podem revisar e certificar o acesso de usuários convidados usando revisões de acesso de seu acesso a aplicativos e associações de grupos. Os revisadores podem usar as ideias fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.

- Os clientes podem revisar e certificar o acesso dos funcionários a aplicativos e associações de grupo com revisões de acesso.

- Os clientes podem coletar controles de revisão de acesso em programas relevantes para a sua organização para rastrear análises de aplicativos de conformidade ou de risco.

Há também um recurso relacionado para que os clientes revisem e certifiquem as atribuições de função de usuários administrativos que estão atribuídos a funções do Azure AD, como Administrador Global ou funções de assinatura do Azure.  Esse recurso está incluído no [Azure AD Privileged Identity Management.](privilegedidentitymanagement-root.md)

Observe que o recurso de revisões de acesso, incluindo a API, está incluído no Azure AD Premium P2.  O locatário onde uma revisão de acesso está sendo criada deve ter uma assinatura válida adquirida ou de avaliação do Azure AD Premium P2 ou EMS E5.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com os recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | [coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista cada `accessReviewScheduleDefinition` . Não inclui instâncias `accessReviewInstance` associadas em listagem. |
|[Acessar AccessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter uma `accessReviewScheduleDefinition` com uma ID especificada. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Criar uma página `accessReviewScheduleDefinition`. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | `accessReviewScheduleDefinition`Exclua uma com uma ID especificada. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de `accessReviewScheduleDefinition` um com uma ID especificada. |
|[Listar accessReviewInstance](../api/accessreviewinstance-list.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Lista cada `accessReviewInstance` um para um específico `accessReviewScheduleDefinition` . Não inclui s `accessReviewInstanceDecisionItem` associados em listagem. |
|[Acessar AccessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Retorna `accessReviewInstance` para um `accessReviewScheduleDefinition` . Não inclui s `accessReviewInstanceDecisionItem` associados no objeto. |
|[Listar aprovação pendente de accessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [Coleção accessReviewInstance.](accessreviewinstance.md) | Obter todos `accessReviewInstance` atribuídos ao usuário chamador. |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete para os revisadores de um `accessReviewInstance` . |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um `accessReviewInstance` . |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada NotReviewed em que ele é o revisor `accessReviewInstanceDecisionItem` para um específico `accessReviewInstance` . |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar manualmente a decisão em um `accessReviewInstance` . |
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Lista cada `accessReviewInstanceDecisionItem` um para um específico `accessReviewInstance` . |
|[Listar aprovação pendente de accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Obter todos `accessReviewInstanceDecisionItems` atribuídos ao usuário de chamada, para um específico `accessReviewInstance` . |
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer um que o usuário de chamada seja atribuído a um revistor, chamar o usuário pode registrar uma decisão, corrigindo `accessReviewInstanceDecisionItems` o objeto de decisão. |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de permissão de aplicativo e função

As funções de diretório a seguir são necessárias para que um usuário chamador gerencie revisões de acesso. Observe que apenas as revisões de acesso em grupos têm suporte atualmente por meio das APIs do Microsoft Graph.

| Operation | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Ler | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
| Criar, Atualizar ou Excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuário |

Além disso, um usuário que é um revistor atribuído de uma revisão de acesso pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com revisões de acesso do Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com revisões de acesso do Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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


