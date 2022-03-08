---
title: Revisões de acesso ao Azure AD
description: Você pode usar as análises de acesso do Azure AD para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário. Esta documentação atende à versão 2nd das APIs.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 580d1299503924486dab1be11c33e8f771592baa
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/08/2022
ms.locfileid: "63336057"
---
# <a name="azure-ad-access-reviews"></a>Revisões de acesso ao Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Use as análises de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar análises de acesso única ou recorrentes para atestar os direitos dos usuários para acessar recursos do Azure AD. Esses recursos do Azure AD incluem grupos, entidades de serviço, pacotes de acesso e funções privilegiadas.

Cenários típicos do cliente para análises de acesso incluem:

- Os clientes podem revisar e certificar o acesso de usuários convidados a grupos por meio de associações de grupo. Os revisadores podem usar as informações fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.
- Os clientes podem revisar e certificar o acesso dos funcionários aos recursos do Azure AD.
- Os clientes podem revisar e auditar atribuições para funções privilegiadas do Azure AD. Isso dá suporte a organizações no gerenciamento de acesso privilegiado.

Observe que o recurso de críticas de acesso, incluindo a API, está incluído Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida comprada ou de avaliação Azure AD Premium P2 ou EMS E5. Para obter mais informações sobre os requisitos de licença, consulte [Requisitos de licença de revisão do Access](/azure/active-directory/governance/access-reviews-overview#license-requirements).


## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|**Agendar definições**| | |
|[Definições de lista](../api/accessreviewset-list-definitions.md) | [Coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter uma lista dos [objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) e suas propriedades. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um objeto accessReviewScheduleDefinition e suas propriedades. |
|[Criar definições](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Exclua um accessReviewScheduleDefinition. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de um accessReviewScheduleDefinition com um identificador especificado. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário de chamada é um revistor em uma ou mais instâncias.|
|**Instâncias**| | |
|[List instances](../api/accessreviewscheduledefinition-list-instances.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Leia as propriedades e as relações de um [objeto accessReviewInstance](../resources/accessreviewinstance.md) . |
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar decisões manualmente em um accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Nenhum|Revise lotes de entidades ou recursos em uma chamada.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Nenhum|Redefine todos os itens de decisão em uma instância para `notReviewed`.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todas as instâncias em um [determinado accessReviewScheduleDefinition](accessreviewscheduledefinition.md) para o qual o usuário de chamada é o revisor de uma ou mais decisões.|
|**Itens de decisão de instância**| | |
|[Listar decisões](../api/accessreviewinstance-list-decisions.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Obter uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Recupera todos os [objetos accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) onde o uso de chamada é o revisor de um [determinado accessReviewInstance](accessreviewinstance.md).|
|[listPendingApproval](../api/accessreviewinstancedecisionitem-listpendingapproval.md) (preterido) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico. Este método está sendo preterido e substituído por [accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |
|**Definições de histórico**| | |
|[Histórico da listaDefinitions](../api/accessreviewset-list-historydefinitions.md)|[Coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Obter uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.|
|[Criar historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Crie um novo [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Obter accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Leia as propriedades e as relações de [um objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Gere um URI para uma instância que pode ser usada para recuperar dados de histórico de revisão.|
|[List instances](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Recupere uma lista dos [objetos accessReviewHistoryInstance](accessreviewhistoryinstance.md) e suas propriedades.|
|**Política**| | |
|[Obter accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Leia as propriedades e as relações de um [objeto accessReviewPolicy](../resources/accessreviewpolicy.md) .|
|[Atualizar accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Atualize as propriedades de [um objeto accessReviewPolicy](../resources/accessreviewpolicy.md) .|
|[Listar definições pendentes de aprovação](../api/accessreviewscheduledefinition-filterbycurrentuser.md) (preterida)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário de chamada é um revistor em uma ou mais instâncias. Este método está sendo preterido e substituído por [accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md).|
|[Lista pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) (preterido) | [Coleção accessReviewInstance](accessreviewinstance.md) . | Obter todos os recursos de accessReviewInstance pendentes atribuídos ao usuário de chamada. Este método está sendo preterido e substituído por [accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de função e permissão de aplicativo

As seguintes [funções do Azure AD](/azure/active-directory/roles/permissions-reference) são necessárias para que um usuário de chamada gerencie as críticas de acesso.

| Operação | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Ler | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
| Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuário |

Além disso, um usuário que é um revistor atribuído de uma revisão de acesso pode gerenciar suas decisões, sem precisar estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Tutoriais](/graph/accessreviews-overview) para saber como usar a API de avaliações de acesso para revisar o acesso aos recursos do Azure AD
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

