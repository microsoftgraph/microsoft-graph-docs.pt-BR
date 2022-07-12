---
title: Tipo de recurso termsAndConditionsAssignment
description: Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 54869ceb0215427b30cd9e7db125212bf480f94a
ms.sourcegitcommit: 7c1f2df6599638963e28dc89491eafb4b81f4e8e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2022
ms.locfileid: "66732434"
---
# <a name="termsandconditionsassignment-resource-type"></a>Tipo de recurso termsAndConditionsAssignment

Namespace: microsoft.graph

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma entidade termsAndConditionsAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um certo grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsAssignments](../api/intune-companyterms-termsandconditionsassignment-list.md)|Coleção [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Propriedades de leitura e relações dos objetos [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Obter termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-get.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Propriedades de leitura e relações do objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Criar termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-create.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Cria um novo objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Excluir termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-delete.md)|Nenhum|Exclui um [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|
|[Atualizar termsAndConditionsAssignment](../api/intune-companyterms-termsandconditionsassignment-update.md)|[termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md)|Atualiza as propriedades de um objeto [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md).|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade.|
|destino|[deviceAndAppManagementAssignmentTarget](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|Destino de atribuição ao qual a política de T&C foi designada.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "collectionId": "String"
  }
}
```





