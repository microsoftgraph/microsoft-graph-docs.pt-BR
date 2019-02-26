---
title: tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma política de termos e condições (T&C) determinada para um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8b5b97e691ff16ce2c86057ab5dae229d8657974
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142683"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>tipo de recurso termsAndConditionsGroupAssignment

> **Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

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
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
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




