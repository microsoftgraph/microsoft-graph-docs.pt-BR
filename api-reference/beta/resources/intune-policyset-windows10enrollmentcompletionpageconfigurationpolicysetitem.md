---
title: Tipo de recurso windows10EnrollmentCompletionPageConfigurationPolicySetItem
description: Uma classe que contém as propriedades usadas para Windows10EnrollmentCompletionPageConfiguration PolicySetItem.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7e167f1af87b9e70ea828b7aa081221d0b4f244c
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2021
ms.locfileid: "58255568"
---
# <a name="windows10enrollmentcompletionpageconfigurationpolicysetitem-resource-type"></a>Tipo de recurso windows10EnrollmentCompletionPageConfigurationPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para Windows10EnrollmentCompletionPageConfiguration PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar windows10EnrollmentCompletionPageConfigurationPolicySetItems](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-list.md)|[Coleção windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Listar propriedades e relações dos [objetos windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|
|[Obter windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-get.md)|[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Leia propriedades e relações do [objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|
|[Criar windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-create.md)|[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Crie um novo [objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|
|[Excluir windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-delete.md)|Nenhum|Exclui um [windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md).|
|[Atualizar windows10EnrollmentCompletionPageConfigurationPolicySetItem](../api/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem-update.md)|[windows10EnrollmentCompletionPageConfigurationPolicySetItem](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|Atualize as propriedades de [um objeto windows10EnrollmentCompletionPageConfigurationPolicySetItem.](../resources/intune-policyset-windows10enrollmentcompletionpageconfigurationpolicysetitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Chave do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Cadeia de caracteres|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|Cadeia de caracteres|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|String collection|Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)|
|prioridade|Int32|Prioridade do Windows10EnrollmentCompletionPageConfigurationPolicySetItem.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10EnrollmentCompletionPageConfigurationPolicySetItem",
  "id": "String (identifier)",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "payloadId": "String",
  "itemType": "String",
  "displayName": "String",
  "status": "String",
  "errorCode": "String",
  "guidedDeploymentTags": [
    "String"
  ],
  "priority": 1024
}
```




