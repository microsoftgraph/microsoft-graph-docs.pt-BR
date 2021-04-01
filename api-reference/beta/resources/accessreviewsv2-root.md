---
title: Revisões de acesso ao Azure AD
description: Você pode usar as análises de acesso do Azure AD para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário. Esta documentação atende à versão 2nd das APIs.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 931541b6f730c0ed52168b4cf3dfef4e927d808a
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473420"
---
# <a name="azure-ad-access-reviews"></a>Revisões de acesso ao Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Você pode usar as análises de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário.

Cenários de cliente típicos para análises de acesso de associações de grupo e acesso a aplicativos são:

- Os clientes podem revisar e certificar o acesso de usuários convidados usando análises de acesso de seu acesso a aplicativos e associações de grupos. Os revisadores podem usar as informações fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.

- Os clientes podem revisar e certificar o acesso de funcionários a aplicativos e associações de grupo com avaliações de acesso.

- Os clientes podem coletar controles de revisão de acesso em programas que são relevantes para sua organização acompanhar análises de conformidade ou aplicativos sensíveis a riscos.

Há também um recurso relacionado para que os clientes revisem e certifiquem as atribuições de função de usuários administrativos que são atribuídas a funções do Azure AD, como Administrador Global ou funções de assinatura do Azure.  Esse recurso está incluído no [Azure AD Privileged Identity Management](privilegedidentitymanagement-root.md).

Observe que o recurso de críticas de acesso, incluindo a API, está incluído no Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida comprada ou avaliação do Azure AD Premium P2 ou EMS E5.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-list.md) | [Coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Lista cada `accessReviewScheduleDefinition` . Não inclui `accessReviewInstance` instâncias associadas em listagem. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um `accessReviewScheduleDefinition` com uma id especificada. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-create.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Criar uma página `accessReviewScheduleDefinition`. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | `accessReviewScheduleDefinition`Exclua um com uma ID especificada. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de `accessReviewScheduleDefinition` um com uma ID especificada. |
|[Listar accessReviewInstance](../api/accessreviewinstance-list.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Lista cada `accessReviewInstance` um para um específico `accessReviewScheduleDefinition` . Não inclui s associados `accessReviewInstanceDecisionItem` em listagem. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Retorna `accessReviewInstance` para `accessReviewScheduleDefinition` um . Não inclui `accessReviewInstanceDecisionItem` s associados no objeto. |
|[Listar accessReviewInstances aguardando aprovação](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [Coleção accessReviewInstance.](accessreviewinstance.md) | Obter todos `accessReviewInstance` atribuídos ao usuário de chamada. |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisadores de um `accessReviewInstance` . |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um `accessReviewInstance` . |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada NotReviewed em que ele é o revisor `accessReviewInstanceDecisionItem` para um `accessReviewInstance` específico . |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar manualmente a decisão em `accessReviewInstance` um . |
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Lista cada `accessReviewInstanceDecisionItem` um para um específico `accessReviewInstance` . |
|[Listar accessReviewInstanceDecisionItems aguardando aprovação](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Obter todos `accessReviewInstanceDecisionItems` atribuídos ao usuário de chamada, para um `accessReviewInstance` específico . |
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer um em que o usuário de chamada recebe um revistor, chamar o usuário pode registrar uma decisão corrigindo `accessReviewInstanceDecisionItems` o objeto decision. |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de função e permissão de aplicativo

As seguintes funções de diretório são necessárias para que um usuário de chamada gerencie as análises de acesso. Observe que apenas as avaliações de acesso em grupos são suportadas atualmente por meio de APIs do Microsoft Graph.

| Operação | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Ler | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
| Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuário |

Além disso, um usuário que é um revistor atribuído de uma revisão de acesso pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com análises de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com análises de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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


