---
title: Tipo de recurso termsAndConditionsGroupAssignment
description: Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1c63f466c007abcf4f402bc483f4a4d1e1bed740
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59106634"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>Tipo de recurso termsAndConditionsGroupAssignment

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma entidade termsAndConditionsGroupAssignment representa a atribuição de uma determinada política de Termos e Condições (T&C) a um determinado grupo. Os usuários do grupo deverão aceitar os termos para que seus dispositivos sejam registrados no Intune.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar termsAndConditionsGroupAssignments](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|[Coleção termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Listar propriedades e relações dos [objetos termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|
|[Obter termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Leia propriedades e relações do [objeto termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|
|[Criar termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Crie um novo [objeto termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|
|[Excluir termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|Nenhum|Exclui um [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md).|
|[Atualizar termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|Atualize as propriedades de [um objeto termsAndConditionsGroupAssignment.](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Identificador exclusivo da entidade.|
|targetGroupId|Cadeia de Caracteres|Identificador exclusivo de um grupo ao&C atribuído.|

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



