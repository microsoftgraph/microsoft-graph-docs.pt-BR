---
title: Tipo de recurso groupPolicyObjectFile
description: O arquivo objeto De política de grupo carregado pelo administrador.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fd832adbed7a8a843c5a6e8ec9df37a5c621a1d8d89df1abfb20a8afaef45ef
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/05/2021
ms.locfileid: "54249815"
---
# <a name="grouppolicyobjectfile-resource-type"></a>Tipo de recurso groupPolicyObjectFile

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

O arquivo objeto De política de grupo carregado pelo administrador.

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar groupPolicyObjectFiles](../api/intune-gpanalyticsservice-grouppolicyobjectfile-list.md)|[coleção groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Listar propriedades e relações dos [objetos groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|
|[Obter groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-get.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Leia propriedades e relações do [objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|
|[Criar groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-create.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Crie um novo [objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|
|[Excluir groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-delete.md)|Nenhum|Exclui um [groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md).|
|[Atualizar groupPolicyObjectFile](../api/intune-gpanalyticsservice-grouppolicyobjectfile-update.md)|[groupPolicyObjectFile](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|Atualize as propriedades de [um objeto groupPolicyObjectFile.](../resources/intune-gpanalyticsservice-grouppolicyobjectfile.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|Ainda não documentado|
|groupPolicyObjectId|Guid|O GUID do objeto de política de grupo do conteúdo XML do GPO|
|ouDistinguishedName|Cadeia de caracteres|O nome diferenciado da UO.|
|createdDateTime|DateTimeOffset|A data e a hora em que GroupPolicy foi carregado pela primeira vez.|
|lastModifiedDateTime|DateTimeOffset|A data e a hora em que GroupPolicyObjectFile foi modificado pela última vez.|
|content|Cadeia de caracteres|O conteúdo do arquivo de objeto de Política de Grupo.|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "id": "String (identifier)",
  "groupPolicyObjectId": "Guid",
  "ouDistinguishedName": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "content": "String"
}
```




