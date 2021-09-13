---
title: Tipo de recurso adminConsentRequestPolicy
description: Especifica a política pela qual as solicitações de consentimento podem ser criadas e gerenciadas para todo o locatário.
author: psignoret
ms.localizationpriority: medium
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: eb2a2bdc94b900d28c5446524d32251dd76027b5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59094489"
---
# <a name="adminconsentrequestpolicy-resource-type"></a>Tipo de recurso adminConsentRequestPolicy

Namespace: microsoft.graph

Especifica a política pela qual as solicitações de consentimento são criadas e gerenciadas para todo o locatário. Há um único **adminConsentRequestPolicy** por locatário.

O **adminConsentRequestPolicy** fornece configurações adicionais ao criar uma solicitação de consentimento para controlar o comportamento do recurso ao iniciar uma solicitação de consentimento.

## <a name="methods"></a>Métodos

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Obter adminConsentRequestPolicy](../api/adminconsentrequestpolicy-get.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|Leia as propriedades e as relações de um [objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)|
|[Atualizar adminConsentRequestPolicy](../api/adminconsentrequestpolicy-update.md)|[adminConsentRequestPolicy](../resources/adminconsentrequestpolicy.md)|Atualize as propriedades de [um objeto adminConsentRequestPolicy.](../resources/adminconsentrequestpolicy.md)|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|isEnabled|Booliano|Especifica se o recurso de solicitação de consentimento do administrador está habilitado ou desabilitado. Obrigatório.|
|notifyReviewers|Boolean|Especifica se os revisadores receberão notificações. Obrigatório.|
|remindersEnabled|Boolean|Especifica se os revisadores receberão emails de lembrete. Obrigatório.|
|requestDurationInDays|Int32|Especifica a duração em que a solicitação está ativa antes de expirar automaticamente se nenhuma decisão for aplicada.|
|revisadores|[Coleção accessReviewReviewerScope](../resources/accessreviewreviewerscope.md)|A lista de revisadores para o consentimento do administrador. Obrigatório.|
|versão|Int32|Especifica a versão dessa política. Quando a política é atualizada, essa versão é atualizada. Somente leitura.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.adminConsentRequestPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.adminConsentRequestPolicy",
  "isEnabled": "Boolean",
  "version": "Integer",
  "notifyReviewers": "Boolean",
  "remindersEnabled": "Boolean",
  "requestDurationInDays": "Integer",
  "reviewers": [
    {
      "@odata.type": "microsoft.graph.accessReviewReviewerScope"
    }
  ]
}
```

