---
title: Revisões de acesso ao Azure AD
description: Você pode usar as análises de acesso do Azure AD para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário. Esta documentação atende à versão 2nd das APIs.
localization_priority: Normal
author: isabelleatmsft
ms.prod: governance
doc_type: conceptualPageType
ms.openlocfilehash: 21fb21426d6168694e2fc05410f582070074edae
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/19/2021
ms.locfileid: "53030912"
---
# <a name="azure-ad-access-reviews"></a>Revisões de acesso ao Azure AD

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

[!INCLUDE [accessreviews-disclaimer-v2](../../includes/accessreviews-disclaimer-v2.md)]


Você pode usar as análises de acesso do [Azure AD](/azure/active-directory/active-directory-azure-ad-controls-access-reviews-overview) para configurar análises de acesso única ou recorrentes para atestar os direitos de acesso do usuário.

Cenários de cliente típicos para análises de acesso de associações de grupo e de aplicativos e acesso a função do Azure AD são:

- Os clientes podem revisar e certificar o acesso do usuário convidado a aplicativos, funções do Azure AD e associações de grupos. Os revisadores podem usar as informações fornecidas para decidir com eficiência se os convidados devem ter acesso contínuo.

- Os clientes podem revisar e certificar o acesso de funcionários a aplicativos, funções do Azure AD e associações de grupo com avaliações de acesso.

Observe que o recurso de críticas de acesso, incluindo a API, está incluído Azure AD Premium P2.  O locatário em que uma revisão de acesso está sendo criada deve ter uma assinatura válida de compra ou avaliação Azure AD Premium P2 ou EMS E5.


## <a name="methods"></a>Methods

A tabela a seguir lista os métodos que você pode usar para interagir com recursos relacionados à revisão de acesso.

