---
title: Tipo de recurso mdmWindowsInformationProtectionPolicyPolicySetItem
description: Uma classe que contém as propriedades usadas para a política de proteção de informações do windows mdm PolicySetItem.
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5fe7bfea53392ad33496fd59ce0dcb83bb93efe8
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080713"
---
# <a name="mdmwindowsinformationprotectionpolicypolicysetitem-resource-type"></a>Tipo de recurso mdmWindowsInformationProtectionPolicyPolicySetItem

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Uma classe que contém as propriedades usadas para a política de proteção de informações do windows mdm PolicySetItem.


Herda de [policySetItem](../resources/intune-policyset-policysetitem.md)

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar mdmWindowsInformationProtectionPolicyPolicySetItems](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-list.md)|[Coleção mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Listar propriedades e relações dos [objetos mdmWindowsInformationProtectionPolicyPolicySetItem.](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|
|[Obter mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-get.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Leia propriedades e relações do [objeto mdmWindowsInformationProtectionPolicyPolicySetItem.](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|
|[Criar mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-create.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Crie um novo [objeto mdmWindowsInformationProtectionPolicyPolicySetItem.](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|
|[Excluir mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-delete.md)|Nenhum|Exclui um [mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md).|
|[Atualizar mdmWindowsInformationProtectionPolicyPolicySetItem](../api/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem-update.md)|[mdmWindowsInformationProtectionPolicyPolicySetItem](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|Atualize as propriedades de [um objeto mdmWindowsInformationProtectionPolicyPolicySetItem.](../resources/intune-policyset-mdmwindowsinformationprotectionpolicypolicysetitem.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Chave do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|createdDateTime|DateTimeOffset|Hora de criação do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|lastModifiedDateTime|DateTimeOffset|Última hora modificada do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|payloadId|Cadeia de Caracteres|PayloadId do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|itemType|String|policySetType do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|displayName|Cadeia de caracteres|DisplayName do PolicySetItem. Herdado de [policySetItem](../resources/intune-policyset-policysetitem.md)|
|status|[policySetStatus](../resources/intune-policyset-policysetstatus.md)|Status do PolicySetItem. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `unknown`, `validating`, `partialSuccess`, `success`, `error`, `notAssigned`.|
|errorCode|[errorCode](../resources/intune-policyset-errorcode.md)|Código de erro se ocorrer algum. Herdado [de policySetItem](../resources/intune-policyset-policysetitem.md). Os valores possíveis são: `noError`, `unauthorized`, `notFound`, `deleted`.|
|guidedDeploymentTags|Conjunto de cadeias de caracteres|Marcas da implantação guiada Herdadas [de policySetItem](../resources/intune-policyset-policysetitem.md)|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mdmWindowsInformationProtectionPolicyPolicySetItem",
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
  ]
}
```



