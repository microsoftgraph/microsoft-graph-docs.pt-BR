---
title: tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4e1caee5aebd46f6958077a9fea474327c629af0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273834"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>tipo de recurso termsAndConditionsGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsGroupAssignments](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|coleção [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Listar Propriedades e relações dos objetos [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Obter termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Leia as propriedades e as relações do objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Criar termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Criar um novo objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|
|[Excluir termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|Nenhum|Exclui [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).|
|[Atualizar termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Atualiza as propriedades de um objeto [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) .|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo da entidade.|
|targetGroupId|String|Identificador exclusivo de um grupo ao qual a política T&C é atribuída.|

## <a name="relationships"></a>Relações
|Relação|Tipo|Descrição|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|Link de navegação para os termos e condições atribuídos.|

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