| Método           | Tipo de retorno    |Descrição|
|:---------------|:--------|:----------|
|[Listar accessReviewScheduleDefinitions](../api/accessreviewscheduledefinition-list.md) | [Coleção accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter uma lista dos [objetos accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) e suas propriedades. |
|[Obter accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-get.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Obter um objeto accessReviewScheduleDefinition e suas propriedades. |
|[Criar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-post.md) | [accessReviewScheduleDefinition](accessreviewscheduledefinition.md) | Crie um novo accessReviewScheduleDefinition. |
|[Excluir accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-delete.md) | Nenhum. | Exclua um accessReviewScheduleDefinition. |
|[Atualizar accessReviewScheduleDefinition](../api/accessreviewscheduledefinition-update.md) | Nenhum. | Atualizar propriedades de um accessReviewScheduleDefinition com um identificador especificado. |
|[accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário de chamada é um revistor em uma ou mais instâncias.|
|[Listar accessReviewInstances](../api/accessreviewinstance-list.md) | [Coleção accessReviewInstance](accessreviewinstance.md) | Obter uma lista dos [objetos accessReviewInstance](../resources/accessreviewinstance.md) e suas propriedades. |
|[Obter accessReviewInstance](../api/accessreviewinstance-get.md) | [accessReviewInstance](accessreviewinstance.md) | Leia as propriedades e as relações de um [objeto accessReviewInstance.](../resources/accessreviewinstance.md) |
|[Enviar lembrete accessReviewInstance](../api/accessreviewinstance-sendreminder.md) | Nenhum. | Envie um lembrete aos revisores de um accessReviewInstance. |
|[Parar accessReviewInstance](../api/accessreviewinstance-stop.md) | Nenhum. | Pare manualmente um accessReviewInstance. |
|[Aceitar recomendações](../api/accessreviewinstance-acceptrecommendations.md) | Nenhum. | Permite que o usuário de chamada aceite a recomendação de decisão para cada acesso NotReviewInstanceDecisionItem em que ele é o revisor para um accessReviewInstance específico. |
|[Aplicar decisões](../api/accessreviewinstance-applydecisions.md) | Nenhum. | Aplicar decisões manualmente em um accessReviewInstance. |
|[Decisões de registro em lotes](../api/accessreviewinstance-batchrecorddecisions.md)|Nenhum|Revise lotes de entidades ou recursos em uma chamada.|
|[Redefinir decisões](../api/accessreviewinstance-resetdecisions.md)|Nenhum|Redefine todos os itens de decisão em uma instância para `notReviewed` .|
|[accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md)|[Coleção accessReviewInstance](../resources/accessreviewinstance.md)|Retorna todas as instâncias em um [determinado accessReviewScheduleDefinition](accessreviewscheduledefinition.md) para o qual o usuário de chamada é o revisor de uma ou mais decisões.|
|[Listar accessReviewInstanceDecisionItems](../api/accessreviewinstancedecisionitem-list.md) | [Coleção accessReviewInstanceDecisionItem](accessreviewinstancedecisionitem.md) | Obter uma lista dos [objetos accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md) e suas propriedades.|
|[Obter accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-get.md)|[accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Leia as propriedades e as relações de um [objeto accessReviewInstanceDecisionItem.](../resources/accessreviewinstancedecisionitem.md)|
|[Atualizar accessReviewInstanceDecisionItem](../api/accessreviewinstancedecisionitem-update.md) | Nenhum. | Para qualquer accessReviewInstanceDecisionItems em que o usuário de chamada recebe um revisor, chamar o usuário pode registrar uma decisão corrigindo o objeto decision. |
|[accessReviewInstanceDecisionItem: filterByCurrentUser](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md)|[Coleção accessReviewInstanceDecisionItem](../resources/accessreviewinstancedecisionitem.md)|Recupera todos os [objetos accessReviewInstanceDecisionItems](accessreviewinstancedecisionitem.md) onde o uso de chamada é o revisor de um [dado accessReviewInstance](accessreviewinstance.md).|
|[Listar accessReviewHistoryDefinitions](../api/accessreviewhistorydefinition-list.md)|[Coleção accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Obter uma lista dos [objetos accessReviewHistoryDefinition](accessreviewhistorydefinition.md) e suas propriedades.|
|[Criar accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-post.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Crie um novo [objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[Obter accessReviewHistoryDefinition](../api/accessreviewhistorydefinition-get.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Leia as propriedades e as relações de [um objeto accessReviewHistoryDefinition.](accessreviewhistorydefinition.md)|
|[generateDownloadUri](../api/accessreviewhistorydefinition-generatedownloaduri.md)|[accessReviewHistoryDefinition](accessreviewhistorydefinition.md)|Gere um URI que pode ser usado para recuperar dados de histórico de revisão.|
|[Obter accessReviewPolicy](../api/accessreviewpolicy-get.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Leia as propriedades e as relações de um [objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)|
|[Atualizar accessReviewPolicy](../api/accessreviewpolicy-update.md)|[accessReviewPolicy](../resources/accessreviewpolicy.md)|Atualize as propriedades de [um objeto accessReviewPolicy.](../resources/accessreviewpolicy.md)|
|[Listar definições pendentes de aprovação (preterida)](../api/accessreviewscheduledefinition-filterbycurrentuser.md)|[Coleção accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md)|Recupera todas as definições para as quais o usuário de chamada é um revistor em uma ou mais instâncias. Este método está sendo preterido e substituído por [accessReviewScheduleDefinition: filterByCurrentUser](../api/accessreviewscheduledefinition-filterbycurrentuser.md).|
|[Lista pendingAccessReviewInstances (preterido)](../api/accessreviewinstance-pendingaccessreviewinstances.md) | [Coleção accessReviewInstance.](accessreviewinstance.md) | Obter todos os recursos de accessReviewInstance pendentes atribuídos ao usuário de chamada. Este método está sendo preterido e substituído por [accessReviewInstance: filterByCurrentUser](../api/accessreviewinstance-filterbycurrentuser.md). |
|[Listar accessReviewInstanceDecisionItems pendente aprovação (preterida)](../api/accessreviewinstancedecisionitem-listpendingapproval.md) | [Coleção accessReviewInstanceDecisionItem.](accessreviewinstancedecisionitem.md) | Obter todos os accessReviewInstanceDecisionItems atribuídos ao usuário de chamada, para um accessReviewInstance específico. Este método está sendo preterido e substituído por [accessReviewInstanceDecisionItem: filterByCurrentUse](../api/accessreviewinstancedecisionitem-filterbycurrentuser.md). |

## <a name="role-and-application-permission-authorization-checks"></a>Verificações de autorização de função e permissão de aplicativo

As seguintes funções de diretório são necessárias para que um usuário de chamada gerencie as análises de acesso. 

| Operação | Permissões de aplicativos | Função de diretório necessária do usuário chamador |
|:------------------|:------------|:--------------------------------------------|
| Leitura | AccessReview.Read.All ou AccessReview.ReadWrite.All | Administrador Global, Leitor Global, Administrador de Segurança, Leitor de Segurança ou Administrador do Usuário |
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

