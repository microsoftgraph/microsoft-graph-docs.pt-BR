---
title: Tipo de recurso delegatedAdminRelationship
description: Representa os detalhes dos privilégios administrativos delegados que um parceiro da Microsoft tem em um locatário do cliente.
author: adtangir
ms.localizationpriority: medium
ms.prod: customer-relationship-management
doc_type: resourcePageType
ms.openlocfilehash: 753212cabaf62f8bbfc5e119f3322b797d6559f8
ms.sourcegitcommit: ffa80f25d55aa37324368b6491d5b7288797285f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/01/2022
ms.locfileid: "65820627"
---
# <a name="delegatedadminrelationship-resource-type"></a>Tipo de recurso delegatedAdminRelationship

Namespace: microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Representa uma relação de administrador delegado entre um parceiro e um cliente.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Criar delegatedAdminRelationship](../api/tenantrelationship-post-delegatedadminrelationships.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Crie um novo **objeto delegatedAdminRelationship** .|
|[Listar delegatedAdminRelationships](../api/tenantrelationship-list-delegatedadminrelationships.md)|[coleção delegatedAdminRelationship](delegatedadminrelationship.md)|Obtenha uma lista dos **objetos delegatedAdminRelationship** e suas propriedades.|
|[Obter delegatedAdminRelationship](../api/delegatedadminrelationship-get.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Leia as propriedades e as relações de um **objeto delegatedAdminRelationship** .|
|[Atualizar delegatedAdminRelationship](../api/delegatedadminrelationship-update.md)|[delegatedAdminRelationship](delegatedadminrelationship.md)|Atualize as propriedades de **um objeto delegatedAdminRelationship** .|
|[Excluir delegatedAdminRelationship](../api/delegatedadminrelationship-delete.md)|Nenhum|**Exclua um objeto delegatedAdminRelationship**.|


## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|accessDetails|[delegatedAdminAccessDetails](../resources/delegatedadminaccessdetails.md)|Os detalhes de acesso que contêm os identificadores das funções administrativas que o administrador do parceiro está solicitando no locatário do cliente.|
|activatedDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e na hora UTC em que a relação se tornou ativa. Somente leitura.|
|createdDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e na hora UTC em que a relação foi criada. Somente leitura.|
|Cliente|[delegatedAdminRelationshipCustomerParticipant](../resources/delegatedadminrelationshipcustomerparticipant.md)|O nome de exibição e o identificador exclusivo do cliente da relação. Isso é configurado pelo parceiro no momento em que a relação é criada ou pelo sistema depois que o cliente aprova a relação. Não pode ser alterado pelo cliente.|
|displayName|Cadeia de caracteres|O nome de exibição da relação usada para facilitar a identificação. Deve ser exclusivo em *todas as* relações de administrador delegado do parceiro. Isso é definido pelo parceiro somente quando a relação está no `created` status e não pode ser alterada pelo cliente.|
|duração|Duration|A duração da relação no formato ISO 8601. Deve ser um valor entre e `P1D` `P2Y` inclusivo. Isso é definido pelo parceiro somente quando a relação está no `created` status e não pode ser alterada pelo cliente.|
|endDateTime|DateTimeOffset|A data e a hora no formato ISO 8601 e no horário UTC quando o **status** da relação é alterado para um `terminated` ou `expired`. Calculado como `endDateTime = activatedDateTime + duration`. Somente leitura.|
|id|Cadeia de caracteres|O identificador exclusivo da relação. Somente leitura. Herdado da [entidade](../resources/entity.md).|
|lastModifiedDateTime|DateTimeOffset|A data e hora no formato ISO 8601 e na hora UTC em que a relação foi modificada pela última vez. Somente leitura.|
|status|delegatedAdminRelationshipStatus|O status da relação. Somente leitura. Os valores possíveis são: , , , , , `created`, `expired`, `expiring`, `terminated`, , `terminating`, `terminationRequested`, `unknownFutureValue`. `approved``approvalPending``active``activating` Suporta o `$orderBy`.|

### <a name="delegatedadminrelationshipstatus-values"></a>valores delegatedAdminRelationshipStatus 
| Member | Descrição |
| --- | --- |
| criadas | O parceiro criou uma nova relação. Nesse estado, a relação pode ser modificada. |
| approvalPending | O parceiro finalizou a relação por meio da `lockForApproval` ação de um objeto [delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) . |
| Aprovado | O cliente aprovou a relação por meio da `approve` ação de um objeto [delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) . |
| Ativar | O sistema inicia o provisionamento da relação. |
| Ativo | O sistema conclui o provisionamento da relação. |
| Expirando | A relação passou pela data de validade. |
| Expirado | O sistema conclui o des provisionamento da relação. |
| terminationRequested | O parceiro ou cliente solicitou o encerramento `terminate` da relação por meio da ação de um objeto [delegatedAdminRelationshipRequest](delegatedadminrelationshiprequest.md) . |
| Terminação | O sistema inicia o des provisionamento da relação. |
| Terminada | O sistema concluiu o des provisionamento da relação. |
| unknownFutureValue | Valor de sentinel de enumeração evolvável. Não usar. |

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|accessAssignments|[coleção delegatedAdminAccessAssignment](../resources/delegatedadminaccessassignment.md)|As atribuições de acesso associadas à relação de administrador delegado.|
|operations|[coleção delegatedAdminRelationshipOperation](../resources/delegatedadminrelationshipoperation.md)|As operações de execução longa associadas à relação de administrador delegado.|
|Solicitações|[coleção delegatedAdminRelationshipRequest](../resources/delegatedadminrelationshiprequest.md)|As solicitações associadas à relação de administrador delegado.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.delegatedAdminRelationship",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.delegatedAdminRelationship",
  "id": "String (identifier)",
  "displayName": "String",
  "duration": "String",
  "customer": {
    "@odata.type": "microsoft.graph.delegatedAdminRelationshipCustomerParticipant"
  },
  "accessDetails": {
    "@odata.type": "microsoft.graph.delegatedAdminAccessDetails"
  },
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "activatedDateTime": "String (timestamp)",
  "endDateTime": "String (timestamp)"
}
```

