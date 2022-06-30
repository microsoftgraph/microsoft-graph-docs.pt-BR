---
title: Revisões de acesso ao Azure AD
description: Você pode usar Azure AD revisões de acesso para configurar revisões de acesso única ou recorrentes para atestar os direitos de acesso do usuário. Esta documentação atende à segunda versão das APIs.
ms.localizationpriority: medium
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 141021e58e995e5939ad1dec2b915fbacfbddf21
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/29/2022
ms.locfileid: "66436607"
---
# <a name="azure-ad-access-reviews"></a>Revisões de acesso ao Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]

Use [Azure AD revisões](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) de acesso para configurar revisões de acesso única ou recorrentes para atestar os direitos dos usuários para acessar Azure AD recursos. Esses Azure AD incluem grupos, entidades de serviço, pacotes de acesso e funções privilegiadas.

Cenários típicos de clientes para revisões de acesso incluem:

- Os clientes podem examinar e certificar o acesso de usuários convidados a grupos por meio de associações de grupo. Os revisores podem usar os insights fornecidos para decidir com eficiência se os convidados devem ter acesso contínuo.
- Os clientes podem examinar e certificar o acesso de funcionários Azure AD recursos.
- Os clientes podem examinar e auditar atribuições para Azure AD funções privilegiadas. Isso dá suporte a organizações no gerenciamento de acesso privilegiado.

Observe que o recurso de revisões de acesso, incluindo a API, está incluído Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida de compra ou avaliação Azure AD Premium P2 em EMS E5. Para obter mais informações sobre os requisitos de licença, consulte [os requisitos de licença de revisões do Access](/azure/active-directory/governance/access-reviews-overview#license-requirements).

[!INCLUDE [GDPR-related-guidance](../../includes/gdpr-msgraph-export-note.md)]

## <a name="methods"></a>Métodos

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|**Definições de agendamento**| | |
|[Definições de lista](../api/accessreviewset-list-definitions.md) | [coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obtenha uma lista dos [objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) e suas propriedades. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obtenha um objeto accessReviewScheduleDefinition e suas propriedades. |
|[Criar definições](../api/accessreviewset-post-definitions.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum | Exclua um accessReviewScheduleDefinition. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum | Atualize as propriedades de um accessReviewScheduleDefinition com um identificador especificado. |
|[filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário chamador é um revisores em uma ou mais instâncias.|
|**Instâncias**| | |
|[List instances](../api/accessreviewscheduledefinition-list-instances.md) | [coleção accessReviewInstance](accessreviewinstance.md) | Obtenha uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Leia as propriedades e as relações de um [objeto accessReviewInstance](../resources/accessreviewinstance.md) . |
|[sendReminder](../api/accessreviewinstance-sendreminder.md) | Nenhum | Envie um lembrete aos revisores de um accessReviewInstance. |
|[stop](../api/accessreviewinstance-stop.md) | Nenhum | Interrompa manualmente um accessReviewInstance. |
|[acceptRecommendations](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum | Permite que o usuário chamado aceite a recomendação de decisão para cada NotReviewed accessReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[applyDecisions](../api/accessreviewinstance-applydecisions.md) | Nenhum | Aplicar decisões manualmente em um accessReviewInstance. |
|[batchRecordDecisions](../api/accessreviewinstance-batchrecorddecisions.md)|Nenhum|Examine lotes de entidades de segurança ou recursos em uma chamada.|
|[resetDecisions](../api/accessreviewinstance-resetdecisions.md)|Nenhum|Redefine todos os itens de decisão em uma instância para `notReviewed`.|
|[filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todas as instâncias em um [determinado accessReviewScheduleDefinition](accessreviewscheduledefinition.md) para o qual o usuário chamador é o revisor de uma ou mais decisões.|
|**Itens de decisão de instância**| | |
|[Listar decisões](../api/accessreviewinstance-list-decisions.md) | [coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Obtenha uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) .|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum | Para qualquer accessReviewInstanceDecisionItems ao qual o usuário chamador é atribuído a um revisor, chamar o usuário pode registrar uma decisão aplicando patch ao objeto de decisão. |
|[filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Recupera todos [os objetos accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) em que o uso de chamada é o revisor de um [determinado accessReviewInstance](accessreviewinstance.md).|
|[listPendingApproval](../api/accessreviewinstancedecisionitem-listpendingapproval.md) (preterido) | [coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) . | Obtenha todos os accessReviewInstanceDecisionItems atribuídos ao usuário chamador para um accessReviewInstance específico. Esse método está sendo preterido e substituído por [accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |
|**Definições de histórico**| | |
|[Listar historyDefinitions](../api/accessreviewset-list-historydefinitions.md)|[coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Obtenha uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.|
|[Criar historyDefinitions](../api/accessreviewset-post-historydefinitions.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Crie um novo [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[Obter accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Leia as propriedades e as relações de um [objeto accessReviewHistoryDefinition](accessreviewhistorydefinition.md) .|
|[generateDownloadUri](../api/accessreviewhistoryinstance-generatedownloaduri.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Gere um URI para uma instância que pode ser usada para recuperar dados do histórico de revisão.|
|[List instances](../api/accessreviewhistorydefinition-list-instances.md)|[accessReviewHistoryInstance](accessreviewhistoryinstance.md)|Recupere uma lista dos [objetos accessReviewHistoryInstance](accessreviewhistoryinstance.md) e suas propriedades.|
|**Política**| | |
|[Obter accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Leia as propriedades e as relações de um [objeto accessReviewPolicy](../resources/accessreviewpolicy.md) .|
|[Atualizar accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Atualize as propriedades de [um objeto accessReviewPolicy](../resources/accessreviewpolicy.md) .|
|[Listar definições com aprovação pendente](../api/accessreviewscheduledefinition-filterbycurrentuser.md) (preterido)|[coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário chamador é um revisores em uma ou mais instâncias. Esse método está sendo preterido e substituído por [accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md).|
|[Listar pendingAccessReviewInstances](../api/accessreviewinstance-pendingaccessreviewinstances.md) (preterido) | [coleção accessReviewInstance](accessreviewinstance.md) . | Obtenha todos os recursos de accessReviewInstance pendentes atribuídos ao usuário que está chamando. Esse método está sendo preterido e substituído por [accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de função e de permissão de aplicativo

As seguintes [Azure AD funções são](/azure/active-directory/roles/permissions-reference) necessárias para que um usuário chamador gerencie as revisões de acesso.

| Operation | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Leitura | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador de Usuário |
| Criar, atualizar ou excluir | AccessReview.ReadWrite.All | Administrador Global ou Administrador de Usuários |

Além disso, um usuário que é um revisador atribuído de uma revisão de acesso pode gerenciar suas decisões, sem a necessidade de estar em uma função de diretório.

## <a name="see-also"></a>Confira também

- [Tutoriais](/graph/accessreviews-overview) para saber como usar a API de revisões de acesso para examinar o acesso a Azure AD recursos
- [Como um administrador pode gerenciar o acesso do usuário com Azure AD revisões de acesso](/azure/active-directory/active-directory-azure-ad-controls-manage-user-access-with-access-reviews)
- [Como um administrador pode gerenciar o acesso de convidados com Azure AD revisões de acesso](/azure/active-directory/active-directory-azure-ad-controls-manage-guest-access-with-access-reviews)


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

