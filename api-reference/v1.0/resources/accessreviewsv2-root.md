---
title: Revisões de acesso ao Azure AD
description: Use as análises de acesso do Azure AD para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário aos recursos do Azure AD.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: e3f43f4ff8ebe464814e6b6c68fec7b1d7c71fd724e81ca8998bd5230e7f3f8a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54180891"
---
# <a name="azure-ad-access-reviews"></a>Revisões de acesso ao Azure AD

Namespace: microsoft.graph


Use as análises de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário aos recursos do Azure AD.

Cenários de cliente típicos para análises de acesso de associações de grupo e de aplicativos e acesso a função do Azure AD são:

- Os clientes podem revisar e certificar o acesso do usuário convidado a aplicativos, funções do Azure AD e associações de grupos. Os revisadores podem usar as informações fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.

- Os clientes podem revisar e certificar o acesso de funcionários a aplicativos, funções do Azure AD e associações de grupo com avaliações de acesso.

O recurso de críticas de acesso, incluindo a API, está disponível apenas com uma licença válida de compra ou avaliação da assinatura Azure AD Premium P2 ou EMS E5.


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Obter uma lista dos [objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) e suas propriedades.|
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Crie um novo [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Leia as propriedades e as relações de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md)|[accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Atualize as propriedades de [um objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md)|None|Exclui um [objeto accessReviewScheduleDefinition.](../resources/accessreviewscheduledefinition.md)|
|[accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Retorna todas as definições em que o usuário de chamada é o revistor de qualquer instância.|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades.|
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md)|[accessReviewInstance](../resources/accessreviewinstance.md)|Leia as propriedades e as relações de um [objeto accessReviewInstance.](../resources/accessreviewinstance.md)|
|[accessReviewInstance: stop](../api/accessreviewinstance-stop.md)|None|Pare manualmente um accessReviewInstance.|
|[accessReviewInstance: sendReminder](../api/accessreviewinstance-sendreminder.md)|None|Envie um lembrete aos revisores de um accessReviewInstance.|
|[accessReviewInstance: resetDecisions](../api/accessreviewinstance-resetdecisions.md)|None|Redefine todos os itens de decisão em uma instância para `notReviewed`|
|[accessReviewInstance: applyDecisions](../api/accessreviewinstance-applydecisions.md)|None|Aplicar manualmente a decisão em um accessReviewInstance.|
|[accessReviewInstance: acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md)|None| Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico.|
|[accessReviewInstance: batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|None|Revise lotes de entidades ou recursos em uma chamada.|
|[accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todos os objetos de instância em uma definição para a qual o usuário de chamada é o revistor.|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Obter uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Atualize as propriedades de [um objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Retorna os itens de decisão dos quais o usuário de chamada é o revistor.|


## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de função e permissão de aplicativo

As seguintes funções de diretório são necessárias para que um usuário de chamada gerencie as análises de acesso. 

| Operation | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Ler | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
| Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuário |

Além disso, um usuário que é um revistor atribuído de uma revisão de acesso pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Como um administrador pode gerenciar o acesso do usuário com análises de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com análises de acesso ao Azure AD](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)
