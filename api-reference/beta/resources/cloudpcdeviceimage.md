---
title: tipo de recurso cloudPcDeviceImage
description: Representa o recurso de imagem no PC de nuvem.
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 600fceffadb03247c646b2728e445c0c07cae9aa
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378266"
---
# <a name="cloudpcdeviceimage-resource-type"></a>tipo de recurso cloudPcDeviceImage

Namespace: microsoft.graph

Representa o recurso de imagem no PC de nuvem.

## <a name="methods"></a>Methods

|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceImages](../api/virtualendpoint-list-deviceimages.md)|coleção [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Listar as propriedades e as relações dos objetos [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Obter cloudPcDeviceImage](../api/cloudpcdeviceimage-get.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Leia as propriedades e os relacionamentos de um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Criar cloudPcDeviceImage](../api/virtualendpoint-post-deviceimages.md)|[cloudPcDeviceImage](../resources/cloudpcdeviceimage.md)|Criar um novo objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[Excluir cloudPcDeviceImage](../api/cloudpcdeviceimage-delete.md)|Nenhum|Excluir um objeto [cloudPcDeviceImage](../resources/cloudpcdeviceimage.md) .|
|[getSourceImages](../api/cloudpcdeviceimage-getsourceimages.md)|coleção [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md)|Obter objetos [cloudPcSourceDeviceImage](../resources/cloudpcsourcedeviceimage.md) .|

## <a name="properties"></a>Propriedades

|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|String|Identificador exclusivo do recurso de imagem no PC de nuvem. Somente leitura.|
|sourceImageResourceId|Cadeia de Caracteres|A ID do recurso de imagem de origem no Azure. Formato obrigatório: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Compute/images/{imageName}".|
|displayName|String|O nome de exibição da imagem.|
|versão|String|A versão da imagem. Por exemplo: 0.0.1, 1.5.13.|
|osBuildNumber|Cadeia de Caracteres|A versão de compilação do so da imagem. Por exemplo: 1909.|
|operatingSystem|String|O sistema operacional da imagem. Por exemplo: Windows 10 Enterprise.|
|lastModifiedDateTime|DateTimeOffset|Os dados e hora em que a imagem foi modificada pela última vez. O horário é mostrado no formato ISO 8601 e no tempo universal coordenado (UTC). Por exemplo, meia-noite UTC em 1º de janeiro de 2014 aparece como ' 2014-01-01T00:00:00Z '.|
|status|cloudPcDeviceImageStatus|O status da imagem no computador de nuvem. Status possível incluem upload pendente, falha ao carregar ou pronto para usar. Os valores possíveis são: `pending`, `ready`, `failed`.|
|statusDetails|cloudPcDeviceImageStatusDetails|Os detalhes do status da imagem, que indica por que o carregamento falhou, se aplicável. Os valores possíveis são: `internalServerError`, `sourceImageNotFound`.|

## <a name="relationships"></a>Relações

Nenhum

## <a name="json-representation"></a>Representação JSON

Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.cloudPcDeviceImage",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.cloudPcDeviceImage",
  "id": "String (identifier)",
  "displayName": "String",
  "operatingSystem": "String",
  "osBuildNumber": "String",
  "version": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "statusDetails": "String",
  "sourceImageResourceId": "String"
}
```
