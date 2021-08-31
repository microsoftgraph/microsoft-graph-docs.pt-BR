---
title: Tipo de recurso deviceManagementSettingInstance
description: Tipo de base para uma instância de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5f4f2e9d6f3aa80da158cfae6e4f9863334e8491
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/31/2021
ms.locfileid: "58800384"
---
# <a name="devicemanagementsettinginstance-resource-type"></a>Tipo de recurso deviceManagementSettingInstance

Namespace: microsoft.graph

> **Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.

> **Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.

Tipo de base para uma instância de configuração

## <a name="methods"></a>Métodos
|Método|Tipo de retorno|Descrição|
|:---|:---|:---|
|[Listar deviceManagementSettingInstances](../api/intune-deviceintent-devicemanagementsettinginstance-list.md)|[Coleção deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Listar propriedades e relações dos [objetos deviceManagementSettingInstance.](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|
|[Obter deviceManagementSettingInstance](../api/intune-deviceintent-devicemanagementsettinginstance-get.md)|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|Leia propriedades e relações do [objeto deviceManagementSettingInstance.](../resources/intune-deviceintent-devicemanagementsettinginstance.md)|

## <a name="properties"></a>Propriedades
|Propriedade|Tipo|Descrição|
|:---|:---|:---|
|id|Cadeia de caracteres|A ID da instância de configuração|
|definitionId|Cadeia de caracteres|A ID da definição de configuração para esta instância|
|valueJson|Cadeia de caracteres|Representação JSON do valor|

## <a name="relationships"></a>Relações
Nenhum

## <a name="json-representation"></a>Representação JSON
Veja a seguir uma representação JSON do recurso.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String"
}
```



